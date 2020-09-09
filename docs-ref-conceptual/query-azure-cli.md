---
title: Resultados de comando de consulta com a CLI do Azure
description: Saiba como realizar consultas JMESPath na saída dos comandos da CLI do Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 17d62f7c6c5b819e34d6fce16caa0ded6faa53f0
ms.sourcegitcommit: 2da241715d25407ed22c1065c0c793acfd865996
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "89563120"
---
# <a name="query-azure-cli-command-output"></a>Consultar a saída do comando da CLI do Azure

A CLI do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados dos comandos. JMESPath é uma linguagem de consulta do JSON, permitindo que você selecione e modifique os dados na saída da CLI. As consultas são executadas na saída do JSON antes de qualquer formatação da exibição.

O argumento `--query` tem suporte de todos os comandos na CLI do Azure. Este artigo aborda como usar os recursos do JMESPath com uma série de exemplos pequenos e simples.

## <a name="dictionary-and-list-cli-results"></a>Dicionário e lista dos resultados da CLI

Mesmo ao usar um formato de saída diferente do JSON, os resultados do comando da CLI são tratados primeiro como JSON para consultas. Os resultados da CLI são uma matriz JSON ou um dicionário. Matrizes são sequências de objetos que podem ser indexados, e dicionários são objetos não ordenados acessados com chaves. Os comandos que _poderiam_ retornar mais de um objeto retornam uma matriz, e os comandos que _sempre_ retornam _apenas_ um objeto retornam um dicionário.

## <a name="get-properties-in-a-dictionary"></a>Obter propriedades em um dicionário

Trabalhando com os resultados do dicionário, você pode acessar as propriedades no nível superior com apenas a chave. O caractere `.` (__subexpressão__) é usado para acessar as propriedades dos dicionários aninhados. Antes de apresentar as consultas, examine a saída não modificada do comando `az vm show`:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

O comando produzirá um dicionário. Parte do conteúdo foi omitida.

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

O comando a seguir obtém as chaves SSH públicas autorizadas para conectar a VM adicionando uma consulta:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

## <a name="get-a-single-value"></a>Obter um valor único

Um caso comum é precisar obter somente _um_ valor de um comando da CLI, como uma ID do recurso do Azure, um nome de recurso, um nome de usuário ou uma senha. Nesse caso, muitas vezes você também quer armazenar o valor em uma variável de ambiente local. Para obter uma propriedade única, primeiro, verifique se você está recebendo somente uma propriedade da consulta. Ao modificar o último exemplo para obter somente o nome de usuário do administrador:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

Parece um valor único válido, mas observe que os caracteres `"` são retornados como parte da saída. Isso indica que o objeto é uma cadeia de caracteres JSON. É importante observar que ao atribuir esse valor diretamente à variável de ambiente como saída do comando, as aspas podem __não__ ser interpretadas pelo shell:

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

Certamente, isso não é desejado. Nesse caso, você quer usar um formato de saída que não inclua os valores retornados com as informações de tipo. A melhor opção de saída oferecida pela CLI para este fim é `tsv`, valores separados por tabulações. Em especial, ao recuperar um valor que é somente um valor único (e não um dicionário ou uma lista), garante-se que a saída `tsv` não tenha aspas.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

