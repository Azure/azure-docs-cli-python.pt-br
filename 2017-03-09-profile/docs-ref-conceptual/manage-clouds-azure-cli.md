---
title: "Gerenciar várias nuvens com a CLI do Azure 2.0"
description: Criar, fazer logon e gerenciar nuvens diferentes com a CLI do Azure 2.0.
keywords: "CLI do Azure 2.0, Azure, nuvens, datacenters, governo, região, China, Alemanha"
author: sptramer
manager: routlaw
ms.author: sttramer
ms.date: 10/20/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.openlocfilehash: 0eb07d2919f6e640e1d594db9e18f9ada4d9f59f
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2017
---
# <a name="managing-multiple-clouds-with-azure-cli-20"></a><span data-ttu-id="33063-104">Gerenciar várias nuvens com a CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="33063-104">Managing multiple clouds with Azure CLI 2.0</span></span>

<span data-ttu-id="33063-105">Se você trabalha em regiões diferentes ou usa o [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/), talvez precise usar mais de uma nuvem.</span><span class="sxs-lookup"><span data-stu-id="33063-105">If you work across different regions or use [Azure Stack](https://docs.microsoft.com/en-us/azure/azure-stack/user/), you may need to use more than one cloud.</span></span> <span data-ttu-id="33063-106">A Microsoft fornece nuvens para a conformidade com as leis regionais, que estão disponíveis seu uso.</span><span class="sxs-lookup"><span data-stu-id="33063-106">Microsoft provides clouds for compliance with regional laws, which are available for your use.</span></span> <span data-ttu-id="33063-107">Este artigo mostra como obter informações sobre as nuvens disponíveis para sua conta, alterar a nuvem atual e registrar ou cancelar o registro de novas nuvens para usar com o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="33063-107">This article shows you how to get information on clouds available to your account, change the current cloud, and register or unregister new clouds for use with Azure Stack.</span></span>

## <a name="listing-clouds"></a><span data-ttu-id="33063-108">Listagem de nuvens</span><span class="sxs-lookup"><span data-stu-id="33063-108">Listing clouds</span></span>

<span data-ttu-id="33063-109">Você pode listar as nuvens disponíveis com o comando [cloud list](/cli/azure/cloud#list).</span><span class="sxs-lookup"><span data-stu-id="33063-109">You can list available clouds with the [cloud list](/cli/azure/cloud#list) command.</span></span> <span data-ttu-id="33063-110">Isso informará qual nuvem está ativa no momento, qual é seu perfil atual e dará informações sobre os nomes de host e sufixos regionais.</span><span class="sxs-lookup"><span data-stu-id="33063-110">This tells you which cloud is currently active, what its current profile is, and information on regional suffixes and host names.</span></span>

<span data-ttu-id="33063-111">Para obter a nuvem ativa e uma lista de todas as nuvens disponíveis:</span><span class="sxs-lookup"><span data-stu-id="33063-111">To get the active cloud and a list of all the available clouds:</span></span>

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

<span data-ttu-id="33063-112">A nuvem ativa no momento possui `True` na coluna `IsActive`.</span><span class="sxs-lookup"><span data-stu-id="33063-112">The currently active cloud has `True` in the `IsActive` column.</span></span> <span data-ttu-id="33063-113">Somente uma nuvem pode estar ativa em determinado momento.</span><span class="sxs-lookup"><span data-stu-id="33063-113">Only one cloud can be active at any time.</span></span> <span data-ttu-id="33063-114">Para obter informações mais detalhadas sobre uma nuvem, incluindo os pontos de extremidade que ela utiliza para os serviços do Azure, use o comando `cloud show`:</span><span class="sxs-lookup"><span data-stu-id="33063-114">To get more detailed information on a cloud, including the endpoints that it uses for Azure services, use the `cloud show` command:</span></span>

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

## <a name="switching-the-active-cloud"></a><span data-ttu-id="33063-115">Alternar a nuvem ativa</span><span class="sxs-lookup"><span data-stu-id="33063-115">Switching the active cloud</span></span>

<span data-ttu-id="33063-116">Para trocar a nuvem ativa no momento, execute o comando [cloud set](/cli/azure/cloud#set).</span><span class="sxs-lookup"><span data-stu-id="33063-116">To switch the currently active cloud, run the [cloud set](/cli/azure/cloud#set) command.</span></span> <span data-ttu-id="33063-117">Esse comando usa um argumento necessário, o nome da nuvem.</span><span class="sxs-lookup"><span data-stu-id="33063-117">This command takes one required argument, the name of the cloud.</span></span>

```azurecli
az cloud set --name AzureChinaCloud
```

> [!IMPORTANT]
> <span data-ttu-id="33063-118">Se a autenticação para a nuvem ativada tiver expirado, você precisará autenticar novamente antes de realizar outras tarefas de CLI.</span><span class="sxs-lookup"><span data-stu-id="33063-118">If your authentication for the activated cloud has expired, you need to re-authenticate before performing any other CLI tasks.</span></span> <span data-ttu-id="33063-119">Se esta for a primeira vez em que troca para a nova nuvem, você também precisará definir a assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="33063-119">If this is your first time switching to the new cloud, you also need to set the active subscription.</span></span>
> <span data-ttu-id="33063-120">Para obter instruções sobre autenticação, consulte [Fazer logon com a CLI do Azure 2.0](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="33063-120">For instructions on authenticating, see [Log in with Azure CLI 2.0](authenticate-azure-cli.md).</span></span> <span data-ttu-id="33063-121">Para obter informações sobre o gerenciamento de assinaturas, confira [Gerenciar assinaturas do Azure com a CLI do Azure 2.0](manage-azure-subscriptions-azure-cli.md)</span><span class="sxs-lookup"><span data-stu-id="33063-121">For information on subscription management, see [Manage Azure subscriptions with Azure CLI 2.0](manage-azure-subscriptions-azure-cli.md)</span></span>

## <a name="register-a-cloud"></a><span data-ttu-id="33063-122">Registrar uma nuvem</span><span class="sxs-lookup"><span data-stu-id="33063-122">Register a cloud</span></span>

<span data-ttu-id="33063-123">Registre uma nova nuvem se tiver seus próprios pontos de extremidade do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="33063-123">Register a new cloud if you have your own endpoints for Azure Stack.</span></span> <span data-ttu-id="33063-124">Uma nuvem é criado com o comando [cloud register](/cli/azure/cloud#register).</span><span class="sxs-lookup"><span data-stu-id="33063-124">Creating a cloud is done with the [cloud register](/cli/azure/cloud#register) command.</span></span> <span data-ttu-id="33063-125">Este comando requer um nome e um conjunto de recursos com pontos de extremidade associados.</span><span class="sxs-lookup"><span data-stu-id="33063-125">This command requires a name and a set of capabilities with associated endpoints.</span></span> <span data-ttu-id="33063-126">Para saber como registrar uma nuvem para usar com o Azure Stack, confira [Instalar e configurar a CLI para usar com o Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span><span class="sxs-lookup"><span data-stu-id="33063-126">To learn how to register a cloud for use with Azure Stack, see [Install and configure CLI for use with Azure Stack](/azure/azure-stack/user/azure-stack-connect-cli#connect-to-azure-stack).</span></span>

<span data-ttu-id="33063-127">Você não precisa registrar sua própria nuvem para regiões na China, Governo dos EUA ou Alemanha.</span><span class="sxs-lookup"><span data-stu-id="33063-127">You do not need to register your own cloud for China, US Government, or German regions.</span></span> <span data-ttu-id="33063-128">São gerenciadas pela Microsoft e ficam disponíveis por padrão.</span><span class="sxs-lookup"><span data-stu-id="33063-128">These are managed by Microsoft and available by default.</span></span>  <span data-ttu-id="33063-129">Para obter mais informações sobre todas as configurações do ponto de extremidade disponíveis, confira a [documentação para `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span><span class="sxs-lookup"><span data-stu-id="33063-129">For more information on all of the available endpoint settings, see the [documentation for `az cloud register`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_register).</span></span>

<span data-ttu-id="33063-130">Registrar uma nuvem não troca automaticamente para ela.</span><span class="sxs-lookup"><span data-stu-id="33063-130">Registering a cloud does not automatically switch to it.</span></span> <span data-ttu-id="33063-131">Use o comando `az cloud set` para selecionar a nuvem recém-criada, conforme descrito acima.</span><span class="sxs-lookup"><span data-stu-id="33063-131">Use the `az cloud set` command to select the newly created cloud as described above.</span></span>

## <a name="update-an-existing-cloud"></a><span data-ttu-id="33063-132">Atualizar uma nuvem existente</span><span class="sxs-lookup"><span data-stu-id="33063-132">Update an existing cloud</span></span>

<span data-ttu-id="33063-133">Se você tiver permissões, também poderá atualizar uma nuvem existente.</span><span class="sxs-lookup"><span data-stu-id="33063-133">If you have permissions, you can also update an existing cloud.</span></span> <span data-ttu-id="33063-134">Faça isso quando precisar trocar para um perfil diferente do Azure, adicionar ou alterar um ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="33063-134">Do this when you need to switch to a different Azure profile, add an endpoint, or change an endpoint.</span></span>
<span data-ttu-id="33063-135">Você faz isso com o comando `az cloud update`, que tem os mesmos argumentos de `az cloud register`.</span><span class="sxs-lookup"><span data-stu-id="33063-135">You do this with the `az cloud update` command, which takes the same arguments as `az cloud register`.</span></span> <span data-ttu-id="33063-136">Para obter mais informações, confira a [documentação para `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span><span class="sxs-lookup"><span data-stu-id="33063-136">For more information, see the [documentation for `az cloud update`](/cli/azure/cloud?view=azure-cli-latest#az_cloud_update).</span></span>

## <a name="unregister-a-cloud"></a><span data-ttu-id="33063-137">Cancelar o registro de uma nuvem</span><span class="sxs-lookup"><span data-stu-id="33063-137">Unregister a cloud</span></span>

<span data-ttu-id="33063-138">Se você não precisar de uma nuvem registrada, ela poderá ser cancelada com o comando [cloud unregister](/cli/azure/cloud#unregister):</span><span class="sxs-lookup"><span data-stu-id="33063-138">If you no longer require a registered cloud, it can be unregistered with the [cloud unregister](/cli/azure/cloud#unregister) command:</span></span>

```azurecli
az cloud unregister --name MyCloud
```
