---
title: "Formatos de saída da CLI do Azure 2.0"
description: "Use --output para formatar a saída dos comandos da CLI do Azure 2.0 para tabelas, listas ou json."
keywords: "CLI do Azure 2.0, saída, formato, tabela, lista, json, Linux, Mac, Windows, OS X"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 74bdb727-481d-45f7-a44e-15d18dc55483
ms.openlocfilehash: de37b1ad6aa55c9ac73b5b6b89d9507c86cc1245
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: pt-BR
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formatos de saída dos comandos da CLI do Azure 2.0

A CLI do Azure 2.0 usa json como opção de saída padrão, mas oferece várias maneiras de formatar a saída de qualquer comando.  Use o parâmetro `--output` (ou `--out` ou `-o`) para formatar a saída do comando em um dos tipos de saída indicados na tabela a seguir. 

--output | Descrição
---------|-------------------------------
`json`   | cadeia de caracteres json. O padrão é `json`.
`jsonc`  | cadeia de caracteres json colorida.
`table`  | tabela com cabeçalhos de coluna.
`tsv`    | valores separados por tabulações.

## <a name="using-the-json-option"></a>Usar a opção de json

O exemplo a seguir exibe a lista de máquinas virtuais em suas assinaturas no formato json padrão.

```azurecli
az vm list --output json
```

Os resultados estão nesse formulário (mostrando apenas o resultado parcial para fins de brevidade).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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
 
## <a name="using-the-table-option"></a>Usar a opção de tabela

A opção de tabela fornece uma forma fácil de ler um conjunto de saída, mas observe que objetos aninhados não são incluídos na saída com a simples `--output table`, ao contrário do exemplo do .json acima.  Usando o mesmo exemplo com o formato de saída 'table' fornece uma lista auxiliar de valores de propriedade mais comuns.

```azurecli
az vm list --out table
```

```
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
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
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

## <a name="using-the-tsv-option"></a>Usar a opção de tsv

O formato de saída 'tsv' retorna uma saída simples baseada em texto e separada por tabulações sem títulos e traços. Esse formato facilita o consumo da saída em outros comandos e ferramentas que precisam processar o texto de alguma maneira. Se o exemplo anterior com a opção `tsv` for usado, gerará o resultado separado por tabulações.

```azurecli
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

A exemplo a seguir mostra como a saída `tsv` pode ser transferida para comandos como `grep` e `cut` para analisar ainda mais os valores específicos da saída `list`. O comando `grep` seleciona apenas os itens que têm o texto "RGD" e, em seguida, o comando `cut` seleciona apenas o oitavo valor do campo (separado por guias) para mostrar na saída.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>Configurar o formato de saída padrão

Você pode usar o comando `az configure` para configurar seu ambiente ou estabelecer as preferências como as configurações padrão para formatos de saída. Para uso comum, o padrão de formato de saída mais fácil é o formato de "tabela" - escolha **3** quando solicitado a fornecer opções de formato de saída. 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```