---
title: Resultados do comando de consulta com a CLI do Azure 2.0
description: Saiba como realizar consultas JMESPath na saída dos comandos da CLI do Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: ed8f8ac160dd8225170ffcfff9619d94b92e456a
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a>Usar consultas JMESPath com a CLI do Azure 2.0

A CLI 2.0 do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados de comandos. JMESPath é uma linguagem de consulta para JSON, permitindo que você selecione e apresente dados de saída da CLI. Essas consultas são executadas na saída JSON antes de executar qualquer outra formatação de exibição.

O argumento `--query` tem suporte de todos os comandos na CLI do Azure. Os exemplos deste artigo abrangem os casos de uso comum e demonstram como usar os recursos do JMESPath.

## <a name="work-with-dictionary-output"></a>Trabalhar com saída de dicionário

Comandos que retornam um dicionário em JSON só podem ser explorados por seus nomes de chave. Os caminhos de chave usam o caractere `.` como separador. O exemplo a seguir efetua pull de uma lista de chaves SSH públicas que têm permissão para se conectar a uma VM do Linux:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Também é possível obter vários valores, colocando-os em uma matriz ordenada. A matriz não tem nenhuma informação de chave, mas a ordem dos elementos da matriz corresponde à ordem das chaves consultadas. O exemplo a seguir mostra como recuperar a imagem do Azure oferecendo o nome e o tamanho do disco do sistema operacional:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Se quiser chaves em sua saída, você pode usar uma sintaxe de dicionário alternativa. A seleção múltipla do elemento em um dicionário usa o formato `{displayKey:keyPath, ...}` para filtrar na expressão `keyPath` do JMESPath. Isso é exibido na saída como `{displayKey: value}`. O exemplo a seguir usa a consulta do último exemplo e a torna mais clara com a atribuição de chaves para a saída:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Ao exibir as informações de formato de saída `table`, a exibição de dicionário é bastante útil. Isso permite configurar seus próprios cabeçalhos de coluna, tornando a leitura da saída ainda mais fácil. Para obter mais informações sobre formatos de saída, confira [Formatos de saída para comandos da CLI 2.0 do Azure](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Algumas chaves são filtradas e não são impressas na exibição da tabela. Essas chaves são `id`, `type` e `etag`. Caso precise ver essas informações, é possível alterar o nome da chave e evitar a filtragem.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Trabalhar com saída de lista

Os comandos da CLI que podem retornar mais de um valor sempre retornam uma matriz. As matrizes podem ter seus elementos acessados por índice, mas nunca há uma garantia de ordem da CLI. A melhor maneira de consultar uma matriz de valores é mesclando-os com o operador `[]`. O operador será gravado depois da chave para a matriz ou como o primeiro elemento na expressão. A mescla executa a consulta a seguindo em relação a cada elemento individual na matriz e coloca os valores resultantes em uma nova matriz. O exemplo a seguir imprime o nome e o sistema operacional em execução em cada VM em um grupo de recursos. 

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

As matrizes que fazem parte de um caminho de chave também podem ser mescladas. Este exemplo demonstra uma consulta que obtém as IDs de objeto do Azure para as NICs às quais uma VM está conectada.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Saída de matriz de filtro com predicados

O JMESPath oferece [expressões de filtragem](http://jmespath.org/specification.html#filterexpressions) para filtrar os dados exibidos. Essas expressões são eficientes, especialmente quando combinadas com [funções internas do JMESPath](http://jmespath.org/specification.html#built-in-functions) para executar correspondências parciais ou manipular dados em um formato padrão. As expressões de filtragem só funcionam em dados de matriz e, quando usadas em qualquer outra situação, retornam o valor `null`. Por exemplo, é possível usar a saída de comandos como a `vm list` e filtrá-la para procurar tipos específicos de VMs. O exemplo a seguir vai além do anterior, filtrando o tipo de VM para capturar somente VMs do Windows e imprimir seu nome.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Experimentar consultas interativamente

Para experimentar expressões JMESPath, convém trabalhar de maneira que você possa editar consultas e inspecionar a saída rapidamente. Um ambiente interativo é oferecido pelo pacote [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) do Python, o qual permite fazer o piping de dados como entrada e, em seguida, gavar consultas internas no programa para extrair os dados.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
