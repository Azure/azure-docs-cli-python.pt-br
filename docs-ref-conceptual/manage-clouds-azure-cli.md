---
title: Selecionar nuvens com a CLI do Azure 2.0
description: Criar, conectar e gerenciar várias nuvens com a CLI do Azure 2.0.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 26b9f414ddaba3cc3f834b4749dee9807d84aa79
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388398"
---
# <a name="select-clouds-with-azure-cli-20"></a><span data-ttu-id="7a848-103">Selecionar nuvens com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="7a848-103">Select clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="7a848-104">Se você trabalha em regiões diferentes ou usa o [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), talvez precise usar mais de uma nuvem.</span><span class="sxs-lookup"><span data-stu-id="7a848-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="7a848-105">A Microsoft fornece nuvens para a conformidade com as leis regionais, que estão disponíveis seu uso.</span><span class="sxs-lookup"><span data-stu-id="7a848-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="7a848-106">Este artigo mostra como obter informações sobre as nuvens, alterar a nuvem atual e registrar ou cancelar o registro de novas nuvens.</span><span class="sxs-lookup"><span data-stu-id="7a848-106">This article shows you how to get information on clouds, change the current cloud, and register or unregister new clouds.</span></span>

## <a name="list-available-clouds"></a><span data-ttu-id="7a848-107">Listar nuvens disponíveis</span><span class="sxs-lookup"><span data-stu-id="7a848-107">List available clouds</span></span>

