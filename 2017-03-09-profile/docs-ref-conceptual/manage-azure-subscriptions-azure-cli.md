---
title: Gerenciar as assinaturas do Azure com a CLI do Azure 2.0
description: Gerencie as assinaturas do Azure com a CLI 2.0 no Linux, Mac ou Windows.
keywords: Assinatura da CLI do Azure 2.0, Linux, Mac, Windows, OS X
author: kamaljit
ms.author: sttramer
manager: routlaw
ms.date: 10/30/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 98fb955e-6dbf-47e2-80ac-170d6d95cb70
ms.openlocfilehash: 0f453ad1bff621250c8aa3147b5f5e916e712e30
ms.sourcegitcommit: 16426a08c0f2f62d0b9dca3df8132cece659acff
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/21/2017
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="3a7fb-104">Gerenciar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="3a7fb-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="3a7fb-105">A maioria dos usuários do Azure terá somente uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-105">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="3a7fb-106">No entanto, se você fizer parte de várias organizações ou sua organização tiver um acesso dividido a certos recursos em agrupamentos, poderá ter várias assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-106">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="3a7fb-107">Várias assinaturas podem ser facilmente gerenciadas com a CLI e as operações podem ser executadas selecionando uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-107">Multiple subscriptions can be easily managed with the CLI, and operations can be performed by selecting a subscription.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="3a7fb-108">Locatários, usuários e assinaturas</span><span class="sxs-lookup"><span data-stu-id="3a7fb-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="3a7fb-109">Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="3a7fb-110">Em geral, um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-110">In general, a _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="3a7fb-111">Esse locatário tem pelo menos uma _assinatura_ e _usuário_.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="3a7fb-112">Um usuário é um indivíduo e é associado a somente um locatário, a organização à qual pertence.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-112">A user is an individual, and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="3a7fb-113">Os usuários são as contas que fazem logon no Azure para provisionar e usar os recursos.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-113">Users are those accounts which log in to Azure to provision and use resources.</span></span> <span data-ttu-id="3a7fb-114">Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="3a7fb-115">Cada recurso é associado a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="3a7fb-116">Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="3a7fb-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
<span data-ttu-id="3a7fb-117">Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="3a7fb-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>

## <a name="working-with-multiple-subscriptions"></a><span data-ttu-id="3a7fb-118">Trabalhando com várias assinaturas</span><span class="sxs-lookup"><span data-stu-id="3a7fb-118">Working with multiple subscriptions</span></span>

<span data-ttu-id="3a7fb-119">Para acessar os recursos contidos em uma assinatura, você precisa trocar sua assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-119">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="3a7fb-120">Todo o trabalho com assinaturas é feito por meio do comando `az account`, que se refere ao contrato de serviço que representa uma assinatura, não à conta individual.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-120">All work with subscriptions is done through the `az account` command, which refers to the service agreement that a subscription represents and not your individual account.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

<span data-ttu-id="3a7fb-121">Para começar a trabalhar com suas assinaturas disponíveis, obtenha uma lista das disponíveis em sua conta:</span><span class="sxs-lookup"><span data-stu-id="3a7fb-121">To start working with your available subscriptions, get a list of those available in your account:</span></span>

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

<span data-ttu-id="3a7fb-122">Para alterar a assinatura ativa, você pode usar `az account set`:</span><span class="sxs-lookup"><span data-stu-id="3a7fb-122">In order to change the active subscription, you can use `az account set`:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="3a7fb-123">É possível pode usar a ID da assinatura ou o nome da assinatura para selecioná-la.</span><span class="sxs-lookup"><span data-stu-id="3a7fb-123">You can use either the subscription ID or the subscription name to select the subscription.</span></span>
