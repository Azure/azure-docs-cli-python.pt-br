---
title: Usar a CLI do Azure com eficiência
description: Dicas para usar a CLI do Azure com eficácia
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 11/18/2020
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 598d7498d17078bdd9f3f1aa9dc2ca4447ca97b2
ms.sourcegitcommit: bd2dbc80328936dadd211764d25c32a14fc58083
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/04/2021
ms.locfileid: "97857794"
---
# <a name="use-azure-cli-effectively"></a>Usar a CLI do Azure com eficiência

Para maior clareza, os scripts Bash são embutidos. Os exemplos do PowerShell ou do lote do Windows são listados no apêndice, que pode ser usado para criar exemplos semelhantes.

## <a name="output-formatting-json-table-or-tsv"></a>Formatação de saída (JSON, tabela ou TSV)

1. O formato `json` é o padrão da CLI e destina-se a fornecer as informações mais abrangentes. Se você preferir um formato diferente, use o argumento `--output` para substituir uma invocação de comando individual ou use `az configure` para atualizar o seu padrão global. Observe que o formato JSON preserva as aspas duplas, geralmente tornando-as inadequadas para fins de script.

2. O `table` é útil para obter um resumo das informações centralizadas, especialmente para comandos de lista. Se você não gostar dos campos no formato de tabela padrão (ou não houver um formato padrão), poderá usar `--output json` para ver todas as informações ou usar o `--query` para especificar o formato que deseja.

    ```sh
    az vm show -g my_rg -n my_vm --query "{name: name, os:storageProfile.imageReference.offer}" -otable
    Name    Os
    ------  ------------
    my_vm   UbuntuServer
    ```

3. `tsv` é útil para fins de script e de saída concisos. O TSV removerá aspas duplas que o formato JSON preserva. Para especificar o formato desejado para o TSV, use o argumento `--query`.

    ```sh
    export vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    az vm stop --ids $vm_ids
    ```

## <a name="pass-values-from-one-command-to-another"></a>Passar valores de um comando para o outro

1. Se o valor for usado mais de uma vez, atribua-o a uma variável. Observe o uso de `-o tsv` no seguinte exemplo:

    ```sh
    running_vm_ids=$(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
    ```
2. Se o valor for usado apenas uma vez, considere usar pipe:
    ```sh
    az vm list --query "[?powerState=='VM running'].name" | grep my_vm
    ```
3. Para listas, considere as seguintes sugestões:

   Se você precisar de mais controles no resultado, use o loop "for":
    ```sh
    #!/usr/bin/env bash
    for vm in $(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv); do
        echo stopping $vm
        az vm stop --ids $vm
        if [ $? -ne 0 ]; then
            echo "Failed to stop $vm"
            exit 1
        fi
        echo $vm stopped
    done
    ```

    Como alternativa, use `xargs` e considere usar o sinalizador `-P` para executar as operações em paralelo para melhor desempenho:
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | xargs -I {} -P 10 az vm start --ids "{}"
    ```
    Por fim, a CLI do Azure tem suporte interno para processar comandos com vários `--ids` em paralelo de modo a obter o mesmo efeito de xargs. Observe que `@-` é usado para obter valores do pipe:
    ```sh
    az vm list -d -g my_rg --query "[?powerState=='VM stopped'].id" -o tsv | az vm start --ids @-
    ```

## <a name="async-operations"></a>Operações assíncronas

Muitos comandos e grupos expõem sinalizadores `--no-wait` nas suas operações de execução prolongada, além de um comando `wait` dedicado. Eles se tornam úteis para determinados cenários:

1. Limpar recursos quando você não depende da limpeza para uma operação subsequente, como excluir um grupo de recursos:
    ```sh
    az group delete -n my_rg --no-wait
    ```
2. Quando você quiser criar vários recursos independentes em paralelo. Isso é semelhante a criar e unir threads:

    ```sh
    az vm create -g my_rg -n vm1 --image centos --no-wait
    az vm create -g my_rg -n vm2 --image centos --no-wait

    subscription=$(az account show --query "id" -otsv)
    vm1_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm1"
    vm2_id="/subscriptions/$subscription/resourceGroups/my_rg/providers/Microsoft.Compute/virtualMachines/vm2"
    az vm wait --created --ids $vm1_id $vm2_id
    ```

## <a name="generic-update-arguments"></a>Argumentos de atualização genéricos

A maioria dos comandos de atualização no recurso de CLI têm os três argumentos genéricos: `--add`, `--set` e `--remove`. Esses argumentos são poderosos, mas geralmente menos convenientes do que os argumentos fortemente tipados normalmente presentes em comandos de atualização. A CLI fornece argumentos fortemente tipados nos cenários mais comuns para facilitar o uso, mas se a propriedade que você deseja definir não estiver listada, os argumentos de atualização genérica geralmente apresentarão um caminho de desbloqueio sem a necessidade de aguardar uma nova versão.

1. A sintaxe de atualização genérica não é muito amigável, portanto, ela exigirá paciência.
2. Verifique se o grupo `Generic Update Arguments` está exposto no comando de atualização. Se não estiver, você precisará reportar um problema, mas se estiver, você poderá tentar o cenário usando-o.
3. Use o comando `show` no recurso que você está interessado para descobrir qual caminho você deve fornecer nos argumentos genéricos. Por exemplo, antes de experimentar `az vm update`, execute `az vm show` para determinar o caminho correto. De modo geral, você usará a sintaxe Dot para acessar as propriedades do dicionário e os colchetes para indexar em listas.
4. Confira os exemplos de trabalho para começar. `az vm update -h` tem bons exemplos.
5. `--set` e `--add` obtêm uma lista de pares chave-valor no formato de `<key1>=<value1> <key2>=<value2>`. Use-os para construir conteúdos não triviais. Se a sintaxe receber mensagens demais, considere usar uma cadeia de caracteres JSON. Por exemplo, para anexar um novo disco de dados a uma VM:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks "{\"createOption\": \"Attach\", \"managedDisk\": {\"id\": \"/subscriptions/0b1f6471-1bf0-4dda-aec3-cb9272f09590/resourceGroups/yg/providers/Microsoft.Compute/disks/yg-disk\"}, \"lun\": 1}"
    ```