Para saber mais sobre o formato de saída `tsv`, confira [Formatos de saída – Formato de saída TSV](format-output-azure-cli.md#tsv-output-format)

## <a name="get-multiple-values"></a>Obter vários valores

Para obter mais de uma propriedade, coloque as expressões entre colchetes `[ ]` (uma __lista de seleção múltipla__), como uma lista separada por vírgulas. Para obter o nome da VM, o usuário administrador e a chave SSH juntos, use o comando:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

Esses valores são listados na matriz de resultados na ordem em que foram fornecidos na consulta. Como o resultado é uma matriz, não há nenhuma chave associada a ele.

## <a name="rename-properties-in-a-query"></a>Renomear as propriedades em uma consulta

Para obter um dicionário, em vez de uma matriz, ao consultar diversos valores, use o operador `{ }` (__hash de seleção múltipla__).
O formato de um hash de seleção múltipla é `{displayName:JMESPathExpression, ...}`.
`displayName` será a cadeia de caracteres mostrada na saída e `JMESPathExpression` é a expressão do JMESPath a avaliar. Modificando o exemplo da seção anterior alterando a lista de seleção múltipla para um hash:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a>Obter propriedades em uma matriz

Uma matriz não tem nenhuma propriedade, mas pode ser indexada. Esse recurso é mostrado no último exemplo com a expressão `publicKeys[0]`, que obtém o primeiro elemento da matriz `publicKeys`. Não há nenhuma garantia de que a CLI de saída será ordenada, portanto, evite usar a indexação, a menos que tenha certeza da ordem ou não se importe com o elemento obtido. Para acessar as propriedades dos elementos em uma matriz, execute uma das duas operações: _nivelamento_ e _filtragem_. Esta seção aborda como nivelar uma matriz.

O nivelamento de uma matriz é feito com o operador `[]` do JMESPath. Todas as expressões após o operador `[]` são aplicadas em cada elemento na matriz atual.
Se `[]` aparecer no início da consulta, ele nivelará o resultado do comando da CLI. Os resultados de `az vm list` podem ser examinados com esse recurso.
Para obter o nome, o SO e o nome do administrador de cada VM em um grupo de recursos:

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

Quando combinados com o formato de saída `--output table`, os nomes de colunas correspondem ao valor `displayKey` do hash de seleção múltipla:

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> Algumas chaves são filtradas e não são impressas na exibição da tabela. Essas chaves são `id`, `type` e `etag`. Para ver esses valores, você pode alterar o nome da chave em um hash de seleção múltipla.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

Qualquer matriz pode ser nivelada, não apenas o resultado de alto nível retornado pelo comando. Na última seção, a expressão `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` foi usada para obter a chave SSH pública para entrar. Para obter _cada_ chave SSH pública, a expressão pode ser escrita como `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.
Esta expressão de consulta nivela a matriz `osProfile.linuxConfiguration.ssh.publicKeys` e executa a expressão `keyData` em cada elemento:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a>Filtrar matrizes

A outra operação usada para obter dados de uma matriz é a _filtragem_. A filtragem é feita com o operador `[?...]` do JMESPath.
Esse operador usa um predicado como conteúdo. Um predicado é qualquer instrução que pode ser avaliada como `true` ou `false`. As expressões em que o predicado é avaliado como `true` são incluídas na saída.

JMESPath oferece a comparação padrão e os operadores lógicos. Eles incluem `<`, `<=`, `>`, `>=`, `==` e `!=`.
JMESPath também dá suporte às operações lógicas e (`&&`) ou (`||`), e não (`!`). Expressões podem ser agrupadas entre parênteses, permitindo expressões de predicado mais complexas. Para obter mais detalhes sobre predicados e operações lógicas, confira a [especificação do JMESPath](http://jmespath.org/specification.html).

Na última seção, nivelamos uma matriz para obter a lista completa de todas as VMs em um grupo de recursos. Usando filtros, essa saída pode ser restrita apenas às VMs do Linux:

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> No JMESPath, as cadeias de caracteres sempre ficam entre aspas simples (`'`). Se você usar aspas duplas como parte de uma cadeia de caracteres em um predicado de filtro, obterá uma saída vazia.

O JMESPath também tem funções internas que podem ajudar na filtragem. Uma dessas funções é `contains(string, substring)`, que verifica se uma cadeia de caracteres contém uma subcadeia. As expressões são avaliadas antes de chamar a função, portanto, o primeiro argumento pode ser uma expressão completa do JMESPath. O exemplo a seguir localiza todas as VMs usando o armazenamento SSD para seu disco do SO:

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

Essa consulta é um pouco longa. A chave `storageProfile.osDisk.managedDisk.storageAccountType` é mencionada duas vezes e rechaveada na saída. Uma maneira de reduzi-la é aplicar o filtro depois de nivelar e selecionar os dados.

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

Para matrizes grandes, pode ser mais rápido aplicar o filtro antes de selecionar os dados.

Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.

## <a name="change-output"></a>Alterar a saída

As funções do JMESPath também têm outra finalidade, que é operar nos resultados de uma consulta. Qualquer função que retorna um valor não booliano altera o resultado de uma expressão.
Por exemplo, você pode classificar os dados por um valor de propriedade com `sort_by(array, &sort_expression)`. O JMESPath usa um operador especial, `&`, para as expressões que devem ser avaliadas posteriormente como parte de uma função. O exemplo a seguir mostra como classificar uma lista de VMs pelo tamanho de disco do SO:

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

Confira a [Especificação do JMESPath - Funções Internas](http://jmespath.org/specification.html#built-in-functions) para obter a lista completa de funções.

## <a name="experiment-with-queries-interactively"></a>Experimentar consultas interativamente

Para começar a experimentar o JMESPath, o pacote [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) do Python oferece um ambiente interativo para trabalhar com as consultas. Os dados são transferidos como entrada e as consultas são gravadas e executadas no editor.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
