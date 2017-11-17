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
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="e2e31-104">Gerenciar várias nuvens com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e2e31-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="e2e31-105">Se você tiver várias assinaturas associadas com o Azure, você pode ter mais de uma nuvem disponível.</span><span class="sxs-lookup"><span data-stu-id="e2e31-105">If you have multiple subscriptions associated with Azure, you may have more than one cloud available.</span></span> <span data-ttu-id="e2e31-106">Cada nuvem tem seus próprios pontos de extremidade e recursos associados e geralmente eles estão associados a uma região específica que tem requisitos ou padrões de proteção de dados diferentes.</span><span class="sxs-lookup"><span data-stu-id="e2e31-106">Each cloud has its own associated endpoints and capabilities, and is often associated with a particular region that has different data protection standards or requirements.</span></span>

<span data-ttu-id="e2e31-107">Para trabalhar efetivamente com várias nuvens, você precisará alternar entre a que está ativa no momento e possivelmente criar novas nuvens.</span><span class="sxs-lookup"><span data-stu-id="e2e31-107">To effectively work with multiple clouds, you will need to be able to switch between which is currently active, and possibly create new clouds.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="e2e31-108">Listagem de nuvens</span><span class="sxs-lookup"><span data-stu-id="e2e31-108">Listing clouds</span></span>

<span data-ttu-id="e2e31-109">Você pode listar suas nuvens disponíveis com o comando [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="e2e31-109">You may list your available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="e2e31-110">Isso informará qual nuvem está ativa no momento, qual é o seu perfil atual e também pode fornecer informações sobre nomes de host e sufixos regionais.</span><span class="sxs-lookup"><span data-stu-id="e2e31-110">This will tell you which cloud is currently active, what its current profile is, and can provide information on regional suffixes and host names.</span></span>

<span data-ttu-id="e2e31-111">Para obter uma lista de nuvens disponíveis e ativoas no momento:</span><span class="sxs-lookup"><span data-stu-id="e2e31-111">To get a list of the available clouds and the currently active one:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="e2e31-112">Alternar a nuvem ativa</span><span class="sxs-lookup"><span data-stu-id="e2e31-112">Switching the active cloud</span></span>

<span data-ttu-id="e2e31-113">Para alternar a nuvem ativa no momento, você deve executar o comando [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="e2e31-113">In order to switch the currently active cloud, you run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="e2e31-114">Esse comando usa um argumento necessário, o nome da nuvem.</span><span class="sxs-lookup"><span data-stu-id="e2e31-114">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="e2e31-115">Se você nunca tiver autenticado para a nuvem ativa, você precisará fazer isso antes de executar outras operações de CLI.</span><span class="sxs-lookup"><span data-stu-id="e2e31-115">If you have never authenticated for the active cloud, you will need to do so before performing any other CLI operations.</span></span> <span data-ttu-id="e2e31-116">Para obter instruções sobre autenticação, consulte [Fazer logon com a CLI do Azure 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="e2e31-116">For instructions on authenticating, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="register-or-unregister-a-cloud"></a><span data-ttu-id="e2e31-117">Registrar ou remover o registro de uma nuvem</span><span class="sxs-lookup"><span data-stu-id="e2e31-117">Register or unregister a cloud</span></span>

<span data-ttu-id="e2e31-118">Registre uma nova nuvem se você tem seus próprios pontos de extremidade ou precisa de um perfil diferente.</span><span class="sxs-lookup"><span data-stu-id="e2e31-118">Register a new cloud if you have your own endpoints or require a different profile.</span></span> <span data-ttu-id="e2e31-119">Uma nuvem é criado com o comando [cloud register](/cli/azure/cloud#register).</span><span class="sxs-lookup"><span data-stu-id="e2e31-119">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="e2e31-120">Este comando requer um nome e, opcionalmente, um conjunto de recursos e designações de ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="e2e31-120">This command requires a name, and optionally a set of capabilities and endpoint designations.</span></span>

<span data-ttu-id="e2e31-121">Para criar uma nuvem com um ponto de extremidade especializado para gerenciador de recursos, com um perfil específico:</span><span class="sxs-lookup"><span data-stu-id="e2e31-121">To create a cloud with a specialized endpoint for the resource manager, with a specific profile:</span></span>

```azurecli
az cloud register --name MyCloud --endpoint-resource-manager "https://my.endpoint.manager" --profile 2017-03-09-profile
```

<span data-ttu-id="e2e31-122">Isso cria a nuvem, mas _não_ a seleciona automaticamente.</span><span class="sxs-lookup"><span data-stu-id="e2e31-122">This creates the cloud, but does _not_ automatically select it.</span></span>

<span data-ttu-id="e2e31-123">Se você não precisar mais da nuvem criada, ela pode ter o registro removido com o comando [cloud unregister](/cli/azure/cloud#unregister):</span><span class="sxs-lookup"><span data-stu-id="e2e31-123">If you no longer require the created cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```

