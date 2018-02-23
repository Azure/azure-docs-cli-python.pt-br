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
ms.openlocfilehash: a5d629675b468421e3abee41b9c8bffd7e96e5b0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="cc73e-103">Formatos de saída dos comandos da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="cc73e-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="cc73e-104">A CLI do Azure 2.0 usa json como opção de saída padrão, mas oferece várias maneiras de formatar a saída de qualquer comando.</span><span class="sxs-lookup"><span data-stu-id="cc73e-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="cc73e-105">Use o parâmetro `--output` (ou `--out` ou `-o`) para formatar a saída do comando em um dos tipos de saída indicados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="cc73e-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table.</span></span>

<span data-ttu-id="cc73e-106">--output</span><span class="sxs-lookup"><span data-stu-id="cc73e-106">--output</span></span> | <span data-ttu-id="cc73e-107">DESCRIÇÃO</span><span class="sxs-lookup"><span data-stu-id="cc73e-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="cc73e-108">cadeia de caracteres json.</span><span class="sxs-lookup"><span data-stu-id="cc73e-108">json string.</span></span> <span data-ttu-id="cc73e-109">O padrão é `json`.</span><span class="sxs-lookup"><span data-stu-id="cc73e-109">`json` is the default.</span></span>
`jsonc`  | <span data-ttu-id="cc73e-110">cadeia de caracteres json colorida.</span><span class="sxs-lookup"><span data-stu-id="cc73e-110">colorized json string.</span></span>
`table`  | <span data-ttu-id="cc73e-111">tabela com cabeçalhos de coluna.</span><span class="sxs-lookup"><span data-stu-id="cc73e-111">table with column headings.</span></span>
`tsv`    | <span data-ttu-id="cc73e-112">valores separados por tabulações.</span><span class="sxs-lookup"><span data-stu-id="cc73e-112">tab-separated values.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a><span data-ttu-id="cc73e-113">Usar a opção de json</span><span class="sxs-lookup"><span data-stu-id="cc73e-113">Using the json option</span></span>

<span data-ttu-id="cc73e-114">O exemplo a seguir exibe a lista de máquinas virtuais em suas assinaturas no formato json padrão.</span><span class="sxs-lookup"><span data-stu-id="cc73e-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="cc73e-115">Os resultados estão nesse formulário (mostrando apenas o resultado parcial para fins de brevidade).</span><span class="sxs-lookup"><span data-stu-id="cc73e-115">The results are in this form (only showing partial output for sake of brevity).</span></span>

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

## <a name="using-the-table-option"></a><span data-ttu-id="cc73e-116">Usar a opção de tabela</span><span class="sxs-lookup"><span data-stu-id="cc73e-116">Using the table option</span></span>

<span data-ttu-id="cc73e-117">A opção de tabela fornece uma forma fácil de ler um conjunto de saída, mas observe que objetos aninhados não são incluídos na saída com a simples `--output table`, ao contrário do exemplo do .json acima.</span><span class="sxs-lookup"><span data-stu-id="cc73e-117">The table option provides an easy to read set of output, but note that nested objects are not included in the output with the simple `--output table`, unlike the preceding .json example.</span></span>  <span data-ttu-id="cc73e-118">Usando o mesmo exemplo com o formato de saída 'table' fornece uma lista auxiliar de valores de propriedade mais comuns.</span><span class="sxs-lookup"><span data-stu-id="cc73e-118">Using the same example with 'table' output format provides a curated list of most common property values.</span></span>

```azurecli-interactive
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

<span data-ttu-id="cc73e-119">Você pode usar o parâmetro `--query` para personalizar as propriedades e as colunas que você deseja mostrar na saída da lista.</span><span class="sxs-lookup"><span data-stu-id="cc73e-119">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="cc73e-120">O exemplo a seguir mostra como selecionar o Nome da VM e o Nome do Grupo de Recursos no comando `list`.</span><span class="sxs-lookup"><span data-stu-id="cc73e-120">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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

## <a name="using-the-tsv-option"></a><span data-ttu-id="cc73e-121">Usar a opção de tsv</span><span class="sxs-lookup"><span data-stu-id="cc73e-121">Using the tsv option</span></span>

<span data-ttu-id="cc73e-122">O formato de saída 'tsv' retorna uma saída simples baseada em texto e separada por tabulações sem títulos e traços.</span><span class="sxs-lookup"><span data-stu-id="cc73e-122">'tsv' output format returns a simple text-based and tab-separated output with no headings and dashes.</span></span> <span data-ttu-id="cc73e-123">Esse formato facilita o consumo da saída em outros comandos e ferramentas que precisam processar o texto de alguma maneira.</span><span class="sxs-lookup"><span data-stu-id="cc73e-123">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="cc73e-124">Se o exemplo anterior com a opção `tsv` for usado, gerará o resultado separado por tabulações.</span><span class="sxs-lookup"><span data-stu-id="cc73e-124">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="cc73e-125">A exemplo a seguir mostra como a saída `tsv` pode ser transferida para comandos como `grep` e `cut` para analisar ainda mais os valores específicos da saída `list`.</span><span class="sxs-lookup"><span data-stu-id="cc73e-125">The next example shows how the `tsv` output can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="cc73e-126">O comando `grep` seleciona apenas os itens que têm o texto "RGD" e, em seguida, o comando `cut` seleciona apenas o oitavo valor do campo (separado por guias) para mostrar na saída.</span><span class="sxs-lookup"><span data-stu-id="cc73e-126">The `grep` command selects only items that have text "RGD" in them and then the `cut` command selects only the eighth field (separated by tabs) value to show in the output.</span></span>

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a><span data-ttu-id="cc73e-127">Configurar o formato de saída padrão</span><span class="sxs-lookup"><span data-stu-id="cc73e-127">Setting the default output format</span></span>

<span data-ttu-id="cc73e-128">Você pode usar o comando `az configure` para configurar seu ambiente ou estabelecer as preferências como as configurações padrão para formatos de saída.</span><span class="sxs-lookup"><span data-stu-id="cc73e-128">You can use the `az configure` command to set up your environment or establish preferences such as default settings for output formats.</span></span> <span data-ttu-id="cc73e-129">Para uso comum, o padrão de formato de saída mais fácil é o formato de "tabela" - escolha **3** quando solicitado a fornecer opções de formato de saída.</span><span class="sxs-lookup"><span data-stu-id="cc73e-129">For common use, the easiest output format default is the "table" format - select **3** when prompted for output format choices.</span></span>

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]:
```
