---
title: Gerenciar assinaturas do Azure com a CLI do Azure
description: Saiba mais sobre locatários, usuários e assinaturas do Azure. Use a CLI do Azure para gerenciar suas assinaturas, criar grupos de gerenciamento e bloquear assinaturas.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/29/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 6a980c45627c79c9e3f8c6c920944cc3dc62281f
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99495220"
---
# <a name="use-azure-subscriptions-with-azure-cli"></a><span data-ttu-id="0462a-104">Usar assinaturas do Azure com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0462a-104">Use Azure subscriptions with Azure CLI</span></span>

<span data-ttu-id="0462a-105">Você pode ter várias assinaturas no Azure.</span><span class="sxs-lookup"><span data-stu-id="0462a-105">You might have multiple subscriptions within Azure.</span></span> <span data-ttu-id="0462a-106">Você pode fazer parte de mais de uma organização ou sua organização pode dividir o acesso a determinados recursos entre agrupamentos.</span><span class="sxs-lookup"><span data-stu-id="0462a-106">You can be part of more than one organization or your organization might divide access to certain resources across groupings.</span></span> <span data-ttu-id="0462a-107">A CLI do Azure dá suporte à seleção de uma assinatura globalmente e por comando.</span><span class="sxs-lookup"><span data-stu-id="0462a-107">The Azure CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="0462a-108">Para obter informações detalhadas sobre assinaturas, cobrança e gerenciamento de custos, confira a [documentação sobre cobrança e gerenciamento de custos](/azure/billing/).</span><span class="sxs-lookup"><span data-stu-id="0462a-108">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="0462a-109">Locatários, usuários e assinaturas</span><span class="sxs-lookup"><span data-stu-id="0462a-109">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="0462a-110">Um _locatário_ é a entidade do Azure Active Directory que abrange toda a organização.</span><span class="sxs-lookup"><span data-stu-id="0462a-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="0462a-111">Um locatário tem uma ou mais _assinaturas_ e _usuários_.</span><span class="sxs-lookup"><span data-stu-id="0462a-111">A tenant has one or more _subscription_ and _user_.</span></span> <span data-ttu-id="0462a-112">Um usuário é um indivíduo e é associado a somente um locatário: a organização à qual pertence.</span><span class="sxs-lookup"><span data-stu-id="0462a-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="0462a-113">Os usuários são as contas que se conectam ao Azure para criar, gerenciar e usar recursos.</span><span class="sxs-lookup"><span data-stu-id="0462a-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span> <span data-ttu-id="0462a-114">Um usuário pode ter acesso a várias _assinaturas_, que são contratos com a Microsoft para usar os serviços de nuvem, incluindo o Azure.</span><span class="sxs-lookup"><span data-stu-id="0462a-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="0462a-115">Cada recurso é associado a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0462a-115">Every resource is associated with a subscription.</span></span>

