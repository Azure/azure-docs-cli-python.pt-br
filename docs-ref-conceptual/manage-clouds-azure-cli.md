---
title: Gerenciar várias nuvens com a CLI do Azure 2.0
description: Criar, fazer logon e gerenciar várias nuvens com a CLI do Azure 2.0.
author: sptramer
manager: carmonm
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 98915fb43f2ad3eb45164f7e47c1a41345f3f9c5
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2018
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="38986-103">Gerenciar várias nuvens com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="38986-103">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="38986-104">Se você trabalha em regiões diferentes ou usa o [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), talvez precise usar mais de uma nuvem.</span><span class="sxs-lookup"><span data-stu-id="38986-104">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="38986-105">A Microsoft fornece nuvens para a conformidade com as leis regionais, que estão disponíveis seu uso.</span><span class="sxs-lookup"><span data-stu-id="38986-105">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="38986-106">Este artigo mostra como obter informações sobre as nuvens disponíveis para sua conta, alterar a nuvem atual e registrar ou cancelar o registro de novas nuvens para usar com o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="38986-106">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="38986-107">Listagem de nuvens</span><span class="sxs-lookup"><span data-stu-id="38986-107">Listing clouds</span></span>

<span data-ttu-id="38986-108">Você pode listar as nuvens disponíveis com o comando [az cloud list](/cli/azure/cloud#az-cloud-list).</span><span class="sxs-lookup"><span data-stu-id="38986-108">You can list available clouds with the [az cloud list](/cli/azure/cloud#az-cloud-list) command.</span></span> <span data-ttu-id="38986-109">Isso informará qual nuvem está ativa no momento, qual é seu perfil atual e dará informações sobre os nomes de host e sufixos regionais.</span><span class="sxs-lookup"><span data-stu-id="38986-109">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="38986-110">Para obter a nuvem ativa e uma lista de todas as nuvens disponíveis:</span><span class="sxs-lookup"><span data-stu-id="38986-110">To get the active cloud and a list of all the available clouds:</span></span>

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

<span data-ttu-id="38986-111">A nuvem ativa no momento possui `True` na coluna `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="38986-111">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="38986-112">Somente uma nuvem pode estar ativa em determinado momento.</span><span class="sxs-lookup"><span data-stu-id="38986-112">Only one cloud can be active at any time.</span></span> <span data-ttu-id="38986-113">Para obter informações mais detalhadas sobre uma nuvem, incluindo os pontos de extremidade que ela utiliza para os serviços do Azure, use o comando `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="38986-113">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

```azurecli
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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="38986-114">Alternar a nuvem ativa</span><span class="sxs-lookup"><span data-stu-id="38986-114">Switching the active cloud</span></span>

<span data-ttu-id="38986-115">Para trocar a nuvem ativa no momento, execute o comando [az cloud set](/cli/azure/cloud#az-cloud-set).</span><span class="sxs-lookup"><span data-stu-id="38986-115">To switch the currently active cloud, run the [az cloud set](/cli/azure/cloud#az-cloud-set) command.</span></span> <span data-ttu-id="38986-116">Esse comando usa um argumento necessário, o nome da nuvem.</span><span class="sxs-lookup"><span data-stu-id="38986-116">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="38986-117">Se a autenticação para a nuvem ativada tiver expirado, você precisará autenticar novamente antes de realizar outras tarefas de CLI.</span><span class="sxs-lookup"><span data-stu-id="38986-117">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="38986-118">Se esta for a primeira vez em que troca para a nova nuvem, você também precisará definir a assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="38986-118">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="38986-119">Para obter instruções sobre autenticação, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="38986-119">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="38986-120">Para obter informações sobre o gerenciamento de assinaturas, confira [Gerenciar assinaturas do Azure com a CLI do Azure 2.0](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="38986-120">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="38986-121">Registrar uma nuvem</span><span class="sxs-lookup"><span data-stu-id="38986-121">Register a cloud</span></span>

<span data-ttu-id="38986-122">Registre uma nova nuvem se tiver seus próprios pontos de extremidade do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="38986-122">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="38986-123">Uma nuvem é criada com o comando [az cloud register](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="38986-123">Creating a cloud is done with the [az cloud register](/cli/azure/cloud#az-cloud-register) command.</span></span> <span data-ttu-id="38986-124">Este comando requer um nome e um conjunto de recursos com pontos de extremidade associados.</span><span class="sxs-lookup"><span data-stu-id="38986-124">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="38986-125">Para saber como registrar uma nuvem para usar com o Azure Stack, consulte [Usar perfis de versão da API com a CLI do Azure 2.0 no Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="38986-125">To learn how to register a cloud for use with Azure Stack, see [Use API version profiles with Azure CLI 2.0 in Azure Stack](/azure/azure-stack/user/azure-stack-version-profiles-azurecli2#connect-to-azure-stack).</span></span>

<span data-ttu-id="38986-126">Você não precisa registrar sua própria nuvem para regiões na China, Governo dos EUA ou Alemanha.</span><span class="sxs-lookup"><span data-stu-id="38986-126">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="38986-127">São gerenciadas pela Microsoft e ficam disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="38986-127">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="38986-128">Para obter mais informações sobre todas as configurações do ponto de extremidade disponíveis, confira a [documentação para `az cloud register`](/cli/azure/cloud#az-cloud-register).</span><span class="sxs-lookup"><span data-stu-id="38986-128">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud#az-cloud-register).</span></span>

<span data-ttu-id="38986-129">Registrar uma nuvem não troca automaticamente para ela.</span><span class="sxs-lookup"><span data-stu-id="38986-129">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="38986-130">Use o comando `az cloud set` para selecionar a nuvem recém-criada, conforme descrito acima.</span><span class="sxs-lookup"><span data-stu-id="38986-130">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="38986-131">Atualizar uma nuvem existente</span><span class="sxs-lookup"><span data-stu-id="38986-131">Update an existing cloud</span></span>

<span data-ttu-id="38986-132">Se você tiver permissões, também poderá atualizar uma nuvem existente.</span><span class="sxs-lookup"><span data-stu-id="38986-132">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="38986-133">Faça isso quando precisar trocar para um perfil diferente do Azure, adicionar ou alterar um ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="38986-133">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="38986-134">Você faz isso com o comando [az cloud update](/cli/azure/cloud#az-cloud-update), que tem os mesmos argumentos de `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="38986-134">You do this with the [az cloud update](/cli/azure/cloud#az-cloud-update) command, which takes the same arguments as `az cloud register`.</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="38986-135">Cancelar o registro de uma nuvem</span><span class="sxs-lookup"><span data-stu-id="38986-135">Unregister a cloud</span></span>

<span data-ttu-id="38986-136">Se você não precisar de uma nuvem registrada, o registro poderá ser cancelado com o comando [az cloud unregister](/cli/azure/cloud#az-cloud-unregister):</span><span class="sxs-lookup"><span data-stu-id="38986-136">If you no longer require a registered cloud, it can be unregistered with the [az cloud unregister](/cli/azure/cloud#az-cloud-unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```
