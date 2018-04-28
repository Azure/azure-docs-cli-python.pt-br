---
title: Resultados do comando de consulta com a CLI do Azure 2.0
description: Saiba como realizar consultas JMESPath na saída dos comandos da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/22/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: eb9311686bf950a450db4bc450da363bbe409f49
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="1cdf6-103">Usar consultas JMESPath com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="1cdf6-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="1cdf6-104">A CLI 2.0 do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados de comandos.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="1cdf6-105">JMESPath é uma linguagem de consulta para JSON, permitindo que você selecione e apresente dados de saída da CLI.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="1cdf6-106">Essas consultas são executadas na saída JSON antes de executar qualquer outra formatação de exibição.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-106">These queries are executed on the JSON output, before performing any other display formatting.</span></span>

<span data-ttu-id="1cdf6-107">O argumento `--query` tem suporte de todos os comandos na CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="1cdf6-108">Os exemplos deste artigo abrangem os casos de uso comum e demonstram como usar os recursos do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="1cdf6-109">Trabalhar com saída de dicionário</span><span class="sxs-lookup"><span data-stu-id="1cdf6-109">Work with dictionary output</span></span>

<span data-ttu-id="1cdf6-110">Comandos que retornam um dicionário em JSON só podem ser explorados por seus nomes de chave.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="1cdf6-111">Os caminhos de chave usam o caractere `.` como separador.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="1cdf6-112">O exemplo a seguir efetua pull de uma lista de chaves SSH públicas que têm permissão para se conectar a uma VM do Linux:</span><span class="sxs-lookup"><span data-stu-id="1cdf6-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="1cdf6-113">Também é possível obter vários valores, colocando-os em uma matriz ordenada.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-113">You can also get multiple values, putting them in an ordered array.</span></span> <span data-ttu-id="1cdf6-114">A matriz não tem nenhuma informação de chave, mas a ordem dos elementos da matriz corresponde à ordem das chaves consultadas.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-114">The array doesn't have any key information, but the order of the array's elements matches the order of the queried keys.</span></span> <span data-ttu-id="1cdf6-115">O exemplo a seguir mostra como recuperar a imagem do Azure oferecendo o nome e o tamanho do disco do sistema operacional:</span><span class="sxs-lookup"><span data-stu-id="1cdf6-115">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="1cdf6-116">Se quiser chaves em sua saída, você pode usar uma sintaxe de dicionário alternativa.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-116">If you want keys in your output, you can use an alternate dictionary syntax.</span></span> <span data-ttu-id="1cdf6-117">A seleção múltipla do elemento em um dicionário usa o formato `{displayKey:keyPath, ...}` para filtrar na expressão `keyPath` do JMESPath.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-117">Multiple element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="1cdf6-118">Isso é exibido na saída como `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-118">This displays in the output as `{displayKey: value}`.</span></span> <span data-ttu-id="1cdf6-119">O exemplo a seguir usa a consulta do último exemplo e a torna mais clara com a atribuição de chaves para a saída:</span><span class="sxs-lookup"><span data-stu-id="1cdf6-119">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="1cdf6-120">Ao exibir as informações de formato de saída `table`, a exibição de dicionário é bastante útil.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-120">When displaying information in the `table` output format, dictionary display is especially useful.</span></span> <span data-ttu-id="1cdf6-121">Isso permite configurar seus próprios cabeçalhos de coluna, tornando a leitura da saída ainda mais fácil.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-121">This allows for setting your own column headers, making output even easier to read.</span></span> <span data-ttu-id="1cdf6-122">Para obter mais informações sobre formatos de saída, confira [Formatos de saída para comandos da CLI 2.0 do Azure](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="1cdf6-122">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="1cdf6-123">Algumas chaves são filtradas e não são impressas na exibição da tabela.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-123">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="1cdf6-124">Essas chaves são `id`, `type` e `etag`.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-124">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="1cdf6-125">Caso precise ver essas informações, é possível alterar o nome da chave e evitar a filtragem.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-125">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="1cdf6-126">Trabalhar com saída de lista</span><span class="sxs-lookup"><span data-stu-id="1cdf6-126">Work with list output</span></span>

<span data-ttu-id="1cdf6-127">Os comandos da CLI que podem retornar mais de um valor sempre retornam uma matriz.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-127">CLI commands that may return more than one value always return an array.</span></span> <span data-ttu-id="1cdf6-128">As matrizes podem ter seus elementos acessados por índice, mas nunca há uma garantia de ordem da CLI.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-128">Arrays can have their elements accessed by index, but there's never an order guarantee from the CLI.</span></span> <span data-ttu-id="1cdf6-129">A melhor maneira de consultar uma matriz de valores é mesclando-os com o operador `[]`.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-129">The best way to query an array of values is to flatten them with the `[]` operator.</span></span> <span data-ttu-id="1cdf6-130">O operador será gravado depois da chave para a matriz ou como o primeiro elemento na expressão.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-130">The operator is written after the key for the array, or as the first element in the expression.</span></span> <span data-ttu-id="1cdf6-131">A mescla executa a consulta a seguindo em relação a cada elemento individual na matriz e coloca os valores resultantes em uma nova matriz.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-131">Flattening runs the query following it against each individual element in the array, and places the resulting values into a new array.</span></span> <span data-ttu-id="1cdf6-132">O exemplo a seguir imprime o nome e o sistema operacional em execução em cada VM em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-132">The following example prints out the name and OS running on each VM in a resource group.</span></span> 

```azurecli
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

<span data-ttu-id="1cdf6-133">As matrizes que fazem parte de um caminho de chave também podem ser mescladas.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-133">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="1cdf6-134">Este exemplo demonstra uma consulta que obtém as IDs de objeto do Azure para as NICs às quais uma VM está conectada.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-134">This example demonstrates a query that gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="1cdf6-135">Saída de matriz de filtro com predicados</span><span class="sxs-lookup"><span data-stu-id="1cdf6-135">Filter array output with predicates</span></span>

<span data-ttu-id="1cdf6-136">O JMESPath oferece [expressões de filtragem](http://jmespath.org/specification.html#filterexpressions) para filtrar os dados exibidos.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-136">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="1cdf6-137">Essas expressões são eficientes, especialmente quando combinadas com [funções internas do JMESPath](http://jmespath.org/specification.html#built-in-functions) para executar correspondências parciais ou manipular dados em um formato padrão.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-137">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to perform partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="1cdf6-138">As expressões de filtragem só funcionam em dados de matriz e, quando usadas em qualquer outra situação, retornam o valor `null`.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-138">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="1cdf6-139">Por exemplo, é possível usar a saída de comandos como a `vm list` e filtrá-la para procurar tipos específicos de VMs.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-139">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="1cdf6-140">O exemplo a seguir vai além do anterior, filtrando o tipo de VM para capturar somente VMs do Windows e imprimir seu nome.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-140">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="1cdf6-141">Experimentar consultas interativamente</span><span class="sxs-lookup"><span data-stu-id="1cdf6-141">Experiment with queries interactively</span></span>

<span data-ttu-id="1cdf6-142">Para experimentar expressões JMESPath, convém trabalhar de maneira que você possa editar consultas e inspecionar a saída rapidamente.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-142">To experiment with JMESPath expressions, you might want to work in a way where you can quickly edit queries and inspect the output.</span></span> <span data-ttu-id="1cdf6-143">Um ambiente interativo é oferecido pelo pacote [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) do Python, o qual permite fazer o piping de dados como entrada e, em seguida, gavar consultas internas no programa para extrair os dados.</span><span class="sxs-lookup"><span data-stu-id="1cdf6-143">An interactive environment is offered by the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package, which allows for piping data as input and then writing in-program queries to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