* <span data-ttu-id="0462a-116">Para saber mais sobre as diferenças entre locatários, usuários e assinaturas, confira o [dicionário de terminologia de nuvem do Azure](/azure/azure-glossary-cloud-terminology).</span><span class="sxs-lookup"><span data-stu-id="0462a-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>
* <span data-ttu-id="0462a-117">Para saber como adicionar uma nova assinatura ao seu locatário do Azure Active Directory, confira [Como associar ou adicionar uma assinatura do Azure ao locatário do Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="0462a-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [Associate or add an Azure subscription to your Azure Active Directory tenant](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
* <span data-ttu-id="0462a-118">Para saber como entrar em um locatário específico, confira [Entrar com a CLI do Azure](./authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="0462a-118">To learn how to sign in to a specific tenant, see [Sign in with the Azure CLI](./authenticate-azure-cli.md).</span></span>

## <a name="commands-in-a-subscription"></a><span data-ttu-id="0462a-119">Comandos em uma assinatura</span><span class="sxs-lookup"><span data-stu-id="0462a-119">Commands in a subscription</span></span>

<span data-ttu-id="0462a-120">Muitos comandos da CLI do Azure funcionam em uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0462a-120">Many Azure CLI commands act within a subscription.</span></span> <span data-ttu-id="0462a-121">Você sempre pode especificar em qual assinatura deseja trabalhar usando o parâmetro **subscription** no comando.</span><span class="sxs-lookup"><span data-stu-id="0462a-121">You can always specify which subscription to work in by using the **subscription** parameter in your command.</span></span> <span data-ttu-id="0462a-122">Esse parâmetro é opcional.</span><span class="sxs-lookup"><span data-stu-id="0462a-122">That parameter is optional.</span></span> <span data-ttu-id="0462a-123">Se você não especificar uma assinatura, o comando usará sua assinatura ativa atual.</span><span class="sxs-lookup"><span data-stu-id="0462a-123">If you don't specify a subscription, the command uses your current, active subscription.</span></span>

<span data-ttu-id="0462a-124">Para ver a assinatura que você está usando no momento, execute o comando [az account show](/cli/azure/account#az_account_show):</span><span class="sxs-lookup"><span data-stu-id="0462a-124">To see the subscription you're currently using, run the [az account show](/cli/azure/account#az_account_show) command:</span></span>

```azurecli
az account show --output table
```

> [!TIP]
> <span data-ttu-id="0462a-125">O parâmetro `--output` é um parâmetro global, disponível para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="0462a-125">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="0462a-126">O valor **table** apresenta a saída em um formato amigável.</span><span class="sxs-lookup"><span data-stu-id="0462a-126">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="0462a-127">Para obter mais informações, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="0462a-127">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="0462a-128">As assinaturas contêm grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="0462a-128">Subscriptions contain resource groups.</span></span> <span data-ttu-id="0462a-129">Um grupo de recursos do Azure é um contêiner que mantém os recursos relacionados a uma solução do Azure.</span><span class="sxs-lookup"><span data-stu-id="0462a-129">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="0462a-130">Se o comando funcionar com os recursos na sua assinatura ativa, você não precisará especificar `--subscription`.</span><span class="sxs-lookup"><span data-stu-id="0462a-130">If your command works with resources in your active subscription, you don't need to specify `--subscription`.</span></span>

<span data-ttu-id="0462a-131">Esse comando cria uma conta de armazenamento no grupo de recursos especificado:</span><span class="sxs-lookup"><span data-stu-id="0462a-131">This command creates a storage account in the specified resource group:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 \
    --location eastus --sku Standard_LRS
```

<span data-ttu-id="0462a-132">Se o grupo de armazenamento não fizer parte da sua assinatura ativa atual, esse comando falhará.</span><span class="sxs-lookup"><span data-stu-id="0462a-132">If the storage group isn't part of your current active subscription, this command fails.</span></span>

<span data-ttu-id="0462a-133">Se necessário, altere a assinatura ativa, conforme descrito na próxima seção, ou especifique a assinatura no comando:</span><span class="sxs-lookup"><span data-stu-id="0462a-133">If necessary, change the active subscription, as described in the next section, or specify the subscription in the command:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --subscription "My Demos" \
    --name storage136 --location eastus --sku Standard_LRS
```

## <a name="change-the-active-subscription"></a><span data-ttu-id="0462a-134">Alterar a assinatura ativa</span><span class="sxs-lookup"><span data-stu-id="0462a-134">Change the active subscription</span></span>

<span data-ttu-id="0462a-135">Altere sua assinatura ativa usando o comando [az account set](/cli/azure/account#az-account-set).</span><span class="sxs-lookup"><span data-stu-id="0462a-135">You can change your active subscription by using the [az account set](/cli/azure/account#az-account-set) command.</span></span>

<span data-ttu-id="0462a-136">Obtenha a lista de assinaturas usando o comando [az account list](/cli/azure/account#az-account-list):</span><span class="sxs-lookup"><span data-stu-id="0462a-136">Get a list of your subscriptions with the [az account list](/cli/azure/account#az-account-list) command:</span></span>

```azurecli
az account list --output table
```

<span data-ttu-id="0462a-137">Esse comando lista todas as assinaturas que você pode acessar.</span><span class="sxs-lookup"><span data-stu-id="0462a-137">This command lists all the subscriptions you can access.</span></span> <span data-ttu-id="0462a-138">Sua assinatura ativa é marcada como `True` na coluna `IsDefault`.</span><span class="sxs-lookup"><span data-stu-id="0462a-138">Your active subscription is marked as `True` in the `IsDefault` column.</span></span> <span data-ttu-id="0462a-139">Se você não vir uma assinatura esperada, adicione o parâmetro `--refresh` para obter a lista mais atual de assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0462a-139">If you don't see a subscription you expect, add the `--refresh` parameter to get the most current list of subscriptions.</span></span>

<span data-ttu-id="0462a-140">Para alternar para outra assinatura, use [az account set](/cli/azure/account#az-account-set) com a ID da assinatura ou o nome para o qual deseja alternar.</span><span class="sxs-lookup"><span data-stu-id="0462a-140">To switch to a different subscription, use [az account set](/cli/azure/account#az-account-set) with the subscription ID or name you want to switch to.</span></span>

```azurecli
az account set --subscription "My Demos"
```

<span data-ttu-id="0462a-141">Suas assinaturas têm um nome e uma ID, que é um GUID.</span><span class="sxs-lookup"><span data-stu-id="0462a-141">Your subscriptions have both a name and an ID, which is a GUID.</span></span> <span data-ttu-id="0462a-142">Você pode usar um desses comandos.</span><span class="sxs-lookup"><span data-stu-id="0462a-142">You can use either for these commands.</span></span> <span data-ttu-id="0462a-143">Se você usar um nome que inclua espaços, use aspas.</span><span class="sxs-lookup"><span data-stu-id="0462a-143">If you use a name that includes spaces, use quotation marks.</span></span>

<span data-ttu-id="0462a-144">Se você executar o comando [az account list](/cli/azure/account#az-account-list) novamente, a coluna `IsDefault` mostrará sua assinatura ativa atual.</span><span class="sxs-lookup"><span data-stu-id="0462a-144">If you run the [az account list](/cli/azure/account#az-account-list) command again, the `IsDefault` column shows your current active subscription.</span></span>

## <a name="create-management-groups"></a><span data-ttu-id="0462a-145">Criar grupos de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="0462a-145">Create management groups</span></span>

<span data-ttu-id="0462a-146">Os grupos de gerenciamento do Azure contêm assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0462a-146">Azure management groups contain subscriptions.</span></span> <span data-ttu-id="0462a-147">Os grupos de gerenciamento fornecem uma forma de gerenciar o acesso, as políticas e a conformidade para essas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="0462a-147">Management groups provide a way to manage access, policies, and compliance for those subscriptions.</span></span> <span data-ttu-id="0462a-148">Para obter mais informações, confira [O que são grupos de gerenciamento do Azure](/azure/governance/management-groups/overview).</span><span class="sxs-lookup"><span data-stu-id="0462a-148">For more information, see [What are Azure management groups](/azure/governance/management-groups/overview).</span></span>

<span data-ttu-id="0462a-149">Use os comandos [az account management-group](/cli/azure/account/management-group) para criar e gerenciar os grupos de gerenciamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="0462a-149">Use the [az account management-group](/cli/azure/account/management-group) commands to create and manage Azure Management Groups.</span></span>

<span data-ttu-id="0462a-150">Crie um grupo de gerenciamento para várias das suas assinaturas usando o comando [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create):</span><span class="sxs-lookup"><span data-stu-id="0462a-150">You can create a management group for several of your subscriptions by using the [az account management-group create](/cli/azure/account/management-group#az_account_management_group_create) command:</span></span>

```azurecli
az account management-group create --name Contoso01
```

<span data-ttu-id="0462a-151">Para ver todos os seus grupos de gerenciamento, use o comando [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list):</span><span class="sxs-lookup"><span data-stu-id="0462a-151">To see all your management groups, use the [az account management-group list](/cli/azure/account/management-group#az_account_management_group_list) command:</span></span>

```azurecli
az account management-group list
```

<span data-ttu-id="0462a-152">Adicione assinaturas ao novo grupo usando o comando [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add):</span><span class="sxs-lookup"><span data-stu-id="0462a-152">Add subscriptions to your new group by using the [az account management-group subscription add](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_add) command:</span></span>

```azurecli
az account management-group subscription add --name Contoso01 --subscription "My Demos"
az account management-group subscription add --name Contoso01 --subscription "My Second Demos"
```

<span data-ttu-id="0462a-153">Para remover uma assinatura, use o comando [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove):</span><span class="sxs-lookup"><span data-stu-id="0462a-153">To remove a subscription, use the [az account management-group subscription remove](/cli/azure/account/management-group/subscription#az_account_management_group_subscription_remove) command:</span></span>

```azurecli
az account management-group subscription remove --name Contoso01 --subscription "My Demos"
```

<span data-ttu-id="0462a-154">Para remover um grupo de gerenciamento, execute o comando [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete):</span><span class="sxs-lookup"><span data-stu-id="0462a-154">To remove a management group, run the [az account management-group delete](/cli/azure/account/management-group#az_account_management_group_delete) command:</span></span>

```azurecli
az account management-group delete --name Contoso01
```

<span data-ttu-id="0462a-155">A remoção de uma assinatura ou a exclusão de um grupo de gerenciamento não exclui nem desativa uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0462a-155">Removing a subscription or deleting a management group doesn't delete or deactivate a subscription.</span></span>

## <a name="set-a-subscription-lock"></a><span data-ttu-id="0462a-156">Definir um bloqueio de assinatura</span><span class="sxs-lookup"><span data-stu-id="0462a-156">Set a subscription lock</span></span>

<span data-ttu-id="0462a-157">Como administrador, você poderá precisar bloquear uma assinatura para impedir que os usuários a excluam ou modifiquem.</span><span class="sxs-lookup"><span data-stu-id="0462a-157">As an administrator, you may need to lock a subscription to prevent users from deleting or modifying it.</span></span> <span data-ttu-id="0462a-158">Para obter mais informações, confira [Bloquear recursos para impedir alterações inesperadas](/azure/azure-resource-manager/management/lock-resources).</span><span class="sxs-lookup"><span data-stu-id="0462a-158">For more information, see [Lock resources to prevent unexpected changes](/azure/azure-resource-manager/management/lock-resources).</span></span>

<span data-ttu-id="0462a-159">Na CLI do Azure, use os comandos [az account lock](/cli/azure/account/lock).</span><span class="sxs-lookup"><span data-stu-id="0462a-159">In Azure CLI, use the [az account lock](/cli/azure/account/lock) commands.</span></span> <span data-ttu-id="0462a-160">Por exemplo, o comando [az account lock create](/cli/azure/account/lock#az_account_lock_create) pode impedir que os usuários excluam uma assinatura:</span><span class="sxs-lookup"><span data-stu-id="0462a-160">For instance, the [az account lock create](/cli/azure/account/lock#az_account_lock_create) command can prevent users from deleting a subscription:</span></span>

```azurecli
az account lock create --name "Cannot delete subscription" --lock-type CanNotDelete
```

> [!NOTE]
> <span data-ttu-id="0462a-161">Você precisa ter as permissões apropriadas para criar ou alterar os bloqueios.</span><span class="sxs-lookup"><span data-stu-id="0462a-161">You need to have appropriate permissions to create or change locks.</span></span>

<span data-ttu-id="0462a-162">Para ver os bloqueios atuais na sua assinatura, use o comando [az account lock list](/cli/azure/account/lock#az_account_lock_list):</span><span class="sxs-lookup"><span data-stu-id="0462a-162">To see the current locks on your subscription, use the [az account lock list](/cli/azure/account/lock#az_account_lock_list) command:</span></span>

```azurecli
az account lock list --output table
```

<span data-ttu-id="0462a-163">Se você tornar uma conta somente leitura, o resultado será semelhante a atribuir permissões da função Leitor a todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="0462a-163">If you make an account read-only, the result resembles assigning permissions of the Reader role to all users.</span></span> <span data-ttu-id="0462a-164">Para saber mais sobre como definir permissões para funções e usuários individuais, confira [Adicionar ou remover atribuições de função do Azure usando a CLI do Azure](/azure/role-based-access-control/role-assignments-cli).</span><span class="sxs-lookup"><span data-stu-id="0462a-164">To learn about setting permissions for individual users and roles, see [Add or remove Azure role assignments using Azure CLI](/azure/role-based-access-control/role-assignments-cli).</span></span>

<span data-ttu-id="0462a-165">Para ver os detalhes de um bloqueio, use o comando [az account lock show](/cli/azure/account/lock#az_account_lock_show):</span><span class="sxs-lookup"><span data-stu-id="0462a-165">To see details for a lock, use the [az account lock show](/cli/azure/account/lock#az_account_lock_show) command:</span></span>

```azurecli
az account lock show --name "Cannot delete subscription"
```

<span data-ttu-id="0462a-166">Você pode remover um bloqueio usando o comando [az account lock delete](/cli/azure/account/lock#az_account_lock_delete):</span><span class="sxs-lookup"><span data-stu-id="0462a-166">You can remove a lock by using the [az account lock delete](/cli/azure/account/lock#az_account_lock_delete) command:</span></span>

```azurecli
az account lock delete --name "Cannot delete subscription"
```

## <a name="see-also"></a><span data-ttu-id="0462a-167">Confira também</span><span class="sxs-lookup"><span data-stu-id="0462a-167">See also</span></span>

* [<span data-ttu-id="0462a-168">Dicionário de terminologia de nuvem do Azure</span><span class="sxs-lookup"><span data-stu-id="0462a-168">Azure cloud terminology dictionary</span></span>](/azure/azure-glossary-cloud-terminology)
* [<span data-ttu-id="0462a-169">Associar ou adicionar uma assinatura do Azure ao seu locatário do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0462a-169">Associate or add an Azure subscription to your Azure Active Directory tenant</span></span>](/azure/active-directory/active-directory-how-subscriptions-associated-directory)
* [<span data-ttu-id="0462a-170">Entrar com a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="0462a-170">Sign in with Azure CLI</span></span>](./authenticate-azure-cli.md)
