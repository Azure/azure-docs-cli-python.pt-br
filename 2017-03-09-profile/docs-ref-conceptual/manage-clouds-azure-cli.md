---
title: "Gerenciar várias nuvens com a CLI do Azure 2.0"
description: Criar, fazer logon e gerenciar nuvens diferentes com a CLI do Azure 2.0.
keywords: "CLI do Azure 2.0, Azure, nuvens, datacenters, governo, região, China, Alemanha"
author: sptramer
manager: douge
ms.author: sttramer
ms.date: 06/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0222b7339e46346ef6c7e9ad98616d9b71129942
ms.sourcegitcommit: f107cf927ea1ef51de181d87fc4bc078e9288e47
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a>Gerenciar várias nuvens com a CLI do Azure 2.0

Se você tiver várias assinaturas associadas com o Azure, você pode ter mais de uma nuvem disponível. Cada nuvem tem seus próprios pontos de extremidade e recursos associados e geralmente eles estão associados a uma região específica que tem requisitos ou padrões de proteção de dados diferentes.

Para trabalhar efetivamente com várias nuvens, você precisará alternar entre a que está ativa no momento e possivelmente criar novas nuvens.

## <a name="listing-clouds"></a>Listagem de nuvens

Você pode listar suas nuvens disponíveis com o comando [cloud list](/cli/azure/cloud#list). Isso informará qual nuvem está ativa no momento, qual é o seu perfil atual e também pode fornecer informações sobre nomes de host e sufixos regionais.

Para obter uma lista de nuvens disponíveis e ativoas no momento:

```azurecli
az cloud list --output table
```

```output
IsActive    Name               Profile
----------  -----------------  ---------
True        AzureCloud         latest
            AzureChinaCloud    latest
            AzureUSGovernment  latest
            AzureGermanCloud   latest
```

## <a name="switching-the-active-cloud"></a>Alternar a nuvem ativa

Para alternar a nuvem ativa no momento, você deve executar o comando [cloud set](/cli/azure/cloud#set). Esse comando usa um argumento necessário, o nome da nuvem.

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> Se você nunca tiver autenticado para a nuvem ativa, você precisará fazer isso antes de executar outras operações de CLI. Para obter instruções sobre autenticação, consulte [Fazer logon com a CLI do Azure 2.0](/cli/azure/authenticate-azure-cli).

## <a name="register-or-unregister-a-cloud"></a>Registrar ou remover o registro de uma nuvem

Registre uma nova nuvem se você tem seus próprios pontos de extremidade ou precisa de um perfil diferente. Uma nuvem é criado com o comando [cloud register](/cli/azure/cloud#register). Este comando requer um nome e, opcionalmente, um conjunto de recursos e designações de ponto de extremidade.

Para criar uma nuvem com um ponto de extremidade especializado para gerenciador de recursos, com um perfil específico:

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

Isso cria a nuvem, mas _não_ a seleciona automaticamente.

Se você não precisar mais da nuvem criada, ela pode ter o registro removido com o comando [cloud unregister](/cli/azure/cloud#unregister):

```azurecli
az cloud unregister --name MyCloud
```