<span data-ttu-id="7a848-108">Você pode listar as nuvens disponíveis com o comando [az cloud list](/cli/azure/cloud#az-cloud-list).</span><span class="sxs-lookup"><span data-stu-id="7a848-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="7a848-109">Esse comando mostra qual nuvem está ativa no momento, qual é seu perfil atual e dará informações sobre os nomes de host e sufixos regionais.</span><span class="sxs-lookup"><span data-stu-id="7a848-109">This command shows which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="7a848-110">Para obter a nuvem ativa e uma lista de todas as nuvens disponíveis:</span><span class="sxs-lookup"><span data-stu-id="7a848-110">To get the active cloud and a list of all the available clouds:</span></span>

```azurecli-interactive
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

<span data-ttu-id="7a848-111">A nuvem ativa no momento possui `True` na coluna `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="7a848-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="7a848-112">Somente uma nuvem pode estar ativa em determinado momento.</span><span class="sxs-lookup"><span data-stu-id="7a848-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="7a848-113">Para obter informações mais detalhadas sobre uma nuvem, incluindo os pontos de extremidade que ela utiliza para os serviços do Azure, use o comando `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="7a848-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli-interactive
az cloud show --name AzureChinaCloud --output json
```

```output
{
  "endpoints": {
    "activeDirectory": "https://login.chinacloudapi.cn",
    "activeDirectoryDataLakeResourceId": null,
    "activeDirectoryGraphResourceId": "https://graph.chinacloudapi.cn/",
    "activeDirectoryResourceId": "https://management.core.chinacloudapi.cn/",
    "batchResourceId": "https://batch.chinacloudapi.cn/",
    "gallery": "https://gallery.chinacloudapi.cn/",
    "management": "https://management.core.chinacloudapi.cn/",
    "resourceManager": "https://management.chinacloudapi.cn",
    "sqlManagement": "https://management.core.chinacloudapi.cn:8443/",
    "vmImageAliasDoc": "https://raw.githubusercontent.com/Azure/azure-rest-api-specs/master/arm-compute/quickstart-templates/aliases.json"
  },
  "isActive": false,
  "name": "AzureChinaCloud",
  "profile": "latest",
  "suffixes": {
    "azureDatalakeAnalyticsCatalogAndJobEndpoint": null,
    "azureDatalakeStoreFileSystemEndpoint": null,
    "keyvaultDns": ".vault.azure.cn",
    "sqlServerHostname": ".database.chinacloudapi.cn",
    "storageEndpoint": "core.chinacloudapi.cn"
  }
}
```

## <a name="switch-the-active-cloud"></a><span data-ttu-id="7a848-114">Alternar a nuvem ativa</span><span class="sxs-lookup"><span data-stu-id="7a848-114">Switch the active cloud</span></span>

<span data-ttu-id="7a848-115">Para trocar a nuvem ativa no momento, execute o comando [az cloud set](/cli/azure/cloud#az-cloud-set).</span><span class="sxs-lookup"><span data-stu-id="7a848-115">To switch the currently active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="7a848-116">Esse comando usa um argumento necessário, o nome da nuvem.</span><span class="sxs-lookup"><span data-stu-id="7a848-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli-interactive
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="7a848-117">Se a autenticação para a nuvem ativada tiver expirado, você precisará autenticar novamente antes de realizar outras tarefas de CLI.</span><span class="sxs-lookup"><span data-stu-id="7a848-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="7a848-118">Se esta for a primeira vez em que troca para a nova nuvem, você também precisará definir a assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="7a848-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="7a848-119">Para obter instruções sobre a autenticação, consulte [Entrar com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="7a848-119">For instructions on authenticating, see [Sign in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="7a848-120">Para obter informações sobre o gerenciamento de assinaturas, confira [Gerenciar assinaturas do Azure com a CLI do Azure 2.0](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="7a848-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-new-cloud"></a><span data-ttu-id="7a848-121">Registrar uma nova nuvem</span><span class="sxs-lookup"><span data-stu-id="7a848-121">Register a new cloud</span></span>

<span data-ttu-id="7a848-122">Registre uma nova nuvem se tiver seus próprios pontos de extremidade do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7a848-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="7a848-123">Uma nuvem é criada com o comando [az cloud register](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="7a848-123">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="7a848-124">Este comando requer um nome e um conjunto de pontos de extremidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="7a848-124">This command requires a name and a set of service endpoints.</span></span> <span data-ttu-id="7a848-125">Para saber como registrar uma nuvem para usar com o Azure Stack, consulte [Usar perfis de versão da API com a CLI do Azure 2.0 no Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="7a848-125">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI 2.0 in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="7a848-126">Você não precisa registrar sua própria nuvem para regiões da Alemanha, China ou Governo dos EUA.</span><span class="sxs-lookup"><span data-stu-id="7a848-126">You do don't to register your own cloud for the China, US Government, or German regions.</span></span> <span data-ttu-id="7a848-127">Essas nuvens são gerenciadas pela Microsoft e ficam disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="7a848-127">These clouds are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="7a848-128">Para obter mais informações sobre todas as configurações do ponto de extremidade disponíveis, confira a [documentação para `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="7a848-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="7a848-129">Você não é automaticamente migrado para uma nuvem ao registrá-la.</span><span class="sxs-lookup"><span data-stu-id="7a848-129">Registering a cloud doesn't automatically switch to it.</span></span> <span data-ttu-id="7a848-130">Use o comando `az cloud set` para escolher a nuvem recém-criada.</span><span class="sxs-lookup"><span data-stu-id="7a848-130">Use the `az cloud set` command to select the newly created cloud.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="7a848-131">Atualizar uma nuvem existente</span><span class="sxs-lookup"><span data-stu-id="7a848-131">Update an existing cloud</span></span>

<span data-ttu-id="7a848-132">Se você tiver permissões, também poderá atualizar uma nuvem existente.</span><span class="sxs-lookup"><span data-stu-id="7a848-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="7a848-133">A atualização de uma nuvem leva à mudança para um perfil de serviços do Azure diferente ou modifica os pontos de extremidade da conexão.</span><span class="sxs-lookup"><span data-stu-id="7a848-133">Updating a cloud switches to a different Azure services profile or modifies the connection endpoints.</span></span>
<span data-ttu-id="7a848-134">Atualize uma nuvem com o comando [az cloud update](/cli/azure/cloud#az-cloud-update), que tem os mesmos argumentos de `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="7a848-134">Update a cloud with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="7a848-135">Cancelar o registro de uma nuvem</span><span class="sxs-lookup"><span data-stu-id="7a848-135">Unregister a cloud</span></span>

<span data-ttu-id="7a848-136">Se você já não precisar de uma nuvem criada, é possível remover seu registro com o comando [cloud unregister](/cli/azure/cloud#az-cloud-unregister):</span><span class="sxs-lookup"><span data-stu-id="7a848-136">If you no longer need a created cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli-interactive
az cloud unregister --name MyCloud
```
