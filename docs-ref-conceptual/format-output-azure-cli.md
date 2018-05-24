---
title: Formatos de saída da CLI do Azure 2.0
description: Saiba como formatar a saída dos comandos da CLI do Azure 2.0 para tabelas, listas ou json.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 016465080e95af3ab0650146e955dd8cffc569e8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="3be52-103">Formatos de saída dos comandos da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="3be52-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="3be52-104">A CLI do Azure 2.0 usa json como opção de saída padrão, mas oferece várias maneiras de formatar a saída de qualquer comando.</span><span class="sxs-lookup"><span data-stu-id="3be52-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="3be52-105">Use o parâmetro `--output` (ou `--out` ou `-o`) para formatar a saída do comando em um dos tipos de saída indicados na tabela a seguir:</span><span class="sxs-lookup"><span data-stu-id="3be52-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="3be52-106">--output</span><span class="sxs-lookup"><span data-stu-id="3be52-106">--output</span></span> | <span data-ttu-id="3be52-107">DESCRIÇÃO</span><span class="sxs-lookup"><span data-stu-id="3be52-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="3be52-108">cadeia de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="3be52-108">JSON string.</span></span> <span data-ttu-id="3be52-109">Esta é a configuração padrão.</span><span class="sxs-lookup"><span data-stu-id="3be52-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="3be52-110">JSON colorido.</span><span class="sxs-lookup"><span data-stu-id="3be52-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="3be52-111">A tabela ASCII com as chaves como títulos de coluna.</span><span class="sxs-lookup"><span data-stu-id="3be52-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="3be52-112">Valores separados por tabulação, sem chaves</span><span class="sxs-lookup"><span data-stu-id="3be52-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="3be52-113">Formato da saída JSON</span><span class="sxs-lookup"><span data-stu-id="3be52-113">JSON output format</span></span>

<span data-ttu-id="3be52-114">O exemplo a seguir exibe a lista de máquinas virtuais em suas assinaturas no formato json padrão.</span><span class="sxs-lookup"><span data-stu-id="3be52-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="3be52-115">A saída a seguir tem alguns campos omitidos para fins de brevidade e informações de identificação substituídas.</span><span class="sxs-lookup"><span data-stu-id="3be52-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="3be52-116">Formato de saída da tabela</span><span class="sxs-lookup"><span data-stu-id="3be52-116">Table output format</span></span>

<span data-ttu-id="3be52-117">O formato de saída `table` fornece saída sem formatação como linhas e colunas de dados agrupados, tornando mais fácil de ler e examinar.</span><span class="sxs-lookup"><span data-stu-id="3be52-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="3be52-118">Objetos aninhados não são incluídos na saída da tabela, mas ainda podem ser filtrados como parte de uma consulta.</span><span class="sxs-lookup"><span data-stu-id="3be52-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="3be52-119">Alguns campos também são omitidos dos dados da tabela, por isso, esse formato é melhor quando você deseja obter uma visão geral dos dados rápida e que possa ser pesquisada manualmente.</span><span class="sxs-lookup"><span data-stu-id="3be52-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

```azurecli-interactive
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

<span data-ttu-id="3be52-120">Você pode usar o parâmetro `--query` para personalizar as propriedades e as colunas que você deseja mostrar na saída da lista.</span><span class="sxs-lookup"><span data-stu-id="3be52-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="3be52-121">O exemplo a seguir mostra como selecionar o Nome da VM e o Nome do Grupo de Recursos no comando `list`.</span><span class="sxs-lookup"><span data-stu-id="3be52-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> <span data-ttu-id="3be52-122">Algumas chaves são filtradas e não são impressas na exibição da tabela.</span><span class="sxs-lookup"><span data-stu-id="3be52-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="3be52-123">Elas são: `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="3be52-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="3be52-124">Se você precisar ver isso na saída, poderá usar o recurso de recriação de chave JMESPath para alterar o nome da chave e evitar a filtragem.</span><span class="sxs-lookup"><span data-stu-id="3be52-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="3be52-125">Para obter mais informações sobre como usar consultas para filtrar dados, confira [Usar as consultas do JMESPath com a CLI 2.0 do Azure](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="3be52-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="3be52-126">O formato de saída TSV</span><span class="sxs-lookup"><span data-stu-id="3be52-126">TSV output format</span></span>

<span data-ttu-id="3be52-127">O formato de saída `tsv` retorna valores separados por tabulação e nova linha sem formatação, chaves ou outros símbolos adicionais.</span><span class="sxs-lookup"><span data-stu-id="3be52-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="3be52-128">Esse formato facilita o consumo da saída em outros comandos e ferramentas que precisam processar o texto de alguma maneira.</span><span class="sxs-lookup"><span data-stu-id="3be52-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="3be52-129">Como o formato `table`, a opção de saída `tsv` não imprime objetos aninhados.</span><span class="sxs-lookup"><span data-stu-id="3be52-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="3be52-130">Se o exemplo anterior com a opção `tsv` for usado, gerará o resultado separado por tabulações.</span><span class="sxs-lookup"><span data-stu-id="3be52-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="3be52-131">O exemplo a seguir mostra como a saída `tsv` pode ser transportada para outros comandos em sistemas UNIX para extrair dados mais específicos.</span><span class="sxs-lookup"><span data-stu-id="3be52-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="3be52-132">O comando `grep` seleciona os itens que têm o texto "RGD" e, em seguida, o comando `cut` seleciona o oitavo campo (separado por tabulações) para mostrar o nome da VM na saída.</span><span class="sxs-lookup"><span data-stu-id="3be52-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="3be52-133">Para fins de processamento de campos separados por tabulação, os valores estão na mesma ordem em que aparecem no objeto JSON impresso.</span><span class="sxs-lookup"><span data-stu-id="3be52-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="3be52-134">Essa ordem garante a consistência entre as execuções do comando.</span><span class="sxs-lookup"><span data-stu-id="3be52-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="3be52-135">Definir o formato de saída padrão</span><span class="sxs-lookup"><span data-stu-id="3be52-135">Set the default output format</span></span>

<span data-ttu-id="3be52-136">Use o comando interativo `az configure` para configurar seu ambiente e estabelecer as configurações padrão para formatos de saída.</span><span class="sxs-lookup"><span data-stu-id="3be52-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="3be52-137">O formato de saída padrão é `json`.</span><span class="sxs-lookup"><span data-stu-id="3be52-137">The default output format is `json`.</span></span> 

```azurecli-interactive
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

<span data-ttu-id="3be52-138">Para saber mais sobre como configurar seu ambiente, confira [Configuração da CLI 2.0 do Azure](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="3be52-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>