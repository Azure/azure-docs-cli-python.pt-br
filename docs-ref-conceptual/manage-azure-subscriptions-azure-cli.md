---
title: Gerenciar as assinaturas do Azure com a CLI do Azure 2.0
description: Gerencie as assinaturas do Azure com a CLI 2.0 no Linux, Mac ou Windows.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/30/2017
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: ee7e0ca03b1ed9c1bfc040fd5714bb9b3549e3cd
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2018
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="2758b-103">Gerenciar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="2758b-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="2758b-104">A maioria dos usuários do Azure terá somente uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2758b-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="2758b-105">No entanto, se você fizer parte de várias organizações ou sua organização tiver um acesso dividido a certos recursos em agrupamentos, poderá ter várias assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="2758b-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="2758b-106">Várias assinaturas podem ser facilmente gerenciadas com a CLI e as operações podem ser executadas selecionando uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2758b-106">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="2758b-107">Locatários, usuários e assinaturas</span><span class="sxs-lookup"><span data-stu-id="2758b-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="2758b-108">Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="2758b-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="2758b-109">Em geral, um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização.</span><span class="sxs-lookup"><span data-stu-id="2758b-109">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="2758b-110">Esse locatário tem pelo menos uma _assinatura_ e _usuário_.</span><span class="sxs-lookup"><span data-stu-id="2758b-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="2758b-111">Um usuário é um indivíduo e é associado a somente um locatário, a organização à qual pertence.</span><span class="sxs-lookup"><span data-stu-id="2758b-111">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="2758b-112">Os usuários são as contas que fazem logon no Azure para provisionar e usar os recursos.</span><span class="sxs-lookup"><span data-stu-id="2758b-112">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="2758b-113">Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="2758b-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="2758b-114">Cada recurso é associado a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="2758b-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="2758b-115">Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="2758b-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="2758b-116">Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="2758b-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="2758b-117">Ao trabalhar com vários locatários, talvez seja necessário fazer logon em um locatário específico.</span><span class="sxs-lookup"><span data-stu-id="2758b-117">When working with multiple tenants, you may need to log into a specific tenant.</span></span> <span data-ttu-id="2758b-118">Para isso, consulte [Fazer logon com a CLI do Azure 2.0](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="2758b-118">To do this, see [Log in with Azure CLI 2.0](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="2758b-119">Trabalhando com várias assinaturas</span><span class="sxs-lookup"><span data-stu-id="2758b-119">Working with multiple subscriptions</span></span>

<span data-ttu-id="2758b-120">Para acessar os recursos contidos em uma assinatura, você precisa trocar sua assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="2758b-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="2758b-121">Todo o trabalho com assinaturas é feito por meio do comando `az account`, que se refere ao contrato de serviço que representa uma assinatura, não à conta individual.</span><span class="sxs-lookup"><span data-stu-id="2758b-121">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="2758b-122">Para começar a trabalhar com suas assinaturas disponíveis, obtenha uma lista das disponíveis em sua conta:</span><span class="sxs-lookup"><span data-stu-id="2758b-122">To start working with your available subscriptions, get a list of those available in your account:</span></span>

```azurecli-interactive
az account list --output table
```

```Output
Name                                         CloudName    SubscriptionId                        State     IsDefault
-------------------------------------------  -----------  ------------------------------------  --------  -----------
My Production Subscription                   AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
My DevTest Subscription                      AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled   True
My Demos                                     AzureCloud   XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX  Enabled
```

<span data-ttu-id="2758b-123">Para alterar a assinatura ativa, você pode usar `az account set`:</span><span class="sxs-lookup"><span data-stu-id="2758b-123">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="2758b-124">É possível pode usar a ID da assinatura ou o nome da assinatura para selecioná-la.</span><span class="sxs-lookup"><span data-stu-id="2758b-124">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