6. Talvez você ache mais útil use a convenção de `@{file}` da CLI, colocar o JSON em um arquivo e carregá-lo. Isso simplifica o comando acima para:
    ```sh
    az vm update -g my_rg -n my_vm --add storageProfile.dataDisks @~/my_disk.json
    ```

## <a name="generic-resource-commands---az-resource"></a>Comandos de recurso genéricos – `az resource`

Pode haver casos em que um serviço no qual você está interessado não tenha cobertura de comando da CLI. Você pode usar os comandos `az resource create/show/list/delete/update/invoke-action` para trabalhar com esses recursos. Veja algumas sugestões:
1. Se apenas `create/update` estiverem envolvidos, considere usar `az group deployment create`. Use os [Modelos de Início Rápido do Azure](https://github.com/Azure/azure-quickstart-templates) para obter exemplos de trabalho.
2. Confira a referência da API REST para obter o conteúdo de solicitação, a URL e a versão da API. Como um exemplo, confira os comentários da comunidade em [como criar o AppInsights](https://github.com/Azure/azure-cli/issues/5543).

## <a name="rest-api-command---az-rest"></a>Comando da API REST – `az rest`

Se nenhum argumento de atualização genérico nem `az resource` atender às suas necessidades, você poderá usar o comando `az rest` para chamar a API REST. Ele é autenticado automaticamente usando a credencial conectada e define o cabeçalho `Content-Type: application/json`.

Isso é extremamente útil para chamar a [API do Microsoft Graph](/graph/api/overview?toc=./ref/toc.json), o que não tem suporte atualmente nos comandos da CLI ([#12946](https://github.com/Azure/azure-cli/issues/12946)).

Por exemplo, para atualizar `redirectUris` para um [Aplicativo](/graph/api/resources/application), chamamos a API REST [Aplicativo de atualização](/graph/api/application-update?tabs=http) com:

```sh
# Line breaks for legibility only

# Get the application
az rest --method GET
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'

# Update `redirectUris` for `web` property
az rest --method PATCH
        --uri 'https://graph.microsoft.com/v1.0/applications/b4e4d2ab-e2cb-45d5-a31a-98eb3f364001'
        --body '{"web":{"redirectUris":["https://myapp.com"]}}'
```

Ao usar `--uri-parameters` para solicitações no formato de OData, use o caractere de escape `$` em ambientes diferentes. No `Bash`, use o caractere escape `$` como `\$`; e no `PowerShell`, use-o em `$` como `` `$``

## <a name="pass-arguments"></a>Passar argumentos

1. Se o valor de um argumento começar com um traço (como `-VerySecret`), ele será analisado como uma opção (nome do argumento, como `-n`) por [argparse](https://docs.python.org/3/library/argparse.html) (https://bugs.python.org/issue9334) ). Para forçá-lo a ser analisado como valor, use `--password="-VerySecret"`. ([Azure/azure-cli#7054](https://github.com/Azure/azure-cli/issues/7054)).
2. Se o valor de um argumento contiver caracteres especiais, como espaço em branco (` `) ou aspas (`"`, `'`), algumas regras de aspas serão aplicadas. Veja a seção abaixo:

### <a name="quoting-issues"></a>Problemas com colocações de aspas

Isso é um problema porque quando o shell de comando (Bash, Zsh, Prompt de Comando do Windows, PowerShell etc.) analisa o comando da CLI, ele interpreta as aspas e os espaços. Sempre consulte os documentos quando você não tiver certeza sobre o uso de um shell:

- Bash: [Colocação de aspas](https://www.gnu.org/software/bash/manual/html_node/Quoting.html)
- PowerShell: [Sobre as regras de colocação de aspas](/powershell/module/microsoft.powershell.core/about/about_quoting_rules)
    - Devido ao problema conhecido [#1995](https://github.com/PowerShell/PowerShell/issues/1995) do PowerShell, algumas regras extras de escape se aplicam. Consulte [Problemas com colocações de aspas no PowerShell](https://github.com/Azure/azure-cli/blob/dev/doc/quoting-issues-with-powershell.md) para obter mais informações.
- Prompt de Comando do Windows: [Instruções: caracteres de escape, delimitadores e aspas na linha de comando do Windows](https://ss64.com/nt/syntax-esc.html)

Para evitar resultados inesperados, veja algumas sugestões:

1. Se o valor contiver espaço em branco, você precisará colocá-lo em aspas.
2. No Bash ou no Windows PowerShell, as aspas simples e duplas serão interpretadas, enquanto no Prompt de Comando do Windows, apenas aspas duplas serão manipuladas, o que significa que as aspas simples serão interpretadas como parte do valor.
3. Se o comando é executado somente no Bash (ou Zsh), o uso de aspas simples tem a vantagem delimitar o conteúdo. Isso pode ser muito útil ao fornecer JSON embutido. Por exemplo, isto funciona no Bash: `'{"foo": "bar"}'`
4. Se o comando for executado no Prompt de Comando do Windows, você precisará usar exclusivamente aspas duplas. Se o valor contiver aspas duplas, você precisará usar o caractere de escape: `"i like to use \" a lot"`. O equivalente do Prompt de Comando do exemplo acima seria: `"{\"foo\": \"bar\"}"`
5. Variáveis exportadas no Bash dentro de aspas duplas serão avaliadas. Se isso não for o que você deseja, use novamente `\ ` para colocar o caractere de escape `"\$var"` ou use aspas simples `'$var'`.
6. Alguns argumentos de CLI, incluindo os argumentos de atualização genéricos, tem uma lista de valores separados por espaços, como `<key1>=<value1> <key2>=<value2>`. Como o valor e o nome da chave podem usar uma cadeia de caracteres arbitrária que pode conter espaços em branco, será necessário usar aspas. Encapsule o par, não a chave ou o valor individual. Portanto, `"my name"=john` está errado. Em vez disso, use `"my name=john"`. Por exemplo:
    ```sh
    az webapp config appsettings set -g my_rg -n my_web --settings "client id=id1" "my name=john"
    ```
7. Use a convenção de `@<file>` da CLI para carregar de um arquivo de modo a ignorar os mecanismos de interpretação do shell:
    ```sh
    az ad app create --display-name my-native --native-app --required-resource-accesses @manifest.json
    ```
8. Quando um argumento da CLI aceita uma lista separada por espaços, estes são os formatos aceitos:
    - `--arg foo bar`: OK. Lista separada por espaços sem aspas
    - `--arg "foo" "bar"`: OK: Lista separada por espaços com aspas
    - `--arg "foo bar"`: INVÁLIDO. Essa é uma cadeia de caracteres com um espaço, não uma lista separada por espaços.
9. Ao executar comandos da CLI do Azure no PowerShell, ocorrerão erros de análise se os argumentos contiverem caracteres especiais do PowerShell, como em `@`. Você pode resolver esse problema adicionando `` ` `` antes do caractere especial para usar o caractere de escape ou colocando o argumento em aspas simples ou duplas `'`/`"`. Por exemplo, `az group deployment create --parameters @parameters.json` não funciona no PowerShell porque `@` é analisado como um [símbolo de nivelamento](/powershell/module/microsoft.powershell.core/about/about_splatting). Para corrigir isso, você pode alterar o argumento para `` `@parameters.json`` ou `'@parameters.json'`.
10. Ao usar `--query` com um comando, alguns caracteres de [JMESPath](https://jmespath.org/specification.html) precisam usar o caractere de escape no shell. Por exemplo, no Bash:
    ```sh
    # Wrong, as the dash needs to be quoted in a JMESPath query
    $ az version --query azure-cli
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Wrong, as the dash needs to be quoted in a JMESPath query, but quotes are interpreted by Bash
    $ az version --query "azure-cli"
    az version: error: argument --query: invalid jmespath_type value: 'azure-cli'

    # Correct
    $ az version --query '"azure-cli"'
    "2.5.1"

    $ az version --query \"azure-cli\"
    "2.5.1"

    $ az version --query "\"azure-cli\""
    "2.5.1"
    ```

    No Prompt de Comando:
    ```cmd
    > az version --query "\"azure-cli\""
    "2.5.1"

    > az version --query \"azure-cli\"
    "2.5.1"
    ```

    No PowerShell (é necessário um escape extra):
    ```powershell
    > az version --query '\"azure-cli\"'
    "2.5.1"

    > az version --query "\`"azure-cli\`""
    "2.5.1"

    > az version --query "\""azure-cli\"""
    "2.5.1"

    > az --% version --query "\"azure-cli\""
    "2.5.1"

    > az --% version --query \"azure-cli\"
    "2.5.1"
    ```

11. A melhor maneira de solucionar um problema de colocação de aspas é executar o comando com o sinalizador `--debug`. Ele revela os argumentos reais recebidos pela CLI na [sintaxe do Python](https://docs.python.org/3/tutorial/introduction.html#strings). Por exemplo, no Bash:

    ```sh
    # Wrong, as quotes and spaces are interpreted by Bash
    $ az {"key": "value"} --debug
    Command arguments: ['{key:', 'value}', '--debug']

    # Wrong, as quotes are interpreted by Bash
    $ az {"key":"value"} --debug
    Command arguments: ['{key:value}', '--debug']

    # Correct
    $ az '{"key":"value"}' --debug
    Command arguments: ['{"key":"value"}', '--debug']

    # Correct
    $ az "{\"key\":\"value\"}" --debug
    Command arguments: ['{"key":"value"}', '--debug']
    ```

## <a name="work-behind-a-proxy"></a>Trabalhar usando um proxy

O uso do proxy é comum em redes corporativas ou é introduzido por ferramentas de rastreamento como Fiddler, mitmproxy etc. Se o proxy usar certificados autoassinados, a biblioteca de [Solicitações](https://github.com/kennethreitz/requests) do Python usada pela CLI vai gerar `SSLError("bad handshake: Error([('SSL routines', 'tls_process_server_certificate', 'certificate verify failed')],)",)`. Há dois modos de lidar com esse erro:

1. Defina a variável de ambiente `REQUESTS_CA_BUNDLE` como o caminho do arquivo de certificado do pacote de AC no formato PEM. Isso será recomendado se você usar a CLI com frequência em um proxy corporativo. O pacote de AC padrão que a CLI usa está localizado em `C:\Program Files (x86)\Microsoft SDKs\Azure\CLI2\Lib\site-packages\certifi\cacert.pem` no Windows e em ` /opt/az/lib/python3.6/site-packages/certifi/cacert.pem` no Ubuntu/Debian ou `/usr/lib64/az/lib/python3.6/site-packages/certifi/cacert.pem` no CentOS/RHEL/SUSE no Linux. Você pode acrescentar o certificado do servidor proxy nesse arquivo ou copiar o conteúdo para outro arquivo de certificado e, em seguida, definir ele como `REQUESTS_CA_BUNDLE`. Por exemplo:

    ```
    <Original cacert.pem>

    -----BEGIN CERTIFICATE-----
    <Your proxy's certificate here>
    -----END CERTIFICATE-----
    ```

   Uma pergunta frequente é se as variáveis de ambiente `HTTP_PROXY` ou `HTTPS_PROXY` devem ou não ser definidas e a resposta é: depende. Por padrão, para o Fiddler no Windows ele atua como um proxy do sistema ao iniciar, você não precisa definir nada. Se a opção estiver desativada ou usando outras ferramentas que não funcionam como proxy do sistema, você deverá defini-las. Como quase todo o tráfego da CLI é baseado em SSL, somente `HTTPS_PROXY` deve ser definido. Se você não tiver certeza, basta defini-las, mas lembre-se de remover a definição depois que o proxy for desligado. Para o Fiddler, o valor padrão é `http://localhost:8888`.

   Alguns proxies exigem autenticação, portanto, o formato das variáveis de ambiente `HTTP_PROXY` ou `HTTPS_PROXY` deverão incluir a autenticação, por exemplo, `HTTPS_PROXY="https://username:password@proxy-server:port"`. Isso será necessário para as bibliotecas subjacentes do Python. Para obter detalhes, confira [Como configurar proxies para as bibliotecas do Azure](https://docs.microsoft.com/azure/developer/python/azure-sdk-configure-proxy?tabs=bash) 

   Para obter outros detalhes, confira o [blog do Stefan](https://blog.jhnr.ch/2018/05/16/working-with-azure-cli-behind-ssl-intercepting-proxy-server/).

2. Desabilite a verificação de certificado na CLI do Azure definindo a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION=1`. Isso não é seguro, mas pode ser usado por um curto período, por exemplo, para capturar um rastreamento de rede para um comando específico e desligá-lo imediatamente quando terminar. Isso pode não funcionar para alguns comandos de plano de dados devido a limitações do SDK subjacentes.

## <a name="concurrent-builds"></a>Builds simultâneos

Se você estiver usando o AZ em um computador de build e vários trabalhos puderem ser executados em paralelo, haverá um risco de que os tokens de logon que são compartilhados entre dois trabalhos de build sejam os trabalhos executados como o mesmo usuário do sistema operacional.  Para evitar erros como esse, defina AZURE_CONFIG_DIR como um diretório no qual os tokens de logon devem ser armazenados.  Pode ser uma pasta criada aleatoriamente ou apenas o nome do workspace do Jenkins, como este ```AZURE_CONFIG_DIR=.```

## <a name="appendix"></a>Apêndice

### <a name="windows-batch-scripts-for-saving-to-variables-and-using-it-later"></a>Scripts de lote do Windows para salvar em variáveis e usar mais tarde

```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    SET "vm_ids=%%F %vm_ids%"  :: construct the id list
)
az vm stop --ids %vm_ids% :: CLI stops all VMs in parallel
```

### <a name="windows-powershell-scripts-for-saving-to-variables-and-using-it-later"></a>Scripts do Windows PowerShell para salvar em variáveis e usar mais tarde

```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
az vm stop --ids $vm_ids # CLI stops all VMs in parallel
```

### <a name="windows-batch-scripts-to-loop-through-a-list"></a>Scripts de lote do Windows para executar um loop em uma lista
```batch
ECHO OFF
SETLOCAL
FOR /F "tokens=* USEBACKQ" %%F IN (`az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv`) DO (
    ECHO Stopping %%F
    az vm stop --ids %%F
)
```

### <a name="windows-powershell-scripts-to-loop-through-a-list"></a>Scripts do Windows PowerShell para executar em loop em uma lista
```powershell
$vm_ids=(az vm list -d -g my_rg --query "[?powerState=='VM running'].id" -o tsv)
foreach ($vm_id in $vm_ids) {
    Write-Output "Stopping $vm_id"
    az vm stop --ids $vm_id
}
```

### <a name="cli-environment-variables"></a>Variáveis de ambiente da CLI

|  Variável de ambiente          | Descrição            |
|--------------------------------|------------------------|
| **AZURE_CONFIG_DIR**           | Diretório de configuração global para arquivos de configuração, logs e telemetria. Se não for especificado, o padrão será `~/.azure`. |
| **AZURE_EXTENSION_DIR**        | O diretório de instalação das extensões. Se não for especificado, o padrão será o diretório `cliextensions` no diretório de configuração global. |
