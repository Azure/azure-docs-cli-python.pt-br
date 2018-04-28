---
title: Extensão de alias da CLI do Azure 2.0
description: Como usar a extensão de alias da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/14/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40a43f5013a5dd0d7bb65b21140bb4fc82769267
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="the-azure-cli-20-alias-extension"></a>A extensão de alias da CLI do Azure 2.0

A extensão de alias permite que os usuários definam comandos personalizados para a CLI do Azure usando comandos existentes. Aliases ajudam a manter seu fluxo de trabalho simples e conciso permitindo atalhos e fornecendo a capacidade de usar argumentos posicionais. Como os aliases são ativados pelo mecanismo do modelo Jinja2, eles oferecem até mesmo o processamento avançado de argumento.

> [!NOTE]
> A Extensão do Alias está em versão prévia pública. Os recursos e o formato do arquivo de configuração podem mudar.

## <a name="install-the-alias-extension"></a>Instalar a extensão do alias

A versão mínima necessária da CLI do Azure para usar a extensão de alias é **2.0.28**. Para verificar sua versão da CLI, execute `az --version`. Se você precisa atualizar sua instalação, siga as instruções em [Instalar a CLI do Azure 2.0](./install-azure-cli.md).

Instalar a extensão com o comando [az extension add](/cli/azure/extension#az-extension-add).

```azurecli
az extension add --name alias
```

Verifique a instalação da extensão com [az extension list](/cli/azure/extension#az-extension-list). Se a extensão de alias tiver sido instalada corretamente, estará relacionada na saída do comando.

```azurecli
az extension list --output table --query '[].{Name:name}'
```

```output
Name
------
alias
```


## <a name="keep-the-extension-up-to-date"></a>Manter a extensão atualizada

A extensão do alias está em desenvolvimento ativo, e novas versões são lançadas regularmente. Quando você atualiza a CLI, as novas versões não são instaladas automaticamente. Instale as atualizações para a extensão com [az extension update](/cli/azure/extension#az-extension-update).

```azurecli
az extension update --name alias
```


## <a name="manage-aliases-for-the-azure-cli"></a>Gerenciar aliases para a CLI do Azure

A extensão de alias fornece comandos familiares e convenientes para gerenciar aliases. Para exibir todos os comandos disponíveis e os detalhes de parâmetros, invoque o comando de alias com `--help`.

```azurecli
az alias --help
```


## <a name="create-simple-alias-commands"></a>Criar comandos simples de alias

Uma das utilidades dos aliases é encurtar grupos de comando ou nomes de comando existentes. Por exemplo, você pode encurtar o grupo de comandos `group` para `rg` e o comando `list` para `ls`.

```azurecli
az alias create --name rg --command group
az alias create --name ls --command list
```

Agora, esses aliases recém-definidos podem ser usados nos mesmos lugares que suas definições.

```azurecli
az rg list
az rg ls
az vm ls
```

Não inclua `az` como parte do comando.

Aliases também podem ser atalhos para comandos completos. O exemplo a seguir lista os grupos de recursos disponíveis e suas localizações na saída da tabela:

```azurecli
az alias create --name ls-groups --command "group list --query '[].{Name:name, Location:location}' --output table"
```

Agora, `ls-groups` pode ser executado como qualquer outro comando da CLI.

```azurecli
az ls-groups
```


## <a name="create-an-alias-command-with-arguments"></a>Criar um comando de alias com argumentos

Você também pode adicionar argumentos posicionais para um comando de alias incluindo-os como `{{ arg_name }}` no nome do alias. O espaço em branco entre as chaves é obrigatório.

```azurecli
az alias create --name "alias_name {{ arg1 }} {{ arg2 }} ..." --command "invoke_including_args"
```

O exemplo de alias seguinte mostra como usar argumentos posicionais para obter o endereço IP público de uma VM.

```azurecli
az alias create \
    --name "get-vm-ip {{ resourceGroup }} {{ vmName }}" \
    --command "vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }}
        --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress"
```

Ao executar esse comando, você fornece valores para os argumentos posicionais.

```azurecli
az get-vm-ip MyResourceGroup MyVM
```

Você também pode usar variáveis de ambiente em comandos invocados pelo aliases, as quais são avaliadas em tempo de execução. O exemplo a seguir adiciona o alias `create-rg`, que cria um grupo de recursos em `eastus` e adiciona uma marca `owner`. Essa marca recebe o valor da variável de ambiente local `USER`.

```azurecli
az alias create \
    --name "create-rg {{ groupName }}" \
    --command "group create --name {{ groupName }} --location eastus --tags owner=\$USER"
```

Para registrar as variáveis de ambiente no comando de alias, o sinal de cifrão `$` deve ser precedido de um caractere de escape.


## <a name="process-arguments-using-jinja2-templates"></a>Processar argumentos usando modelos Jinja2

A substituição de argumento na extensão de alias é executada por [Jinja2](http://jinja.pocoo.org/docs/2.10/), e fornece acesso completo aos recursos do mecanismo do modelo Jinja2. Os modelos permitem que você execute ações como extração de dados e substituição em cadeias de caracteres.

Com modelos Jinja2, você pode escrever aliases que aceitam tipos diferentes de argumentos em comparação com o comando subjacente. Por exemplo, você pode criar um alias que usa uma URL de armazenamento. Em seguida, essa URL é analisada para passar os nomes de conta e do contêiner para o comando de armazenamento.

```azurecli
az alias create \
    --name 'storage-ls {{ url }}' \
    --command "storage blob list
        --account-name {{ url.replace('https://', '').split('.')[0] }}
        --container-name {{ url.replace('https://', '').split('/')[1] }}"
```

Para saber mais sobre o mecanismo de modelo Jinja2, confira a [documentação do Jinja2](http://jinja.pocoo.org/docs/2.10/templates/).


## <a name="alias-configuration-file"></a>Arquivo de configuração de alias

Outra maneira de criar e modificar aliases é alterando o arquivo de configuração de alias. As definições de comando do alias são gravadas em um arquivo de configuração localizado em `$AZURE_USER_CONFIG/alias`. O valor padrão de `AZURE_USER_CONFIG` é `$HOME/.azure` no Linux e macOS, e `%USERPROFILE%\.azure` no Windows. O arquivo de configuração do alias é gravado no formato de arquivo de configuração INI. O formato para comandos de alias é:

```ini
[alias_name]
command = invoked_commands
```

Para aliases que contêm argumentos posicionais, o formato para os comandos de alias é:

```ini
[alias_name {{ arg1 }} {{ arg2 }} ...]
command = invoked_commands_including_args
```


## <a name="create-an-alias-command-with-arguments-via-the-alias-configuration-file"></a>Criar um comando de alias com argumentos por meio do arquivo de configuração do alias

Abaixo há um arquivo de configuração de alias que contém um comando de alias de exemplo com argumentos, o qual obtém o endereço IP público para uma VM. Verifique se o comando invocado está em uma única linha e contém os mesmos argumentos definidos no alias.

```ini
[get-vm-ip {{ resourceGroup }} {{ vmName }}]
command = vm list-ip-addresses --resource-group {{ resourceGroup }} --name {{ vmName }} --query [0].virtualMachine.network.publicIpAddresses[0].ipAddress
```


## <a name="uninstall-the-alias-extension"></a>Desinstalar a extensão do alias

Para desinstalar a extensão, use o comando [az extension remove](/cli/azure/extension#az-extension-remove).

```azurecli
az extension remove --name alias
```

Se você desinstalou devido a um bug ou outros problemas com a extensão, [arquive um problema do GitHub](https://github.com/Azure/azure-cli-extensions/issues) para que possamos fornecer uma correção.
