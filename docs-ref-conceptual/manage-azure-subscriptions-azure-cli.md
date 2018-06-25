---
title: Gerenciar as assinaturas do Azure com a CLI do Azure
description: Gerenciar as assinaturas do Azure com a CLI do Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/15/2018
ms.topic: conceptual
ms.produdct: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: active-directory
ms.openlocfilehash: fdc8ffca38a6a581ae63b0518df72f6e09110d07
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262702"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="1b04c-103">Gerenciar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="1b04c-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="1b04c-104">A maioria dos usuários do Azure terá somente uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1b04c-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="1b04c-105">No entanto, se você fizer parte de várias organizações ou sua organização tiver um acesso dividido a certos recursos em agrupamentos, poderá ter várias assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="1b04c-105">However, if you are part of multiple organizations or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="1b04c-106">Várias assinaturas podem ser facilmente gerenciadas com a CLI definindo uma assinatura global para todos os comandos, ou selecionando uma assinatura em uma base por comando.</span><span class="sxs-lookup"><span data-stu-id="1b04c-106">Multiple subscriptions can be easily managed with the CLI either by setting a global subscription for all commands, or selecting a subscription on a per-command basis.</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="1b04c-107">Locatários, usuários e assinaturas</span><span class="sxs-lookup"><span data-stu-id="1b04c-107">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="1b04c-108">Talvez você tenha alguma confusão sobre a diferença entre locatários, usuários e assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="1b04c-108">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="1b04c-109">Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização.</span><span class="sxs-lookup"><span data-stu-id="1b04c-109">A _tenant_ is the Azure Active Directory entity which encompasses a whole organization.</span></span> <span data-ttu-id="1b04c-110">Esse locatário tem pelo menos uma _assinatura_ e _usuário_.</span><span class="sxs-lookup"><span data-stu-id="1b04c-110">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="1b04c-111">Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence.</span><span class="sxs-lookup"><span data-stu-id="1b04c-111">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="1b04c-112">Os usuários são as contas que fazem logon no Azure para provisionar e usar os recursos.</span><span class="sxs-lookup"><span data-stu-id="1b04c-112">Users are those accounts which log in to Azure to provision and use resources.</span></span>
<span data-ttu-id="1b04c-113">Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="1b04c-113">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="1b04c-114">Cada recurso é associado a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="1b04c-114">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="1b04c-115">Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="1b04c-115">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="1b04c-116">Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como adicionar uma assinatura do Azure ao Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="1b04c-116">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="1b04c-117">Ao trabalhar com vários locatários, talvez seja necessário entrar em um locatário específico.</span><span class="sxs-lookup"><span data-stu-id="1b04c-117">When working with multiple tenants, you may need to sign in to a specific tenant.</span></span> <span data-ttu-id="1b04c-118">Para isso, confira [Entrar com a CLI do Azure](/cli/azure/authenticate-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="1b04c-118">To do this, see [Sign in with Azure CLI](/cli/azure/authenticate-azure-cli).</span></span>

## <a name="work-with-multiple-subscriptions"></a><span data-ttu-id="1b04c-119">Como trabalhar com várias assinaturas</span><span class="sxs-lookup"><span data-stu-id="1b04c-119">Work with multiple subscriptions</span></span>

<span data-ttu-id="1b04c-120">Para acessar os recursos contidos em uma assinatura, você precisa trocar sua assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="1b04c-120">To access the resources contained within a subscription, you need to switch your active subscription.</span></span> <span data-ttu-id="1b04c-121">A alternância de sua assinatura pode ser feita para todos os comandos da CLI do Azure com [az account set](/cli/azure/account#az-account-set), ou feita por uma base por comando usando o argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="1b04c-121">Switching your subscription can be done for all Azure CLI commands with [az account set](/cli/azure/account#az-account-set), or done on a per-command basis by using the `--subscription` argument.</span></span>

<span data-ttu-id="1b04c-122">Para começar, você precisará de uma lista de suas assinaturas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1b04c-122">To start, you will need a list of your available subscriptions.</span></span> <span data-ttu-id="1b04c-123">Para obter, use o comando [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="1b04c-123">To get it, use the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli-interactive
az account list --output table
```

<span data-ttu-id="1b04c-124">Para alterar a assinatura ativa globalmente, use `az account set` junto com a ID da assinatura ou o nome da assinatura:</span><span class="sxs-lookup"><span data-stu-id="1b04c-124">To change the active subscription globally, use `az account set` along with either the subscription ID or subscription name:</span></span>

```azurecli-interactive
az account set --subscription "My Demos"
```

<span data-ttu-id="1b04c-125">Para usar uma assinatura específica para um comando, use o argumento `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="1b04c-125">To use a specific subscription for a command, just use the `--subscription` argument.</span></span> <span data-ttu-id="1b04c-126">Esse argumento tem uma ID da assinatura ou o nome da assinatura:</span><span class="sxs-lookup"><span data-stu-id="1b04c-126">This argument takes either a subscription ID or subscription name:</span></span>

```azurecli-interactive
az vm create --subscription "My Demos" --resource-group MyGroup --name NewVM --image Ubuntu
```
