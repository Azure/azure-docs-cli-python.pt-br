---
title: "Formatos de saída da CLI do Azure 2.0"
description: "Saiba como formatar a saída dos comandos da CLI do Azure 2.0 para tabelas, listas ou json."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: ec96d1cb21b32cd982dbec5e4bf38110f8686c25
ms.sourcegitcommit: f82774a6f92598c41da9956284f563757f402774
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/19/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formatos de saída dos comandos da CLI do Azure 2.0

A CLI do Azure 2.0 usa json como opção de saída padrão, mas oferece várias maneiras de formatar a saída de qualquer comando.  Use o parâmetro `--output` (ou `--out` ou `-o`) para formatar a saída do comando em um dos tipos de saída indicados na tabela a seguir:

--output | DESCRIÇÃO
---------|-------------------------------
`json`   | cadeia de caracteres JSON. Esta é a configuração padrão.
`jsonc`  | JSON colorido.
`table`  | A tabela ASCII com as chaves como títulos de coluna.
`tsv`    | Valores separados por tabulação, sem chaves

## <a name="json-output-format"></a>Formato da saída JSON

O exemplo a seguir exibe a lista de máquinas virtuais em suas assinaturas no formato json padrão.

```azurecli
az vm list --output json
```

A saída a seguir tem alguns campos omitidos para fins de brevidade e informações de identificação substituídas.

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="table-output-format"></a>Formato de saída da tabela

O formato de saída `table` fornece saída sem formatação como linhas e colunas de dados agrupados, tornando mais fácil de ler e examinar. Objetos aninhados não são incluídos na saída da tabela, mas ainda podem ser filtrados como parte de uma consulta. Alguns campos também são omitidos dos dados da tabela, por isso, esse formato é melhor quando você deseja obter uma visão geral dos dados rápida e que possa ser pesquisada manualmente.

```azurecli
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```
Você pode usar o parâmetro `--query` para personalizar as propriedades e as colunas que você deseja mostrar na saída da lista. O exemplo a seguir mostra como selecionar o Nome da VM e o Nome do Grupo de Recursos no comando `list`.

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> Algumas chaves são filtradas e não são impressas na exibição da tabela. Elas são: `id`, `type` e `etag`. Se você precisar ver isso na saída, poderá usar o recurso de recriação de chave JMESPath para alterar o nome da chave e evitar a filtragem.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Para obter mais informações sobre como usar consultas para filtrar dados, confira [Usar as consultas do JMESPath com a CLI 2.0 do Azure](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>O formato de saída TSV

O formato de saída `tsv` retorna valores separados por tabulação e nova linha sem formatação, chaves ou outros símbolos adicionais. Esse formato facilita o consumo da saída em outros comandos e ferramentas que precisam processar o texto de alguma maneira. Como o formato `table`, a opção de saída `tsv` não imprime objetos aninhados.

Se o exemplo anterior com a opção `tsv` for usado, gerará o resultado separado por tabulações.

```azurecli
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

O exemplo a seguir mostra como a saída `tsv` pode ser transportada para outros comandos em sistemas UNIX para extrair dados mais específicos. O comando `grep` seleciona os itens que têm o texto "RGD" e, em seguida, o comando `cut` seleciona o oitavo campo (separado por tabulações) para mostrar o nome da VM na saída.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

Para fins de processamento de campos separados por tabulação, os valores estão na mesma ordem em que aparecem no objeto JSON impresso. Essa ordem garante a consistência entre as execuções do comando.

## <a name="set-the-default-output-format"></a>Definir o formato de saída padrão

Use o comando interativo `az configure` para configurar seu ambiente e estabelecer as configurações padrão para formatos de saída. O formato de saída padrão é `json`. 

```azurecli
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

Para saber mais sobre como configurar seu ambiente, confira [Configuração da CLI 2.0 do Azure](/cli/azure/azure-cli-configuration).
