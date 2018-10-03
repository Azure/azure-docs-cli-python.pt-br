---
title: Resultados de comando de consulta com a CLI do Azure
description: Saiba como realizar consultas JMESPath na saída dos comandos da CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 4522242952e5d257449c9c593885c62de2f56d0f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178024"
---
# <a name="use-jmespath-queries-with-azure-cli"></a><span data-ttu-id="cf86b-103">Usar consultas JMESPath com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="cf86b-103">Use JMESPath queries with Azure CLI</span></span> 

<span data-ttu-id="cf86b-104">A CLI do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados dos comandos.</span><span class="sxs-lookup"><span data-stu-id="cf86b-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="cf86b-105">JMESPath é uma linguagem de consulta para JSON, permitindo que você selecione e apresente dados de saída da CLI.</span><span class="sxs-lookup"><span data-stu-id="cf86b-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="cf86b-106">Essas consultas são executadas na saída JSON antes de qualquer formatação de exibição.</span><span class="sxs-lookup"><span data-stu-id="cf86b-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="cf86b-107">O argumento `--query` tem suporte de todos os comandos na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="cf86b-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="cf86b-108">Os exemplos deste artigo abrangem os casos de uso comum e demonstram como usar os recursos do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="cf86b-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="cf86b-109">Trabalhar com saída de dicionário</span><span class="sxs-lookup"><span data-stu-id="cf86b-109">Work with dictionary output</span></span>

<span data-ttu-id="cf86b-110">Comandos que retornam um dicionário em JSON só podem ser explorados por seus nomes de chave.</span><span class="sxs-lookup"><span data-stu-id="cf86b-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="cf86b-111">Os caminhos de chave usam o caractere `.` como separador.</span><span class="sxs-lookup"><span data-stu-id="cf86b-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="cf86b-112">O exemplo a seguir efetua pull de uma lista de chaves SSH públicas que têm permissão para se conectar a uma VM do Linux:</span><span class="sxs-lookup"><span data-stu-id="cf86b-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="cf86b-113">Vários valores podem ser colocados em uma matriz ordenada.</span><span class="sxs-lookup"><span data-stu-id="cf86b-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="cf86b-114">O exemplo a seguir mostra como recuperar a imagem do Azure oferecendo o nome e o tamanho do disco do sistema operacional:</span><span class="sxs-lookup"><span data-stu-id="cf86b-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="cf86b-115">Se quiser chaves em sua saída, você pode usar uma sintaxe de dicionário alternativa.</span><span class="sxs-lookup"><span data-stu-id="cf86b-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="cf86b-116">A escolha do elemento em um dicionário usa o formato `{displayKey:keyPath, ...}` para filtrar na expressão `keyPath` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="cf86b-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="cf86b-117">Nos valores de saída, os pares chave/valor são alterados para `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="cf86b-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="cf86b-118">O exemplo a seguir usa a consulta do último exemplo e a torna mais clara com a atribuição de chaves para a saída:</span><span class="sxs-lookup"><span data-stu-id="cf86b-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="cf86b-119">Ao exibir as informações de formato de saída `table`, a exibição de dicionário permite configurar seus próprios cabeçalhos de coluna.</span><span class="sxs-lookup"><span data-stu-id="cf86b-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="cf86b-120">Para obter mais informações sobre formatos de saída, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="cf86b-120">For more information on output formats, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="cf86b-121">Algumas chaves são filtradas e não são impressas na exibição da tabela.</span><span class="sxs-lookup"><span data-stu-id="cf86b-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="cf86b-122">Essas chaves são `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="cf86b-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="cf86b-123">Caso precise ver essas informações, é possível alterar o nome da chave e evitar a filtragem.</span><span class="sxs-lookup"><span data-stu-id="cf86b-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="cf86b-124">Trabalhar com saída de lista</span><span class="sxs-lookup"><span data-stu-id="cf86b-124">Work with list output</span></span>

<span data-ttu-id="cf86b-125">Os comandos da CLI que podem retornar mais de um valor retornam uma matriz.</span><span class="sxs-lookup"><span data-stu-id="cf86b-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="cf86b-126">Os elementos da matriz são acessados por índice e não podem ser sempre retornados na mesma ordem.</span><span class="sxs-lookup"><span data-stu-id="cf86b-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="cf86b-127">É possível consultar todos os elementos da matriz ao mesmo tempo mesclando-os com o operador `[]`.</span><span class="sxs-lookup"><span data-stu-id="cf86b-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="cf86b-128">O operador é colocado depois da matriz ou como o primeiro elemento em uma expressão.</span><span class="sxs-lookup"><span data-stu-id="cf86b-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="cf86b-129">Mesclar uma matriz executa a consulta depois dela em relação a cada elemento da matriz.</span><span class="sxs-lookup"><span data-stu-id="cf86b-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="cf86b-130">O exemplo a seguir imprime o nome e o sistema operacional em execução em cada VM em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="cf86b-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

<span data-ttu-id="cf86b-131">As matrizes que fazem parte de um caminho de chave também podem ser mescladas.</span><span class="sxs-lookup"><span data-stu-id="cf86b-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="cf86b-132">A consulta a seguir obtém as IDs de objeto do Azure para as NICs às quais uma VM está conectada.</span><span class="sxs-lookup"><span data-stu-id="cf86b-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="cf86b-133">Saída de matriz de filtro com predicados</span><span class="sxs-lookup"><span data-stu-id="cf86b-133">Filter array output with predicates</span></span>

<span data-ttu-id="cf86b-134">O JMESPath oferece [expressões de filtragem](http://jmespath.org/specification.html#filterexpressions) para filtrar os dados exibidos.</span><span class="sxs-lookup"><span data-stu-id="cf86b-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="cf86b-135">Essas expressões são eficientes, especialmente quando combinadas com [funções internas do JMESPath](http://jmespath.org/specification.html#built-in-functions) para realizar correspondências parciais ou manipular dados em um formato padrão.</span><span class="sxs-lookup"><span data-stu-id="cf86b-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="cf86b-136">As expressões de filtragem só funcionam em dados de matriz e, quando usadas em qualquer outra situação, retornam o valor `null`.</span><span class="sxs-lookup"><span data-stu-id="cf86b-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="cf86b-137">Por exemplo, é possível usar a saída de comandos como a `vm list` e filtrá-la para procurar tipos específicos de VMs.</span><span class="sxs-lookup"><span data-stu-id="cf86b-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="cf86b-138">O exemplo a seguir vai além do anterior, filtrando o tipo de VM para capturar somente VMs do Windows e imprimir seu nome.</span><span class="sxs-lookup"><span data-stu-id="cf86b-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="cf86b-139">Experimentar consultas interativamente</span><span class="sxs-lookup"><span data-stu-id="cf86b-139">Experiment with queries interactively</span></span>

<span data-ttu-id="cf86b-140">Para começar a aprender JMESPath, o pacote Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) oferece um ambiente interativo para testar as consultas.</span><span class="sxs-lookup"><span data-stu-id="cf86b-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="cf86b-141">Os dados são inseridos como entrada e, em seguida, as consultas no programa são gravadas e editadas para extrair os dados.</span><span class="sxs-lookup"><span data-stu-id="cf86b-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
