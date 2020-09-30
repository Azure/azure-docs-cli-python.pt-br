---
title: Formatos de saída da CLI do Azure
description: Saiba como formatar a saída dos comandos da CLI do Azure para tabelas, listas ou json.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: fd505aa70b847595d1b3dd02b6d88b60ca95db4c
ms.sourcegitcommit: 5d29362589078b66d15f5cd494fe903a5195658d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "91225857"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="2daa3-103">Formatos de saída dos comandos da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="2daa3-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="2daa3-104">A CLI do Azure usa JSON como formato de saída padrão, mas oferece outros formatos.</span><span class="sxs-lookup"><span data-stu-id="2daa3-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="2daa3-105">Use o parâmetro `--output` (`--out` ou `-o`) para formatar a saída da CLI.</span><span class="sxs-lookup"><span data-stu-id="2daa3-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="2daa3-106">Os valores e tipos de argumentos de saída são:</span><span class="sxs-lookup"><span data-stu-id="2daa3-106">The argument values and types of output are:</span></span>

<span data-ttu-id="2daa3-107">--output</span><span class="sxs-lookup"><span data-stu-id="2daa3-107">--output</span></span> | <span data-ttu-id="2daa3-108">DESCRIÇÃO</span><span class="sxs-lookup"><span data-stu-id="2daa3-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="2daa3-109">cadeia de caracteres JSON.</span><span class="sxs-lookup"><span data-stu-id="2daa3-109">JSON string.</span></span> <span data-ttu-id="2daa3-110">Essa configuração é a padrão</span><span class="sxs-lookup"><span data-stu-id="2daa3-110">This setting is the default</span></span>
`jsonc`  | <span data-ttu-id="2daa3-111">JSON colorido</span><span class="sxs-lookup"><span data-stu-id="2daa3-111">Colorized JSON</span></span>
`yaml`   | <span data-ttu-id="2daa3-112">YAML, uma alternativa ao JSON legível por computador</span><span class="sxs-lookup"><span data-stu-id="2daa3-112">YAML, a machine-readable alternative to JSON</span></span>
`table`  | <span data-ttu-id="2daa3-113">A tabela ASCII com chaves como títulos de colunas</span><span class="sxs-lookup"><span data-stu-id="2daa3-113">ASCII table with keys as column headings</span></span>
`tsv`    | <span data-ttu-id="2daa3-114">Valores separados por tabulação, sem chaves</span><span class="sxs-lookup"><span data-stu-id="2daa3-114">Tab-separated values, with no keys</span></span>
`none`   | <span data-ttu-id="2daa3-115">Nenhuma saída diferente de erros e avisos</span><span class="sxs-lookup"><span data-stu-id="2daa3-115">No output other than errors and warnings</span></span>

## <a name="json-output-format"></a><span data-ttu-id="2daa3-116">Formato da saída JSON</span><span class="sxs-lookup"><span data-stu-id="2daa3-116">JSON output format</span></span>

<span data-ttu-id="2daa3-117">O exemplo a seguir exibe a lista de máquinas virtuais em suas assinaturas no formato JSON padrão.</span><span class="sxs-lookup"><span data-stu-id="2daa3-117">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="2daa3-118">A saída a seguir tem alguns campos omitidos para fins de brevidade e informações de identificação substituídas.</span><span class="sxs-lookup"><span data-stu-id="2daa3-118">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="2daa3-119">Formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="2daa3-119">YAML output format</span></span>

