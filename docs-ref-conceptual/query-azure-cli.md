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
# <a name="use-jmespath-queries-with-azure-cli"></a>Usar consultas JMESPath com a CLI do Azure 

A CLI do Azure usa o argumento `--query` para executar uma [consulta JMESPath](http://jmespath.org) nos resultados dos comandos. JMESPath é uma linguagem de consulta para JSON, permitindo que você selecione e apresente dados de saída da CLI. Essas consultas são executadas na saída JSON antes de qualquer formatação de exibição.

O argumento `--query` tem suporte de todos os comandos na CLI do Azure. Os exemplos deste artigo abrangem os casos de uso comum e demonstram como usar os recursos do JMESPath.

## <a name="work-with-dictionary-output"></a>Trabalhar com saída de dicionário

Comandos que retornam um dicionário em JSON só podem ser explorados por seus nomes de chave. Os caminhos de chave usam o caractere `.` como separador. O exemplo a seguir efetua pull de uma lista de chaves SSH públicas que têm permissão para se conectar a uma VM do Linux:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Vários valores podem ser colocados em uma matriz ordenada. O exemplo a seguir mostra como recuperar a imagem do Azure oferecendo o nome e o tamanho do disco do sistema operacional:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Se quiser chaves em sua saída, você pode usar uma sintaxe de dicionário alternativa.  A escolha do elemento em um dicionário usa o formato `{displayKey:keyPath, ...}` para filtrar na expressão `keyPath` do JMESPath. Nos valores de saída, os pares chave/valor são alterados para `{displayKey: value}`. O exemplo a seguir usa a consulta do último exemplo e a torna mais clara com a atribuição de chaves para a saída:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Ao exibir as informações de formato de saída `table`, a exibição de dicionário permite configurar seus próprios cabeçalhos de coluna. Para obter mais informações sobre formatos de saída, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Algumas chaves são filtradas e não são impressas na exibição da tabela. Essas chaves são `id`, `type` e `etag`. Caso precise ver essas informações, é possível alterar o nome da chave e evitar a filtragem.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Trabalhar com saída de lista

Os comandos da CLI que podem retornar mais de um valor retornam uma matriz. Os elementos da matriz são acessados por índice e não podem ser sempre retornados na mesma ordem. É possível consultar todos os elementos da matriz ao mesmo tempo mesclando-os com o operador `[]`. O operador é colocado depois da matriz ou como o primeiro elemento em uma expressão. Mesclar uma matriz executa a consulta depois dela em relação a cada elemento da matriz.

O exemplo a seguir imprime o nome e o sistema operacional em execução em cada VM em um grupo de recursos.

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

As matrizes que fazem parte de um caminho de chave também podem ser mescladas. A consulta a seguir obtém as IDs de objeto do Azure para as NICs às quais uma VM está conectada.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Saída de matriz de filtro com predicados

O JMESPath oferece [expressões de filtragem](http://jmespath.org/specification.html#filterexpressions) para filtrar os dados exibidos. Essas expressões são eficientes, especialmente quando combinadas com [funções internas do JMESPath](http://jmespath.org/specification.html#built-in-functions) para realizar correspondências parciais ou manipular dados em um formato padrão. As expressões de filtragem só funcionam em dados de matriz e, quando usadas em qualquer outra situação, retornam o valor `null`. Por exemplo, é possível usar a saída de comandos como a `vm list` e filtrá-la para procurar tipos específicos de VMs. O exemplo a seguir vai além do anterior, filtrando o tipo de VM para capturar somente VMs do Windows e imprimir seu nome.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Experimentar consultas interativamente

Para começar a aprender JMESPath, o pacote Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) oferece um ambiente interativo para testar as consultas. Os dados são inseridos como entrada e, em seguida, as consultas no programa são gravadas e editadas para extrair os dados.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
