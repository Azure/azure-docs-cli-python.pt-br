---
title: Gerenciar assinaturas do Azure com a CLI do Azure
description: Gerencie as assinaturas do Azure com a CLI do Azure.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/09/2018
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: dad217dff159baa39bd1361258fb308eea872564
ms.sourcegitcommit: ee64dc738cfe689a2a479e32a87bf420f96c31c8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2020
ms.locfileid: "77780053"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="1fc62-103">Usar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="1fc62-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="1fc62-104">A maioria dos usuários do Azure terá somente uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1fc62-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="1fc62-105">No entanto, se você fizer parte de mais de uma organização ou se sua organização tiver dividido o acesso a determinados recursos nos agrupamentos, poderá ter várias assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="1fc62-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="1fc62-106">A CLI é compatível com a escolha de uma assinatura globalmente e por comando.</span><span class="sxs-lookup"><span data-stu-id="1fc62-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="1fc62-107">Para obter informações detalhadas sobre assinaturas, cobrança e gerenciamento de custos, confira a [documentação sobre cobrança e gerenciamento de custos](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="1fc62-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="1fc62-108">Locatários, usuários e assinaturas</span><span class="sxs-lookup"><span data-stu-id="1fc62-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="1fc62-109">Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="1fc62-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="1fc62-110">Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização.</span><span class="sxs-lookup"><span data-stu-id="1fc62-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="1fc62-111">Esse locatário tem pelo menos uma _assinatura_ e _usuário_.</span><span class="sxs-lookup"><span data-stu-id="1fc62-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="1fc62-112">Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence.</span><span class="sxs-lookup"><span data-stu-id="1fc62-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="1fc62-113">Os usuários são as contas que se conectam ao Azure para criar, gerenciar e usar recursos.</span><span class="sxs-lookup"><span data-stu-id="1fc62-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="1fc62-114">Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="1fc62-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="1fc62-115">Cada recurso é associado a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1fc62-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="1fc62-116">Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="1fc62-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="1fc62-117">Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="1fc62-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="1fc62-118">Para saber como entrar em um locatário específico, confira [Entrar com a CLI do Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="1fc62-118">To learn how to sign in to a specific tenant, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="1fc62-119">Alterar a assinatura ativa</span><span class="sxs-lookup"><span data-stu-id="1fc62-119">Change the active subscription</span></span>

<span data-ttu-id="1fc62-120">Para acessar os recursos de uma assinatura, você precisa trocar sua assinatura ativa ou usar o argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="1fc62-120">To access the resources for a subscription, switch your active subscription or use the `--subscription` argument.</span></span> <span data-ttu-id="1fc62-121">A troca da assinatura de todos os comandos é feita com [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="1fc62-121">Switching your subscription for all commands is done with [az account set](/cli/azure/account#az-account-set).</span></span>

<span data-ttu-id="1fc62-122">Para trocar sua assinatura ativa:</span><span class="sxs-lookup"><span data-stu-id="1fc62-122">To switch your active subscription:</span></span>

1. <span data-ttu-id="1fc62-123">Obtenha a lista de assinaturas usando o comando [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="1fc62-123">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

    ```azurecli-interactive
    az account list --output table
    ```
2. <span data-ttu-id="1fc62-124">Use `az account set` com a ID da assinatura ou nome para o qual você deseja alterar.</span><span class="sxs-lookup"><span data-stu-id="1fc62-124">Use `az account set` with the subscription ID or name you want to switch to.</span></span>

    ```azurecli-interactive
    az account set --subscription "My Demos"
    ```

<span data-ttu-id="1fc62-125">Para executar apenas um único comando com uma assinatura diferente, use o argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="1fc62-125">To run only a single command with a different subscription, use the `--subscription` argument.</span></span> <span data-ttu-id="1fc62-126">Esse argumento tem uma ID da assinatura ou o nome da assinatura:</span><span class="sxs-lookup"><span data-stu-id="1fc62-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