<span data-ttu-id="2daa3-120">O formato `yaml` imprime a saída como [YAML](http://yaml.org/), um formato de serialização de dados de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="2daa3-120">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="2daa3-121">YAML tende a ser mais fácil de ler que o JSON e facilmente mapeia para esse formato.</span><span class="sxs-lookup"><span data-stu-id="2daa3-121">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="2daa3-122">Alguns aplicativos e comandos da CLI usam YAML como entrada de configuração, em vez de JSON.</span><span class="sxs-lookup"><span data-stu-id="2daa3-122">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="2daa3-123">A saída a seguir tem alguns campos omitidos para fins de brevidade e informações de identificação substituídas.</span><span class="sxs-lookup"><span data-stu-id="2daa3-123">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a><span data-ttu-id="2daa3-124">Formato de saída da tabela</span><span class="sxs-lookup"><span data-stu-id="2daa3-124">Table output format</span></span>

<span data-ttu-id="2daa3-125">O formato `table` imprime a saída como uma tabela ASCII, facilitando a leitura e a análise.</span><span class="sxs-lookup"><span data-stu-id="2daa3-125">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="2daa3-126">Objetos aninhados não são incluídos na saída da tabela, mas ainda podem ser filtrados como parte de uma consulta.</span><span class="sxs-lookup"><span data-stu-id="2daa3-126">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="2daa3-127">Alguns campos não estão incluídos na tabela, por isso, esse formato é o ideal quando seu objetivo é ter uma visão geral rápida dos dados e que possa ser pesquisada manualmente.</span><span class="sxs-lookup"><span data-stu-id="2daa3-127">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="2daa3-128">Você pode usar o parâmetro `--query` para personalizar as propriedades e as colunas que você deseja mostrar na saída da lista.</span><span class="sxs-lookup"><span data-stu-id="2daa3-128">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="2daa3-129">O exemplo a seguir mostra como selecionar o Nome da VM e o Nome do Grupo de Recursos no comando `list`.</span><span class="sxs-lookup"><span data-stu-id="2daa3-129">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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
> <span data-ttu-id="2daa3-130">Algumas chaves não são impressas no modo de exibição de tabela, por padrão.</span><span class="sxs-lookup"><span data-stu-id="2daa3-130">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="2daa3-131">Elas são: `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="2daa3-131">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="2daa3-132">Se você precisar ver isso na saída, poderá usar o recurso de recriação de chave JMESPath para alterar o nome da chave e evitar a filtragem.</span><span class="sxs-lookup"><span data-stu-id="2daa3-132">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="2daa3-133">Para obter mais informações sobre como usar consultas para filtrar dados, confira [Usar as consultas JMESPath com a CLI do Azure](./query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="2daa3-133">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](./query-azure-cli.md).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="2daa3-134">O formato de saída TSV</span><span class="sxs-lookup"><span data-stu-id="2daa3-134">TSV output format</span></span>

<span data-ttu-id="2daa3-135">O formato de saída `tsv` retorna valores separados por tabulação e nova linha sem formatação, chaves ou outros símbolos adicionais.</span><span class="sxs-lookup"><span data-stu-id="2daa3-135">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="2daa3-136">Esse formato facilita o consumo da saída em outros comandos e ferramentas que precisam processar o texto de alguma maneira.</span><span class="sxs-lookup"><span data-stu-id="2daa3-136">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="2daa3-137">Como o formato `table`, `tsv` não imprime objetos aninhados.</span><span class="sxs-lookup"><span data-stu-id="2daa3-137">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="2daa3-138">Se o exemplo anterior com a opção `tsv` for usado, gerará o resultado separado por tabulações.</span><span class="sxs-lookup"><span data-stu-id="2daa3-138">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="2daa3-139">Uma restrição do formato de saída TSV é que não há uma garantia de ordem na saída.</span><span class="sxs-lookup"><span data-stu-id="2daa3-139">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="2daa3-140">A CLI realiza todos os esforços para preservar a ordem classificando alfabeticamente as chaves na resposta JSON e, em seguida, imprimindo os valores em ordem para a saída TSV.</span><span class="sxs-lookup"><span data-stu-id="2daa3-140">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="2daa3-141">No entanto, isso não é uma garantia de que a ordem sempre será idêntica, pois o formato de resposta do serviço do Azure pode ser alterado.</span><span class="sxs-lookup"><span data-stu-id="2daa3-141">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="2daa3-142">Para impor uma ordem consistente, é necessário usar o parâmetro `--query` e o formato de [lista de multisseleção](query-azure-cli.md#get-multiple-values).</span><span class="sxs-lookup"><span data-stu-id="2daa3-142">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="2daa3-143">Quando um comando de CLI retorna um único dicionário JSON, use o formato geral `[key1, key2, ..., keyN]` para forçar uma ordem de chave.</span><span class="sxs-lookup"><span data-stu-id="2daa3-143">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="2daa3-144">Para comandos de CLI que retornam uma matriz, use o formato geral `[].[key1, key2, ..., keyN]` para ordenar os valores de coluna.</span><span class="sxs-lookup"><span data-stu-id="2daa3-144">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="2daa3-145">Por exemplo, para ordenar as informações exibidas acima da ID, do local, do grupo de recursos e do nome da VM:</span><span class="sxs-lookup"><span data-stu-id="2daa3-145">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

<span data-ttu-id="2daa3-146">O exemplo a seguir mostra como a saída `tsv` pode ser transportada para outros comandos no bash.</span><span class="sxs-lookup"><span data-stu-id="2daa3-146">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="2daa3-147">A consulta é usada para filtrar a saída e forçar o ordenamento, `grep` seleciona itens com o texto "RGD" e o comando `cut` seleciona o quarto campo para mostrar o nome da VM na saída.</span><span class="sxs-lookup"><span data-stu-id="2daa3-147">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="2daa3-148">Definir o formato de saída padrão</span><span class="sxs-lookup"><span data-stu-id="2daa3-148">Set the default output format</span></span>

<span data-ttu-id="2daa3-149">Use o comando interativo `az configure` para configurar seu ambiente e estabelecer as configurações padrão para formatos de saída.</span><span class="sxs-lookup"><span data-stu-id="2daa3-149">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="2daa3-150">O formato de saída padrão é `json`.</span><span class="sxs-lookup"><span data-stu-id="2daa3-150">The default output format is `json`.</span></span>

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
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

<span data-ttu-id="2daa3-151">Para saber mais sobre como configurar seu ambiente, confira [Configuração da CLI do Azure](./azure-cli-configuration.md).</span><span class="sxs-lookup"><span data-stu-id="2daa3-151">To learn more about configuring your environment, see [Azure CLI configuration](./azure-cli-configuration.md).</span></span>