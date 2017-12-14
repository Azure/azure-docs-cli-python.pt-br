---
title: Resultados do comando de consulta com a CLI do Azure 2.0
description: "Use --query para realizar consultas JMESPath na saída dos comandos da CLI do Azure 2.0."
keywords: CLI do Azure 2.0, JMESPath, consulta, Linux, Mac, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: b086785f7b20622111e0a05e7cc7c27ddb5449b5
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="9399e-104">Como usar consultas JMESPath com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="9399e-104">Using JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="9399e-105">A CLI do Azure 2.0 usa o parâmetro `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados do comando `az`.</span><span class="sxs-lookup"><span data-stu-id="9399e-105">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="9399e-106">JMESPath é uma linguagem de consulta eficiente para saídas JSON.</span><span class="sxs-lookup"><span data-stu-id="9399e-106">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="9399e-107">Se estiver familiarizado com consultas JMESPath, consulte um tutorial em [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="9399e-107">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="9399e-108">O parâmetro `Query` é suportado por cada tipo de recurso (Serviços de Contêiner, Aplicativos Web, VM, etc.) na CLI do Azure 2.0 e pode ser usado para várias finalidades diferentes.</span><span class="sxs-lookup"><span data-stu-id="9399e-108">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="9399e-109">Listamos vários exemplos abaixo.</span><span class="sxs-lookup"><span data-stu-id="9399e-109">We have listed several examples below.</span></span>

## <a name="selecting-simple-properties"></a><span data-ttu-id="9399e-110">Seleção de propriedades simples</span><span class="sxs-lookup"><span data-stu-id="9399e-110">Selecting simple properties</span></span>

<span data-ttu-id="9399e-111">O comando `list` simples com o formato de saída `table` retorna um conjunto estruturado com as propriedades mais comuns e simples para cada tipo de recurso em um formato tabular de fácil leitura.</span><span class="sxs-lookup"><span data-stu-id="9399e-111">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

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

<span data-ttu-id="9399e-112">Você pode usar o parâmetro `--query` para mostrar apenas o nome do Grupo de Recursos e o nome da VM para todas as máquinas virtuais em sua assinatura.</span><span class="sxs-lookup"><span data-stu-id="9399e-112">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query [*].[name, resourceGroup] --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

<span data-ttu-id="9399e-113">No exemplo anterior, observe que os cabeçalhos das colunas são "Coluna1" e "Coluna2".</span><span class="sxs-lookup"><span data-stu-id="9399e-113">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="9399e-114">Também é possível adicionar nomes ou rótulos amigáveis às propriedades selecionadas.</span><span class="sxs-lookup"><span data-stu-id="9399e-114">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="9399e-115">No exemplo a seguir, adicionamos os rótulos "VMName" e "RGName" às propriedades selecionadas "name" e "resourceGroup".</span><span class="sxs-lookup"><span data-stu-id="9399e-115">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="selecting-complex-nested-properties"></a><span data-ttu-id="9399e-116">Seleção de propriedades aninhadas complexas</span><span class="sxs-lookup"><span data-stu-id="9399e-116">Selecting complex nested properties</span></span>

<span data-ttu-id="9399e-117">Se a propriedade que você deseja selecionar estiver aninhada profundamente na saída JSON, será necessário fornecer o caminho completo para a propriedade aninhada.</span><span class="sxs-lookup"><span data-stu-id="9399e-117">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="9399e-118">O exemplo a seguir mostra como selecionar o nome da VM e o tipo do SO a partir do comando de lista da vm.</span><span class="sxs-lookup"><span data-stu-id="9399e-118">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="9399e-119">Filtrar com a função contains</span><span class="sxs-lookup"><span data-stu-id="9399e-119">Filter with the contains function</span></span>

<span data-ttu-id="9399e-120">Você pode usar a função `contains` do JMESPath para refinar os resultados retornados na consulta.</span><span class="sxs-lookup"><span data-stu-id="9399e-120">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="9399e-121">No exemplo a seguir, o comando seleciona apenas as VMs com o texto "RGD" em seu nome.</span><span class="sxs-lookup"><span data-stu-id="9399e-121">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

<span data-ttu-id="9399e-122">Com o exemplo a seguir, os resultados retornarão as VMs com o vmSize 'Standard_DS1'.</span><span class="sxs-lookup"><span data-stu-id="9399e-122">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a><span data-ttu-id="9399e-123">Filtrar com grep</span><span class="sxs-lookup"><span data-stu-id="9399e-123">Filter with grep</span></span>

<span data-ttu-id="9399e-124">O formato de saída `tsv` é um texto separado por tabulações sem cabeçalhos.</span><span class="sxs-lookup"><span data-stu-id="9399e-124">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="9399e-125">Ele pode ser transferido para comandos como `grep` e `cut` para analisar ainda mais os valores específicos da saída `list`.</span><span class="sxs-lookup"><span data-stu-id="9399e-125">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="9399e-126">No exemplo a seguir, o comando `grep` seleciona apenas as VMs com o texto "RGD" em seu nome.</span><span class="sxs-lookup"><span data-stu-id="9399e-126">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="9399e-127">O comando `cut` seleciona apenas o valor do oitavo campo (separado por tabulações) para mostrar na saída.</span><span class="sxs-lookup"><span data-stu-id="9399e-127">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="9399e-128">Explorar com jpterm</span><span class="sxs-lookup"><span data-stu-id="9399e-128">Explore with jpterm</span></span>

<span data-ttu-id="9399e-129">Você também pode transferir a saída do comando para [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) e testar sua consulta JMESPath lá.</span><span class="sxs-lookup"><span data-stu-id="9399e-129">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

