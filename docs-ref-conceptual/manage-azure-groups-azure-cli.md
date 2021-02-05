---
title: Gerenciar grupos de recursos do Azure com a CLI do Azure
description: Saiba mais sobre os grupos de recursos do Azure e o uso da CLI do Azure para gerenciá-los. Saiba mais sobre os grupos de recursos persistentes e padrão.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/15/2021
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.custom: devx-track-azurecli
ms.openlocfilehash: 22167bf3d0e1d3356ebf4a1a9854bab9d5476051
ms.sourcegitcommit: 3e79897e0aeca4d74bc8ff0410121b011b5884ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "99496074"
---
# <a name="working-with-resource-groups-in-azure-cli"></a><span data-ttu-id="d06ac-104">Como trabalhar com grupos de recursos na CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d06ac-104">Working with resource groups in Azure CLI</span></span>

<span data-ttu-id="d06ac-105">Um grupo de recursos do Azure é um contêiner que mantém os recursos relacionados a uma solução do Azure.</span><span class="sxs-lookup"><span data-stu-id="d06ac-105">An Azure resource group is a container that holds related resources for an Azure solution.</span></span> <span data-ttu-id="d06ac-106">Um grupo de recursos pode conter armazenamento, máquinas virtuais, aplicativos, painéis, serviços ou quase tudo o que você usa no Azure.</span><span class="sxs-lookup"><span data-stu-id="d06ac-106">A resource group might contain storage, virtual machines, apps, dashboards, services, or almost anything you deal with in Azure.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="d06ac-107">Criar um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="d06ac-107">Create a resource group</span></span>

<span data-ttu-id="d06ac-108">Para criar um grupo de recursos, use o comando [az group create](/cli/azure/group#az_group_create):</span><span class="sxs-lookup"><span data-stu-id="d06ac-108">To create a resource group, use the [az group create](/cli/azure/group#az_group_create) command:</span></span>

```azurecli
az group create --name MyResourceGroup --location eastus
```

<span data-ttu-id="d06ac-109">Um grupo de recursos pertence a uma só localização.</span><span class="sxs-lookup"><span data-stu-id="d06ac-109">A resource group belongs to a single location.</span></span> <span data-ttu-id="d06ac-110">Para ver todas as localizações com suporte na sua assinatura atual, execute o comando [az account list-locations](/cli/azure/account#az_account_list_locations):</span><span class="sxs-lookup"><span data-stu-id="d06ac-110">To see all the locations supported in your current subscription, run the [az account list-locations](/cli/azure/account#az_account_list_locations) command:</span></span>

```azurecli
az account list-locations
```

<span data-ttu-id="d06ac-111">Para ver todos os grupos de recursos para a sua assinatura atual, use o comando [az group list](/cli/azure/group#az_group_list):</span><span class="sxs-lookup"><span data-stu-id="d06ac-111">To see all the resource groups for your current subscription, use the [az group list](/cli/azure/group#az_group_list) command:</span></span>

```azurecli
az group list --output table
```

> [!TIP]
> <span data-ttu-id="d06ac-112">O parâmetro `--output` é um parâmetro global, disponível para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-112">The `--output` parameter is a global parameter, available for all commands.</span></span> <span data-ttu-id="d06ac-113">O valor **table** apresenta a saída em um formato amigável.</span><span class="sxs-lookup"><span data-stu-id="d06ac-113">The **table** value presents output in a friendly format.</span></span> <span data-ttu-id="d06ac-114">Para obter mais informações, confira [Formatos de saída para comandos da CLI do Azure](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="d06ac-114">For more information, see [Output formats for Azure CLI commands](/cli/azure/format-output-azure-cli).</span></span>

<span data-ttu-id="d06ac-115">Ao criar um recurso, você o cria em um grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-115">When you create a resource, you create it in a resource group.</span></span> <span data-ttu-id="d06ac-116">O seguinte exemplo mostra a criação de uma conta de armazenamento com o comando [az storage account create](/cli/azure/storage/account#az_storage_account_create):</span><span class="sxs-lookup"><span data-stu-id="d06ac-116">The following example shows a storage account created by using the [az storage account create](/cli/azure/storage/account#az_storage_account_create) command:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage134 --location eastus --sku Standard_LRS
```

<span data-ttu-id="d06ac-117">Para remover um grupo de recursos, execute o comando [az group delete](/cli/azure/group#az_group_delete):</span><span class="sxs-lookup"><span data-stu-id="d06ac-117">To remove a resource group, run the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
```

<span data-ttu-id="d06ac-118">Ao remover um grupo de recursos, você exclui todos os recursos que pertencem a ele.</span><span class="sxs-lookup"><span data-stu-id="d06ac-118">When you remove a resource group, you delete all the resources that belong to it.</span></span> <span data-ttu-id="d06ac-119">Não há nenhuma opção para restaurar os recursos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-119">There's no option to undelete resources.</span></span> <span data-ttu-id="d06ac-120">Se você testar um dos comandos deste artigo, a exclusão dos grupos de recursos criados limpará a sua conta.</span><span class="sxs-lookup"><span data-stu-id="d06ac-120">If you try any of the commands in this article, deleting the resource groups you create cleans up your account.</span></span>

## <a name="persist-a-resource-group"></a><span data-ttu-id="d06ac-121">Persistir um grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="d06ac-121">Persist a resource group</span></span>

<span data-ttu-id="d06ac-122">A persistência de parâmetro permite que você reutilize valores para determinados parâmetros, incluindo grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-122">Parameter persistence allows you to reuse values for certain parameters, including resource groups.</span></span>

<span data-ttu-id="d06ac-123">Primeiro, ative o recurso de persistência usando o comando [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on):</span><span class="sxs-lookup"><span data-stu-id="d06ac-123">First, turn on the persistence feature by using the [az config param-persist on](/cli/azure/config/param-persist#az_config_param_persist_on) command:</span></span>

```azurecli
az config param-persist on
```

<span data-ttu-id="d06ac-124">Depois de ativar a persistência, crie outro grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="d06ac-124">After turning on persistence, create another resource group:</span></span>

 ```azurecli
az group create --name OtherResourceGroup --location eastus
```

<span data-ttu-id="d06ac-125">Desde que a persistência esteja ativada, você poderá deixar o parâmetro `--resource-group` fora dos comandos futuros.</span><span class="sxs-lookup"><span data-stu-id="d06ac-125">As long as persistence is on, your can leave the `--resource-group` parameter out of future commands.</span></span> <span data-ttu-id="d06ac-126">O seguinte comando cria uma conta de armazenamento no grupo **OtherResourceGroup**:</span><span class="sxs-lookup"><span data-stu-id="d06ac-126">The following command creates a storage account in the **OtherResourceGroup** group:</span></span>

```azurecli
az storage account create --name storage135 --location eastus --sku Standard_LRS
```

<span data-ttu-id="d06ac-127">Se você especificar um grupo de recursos no comando, isso terá precedência.</span><span class="sxs-lookup"><span data-stu-id="d06ac-127">If you specify a resource group in the command, that takes precedence.</span></span> <span data-ttu-id="d06ac-128">O seguinte comando cria um grupo de armazenamento em um grupo de recursos chamado **StorageGroups**:</span><span class="sxs-lookup"><span data-stu-id="d06ac-128">The following command creates a storage group in a resource group called **StorageGroups**:</span></span>

```azurecli
az storage account create --resource-group StorageGroups --name storage136 --location eastus --sku Standard_LRS
```

<span data-ttu-id="d06ac-129">No entanto, depois que você especificar outro grupo de recursos como um valor, a CLI do Azure redefinirá o valor persistente.</span><span class="sxs-lookup"><span data-stu-id="d06ac-129">Once you specify another resource group as a value, however, Azure CLI resets the persisted value.</span></span> <span data-ttu-id="d06ac-130">Os novos comandos usam **StorageGroups** como o grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-130">New commands use **StorageGroups** as the resource group.</span></span> <span data-ttu-id="d06ac-131">Você poderá ver os valores persistentes usando o comando [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show):</span><span class="sxs-lookup"><span data-stu-id="d06ac-131">You can see the persisted values by using the [az config param-persist show](/cli/azure/config/param-persist#az_config_param_persist_show) command:</span></span>

```azurecli
az config param-persist show
```

<span data-ttu-id="d06ac-132">Esse comando mostra os valores persistentes atuais.</span><span class="sxs-lookup"><span data-stu-id="d06ac-132">This command shows you the current persisted values.</span></span> <span data-ttu-id="d06ac-133">Esses valores são armazenados em um arquivo chamado *local_context_\<username>* em um diretório oculto chamado *.azure*.</span><span class="sxs-lookup"><span data-stu-id="d06ac-133">These values are stored in a file called *local_context_\<username>* in a hidden directory called *.azure*.</span></span> <span data-ttu-id="d06ac-134">A CLI do Azure cria o diretório na sua localização atual quando você cria um valor persistente pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="d06ac-134">Azure CLI creates the directory in your current location when you first create a persistent value.</span></span>

<span data-ttu-id="d06ac-135">Quando você terminar de usar parâmetros persistentes, execute o comando [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off):</span><span class="sxs-lookup"><span data-stu-id="d06ac-135">When you're done using persisted parameters, run the [az config param-persist off](/cli/azure/config/param-persist#az_config_param_persist_off) command:</span></span>

```azurecli
az config param-persist off
```

<span data-ttu-id="d06ac-136">A CLI do Azure salvará os valores persistentes.</span><span class="sxs-lookup"><span data-stu-id="d06ac-136">Azure CLI saves your persisted values.</span></span> <span data-ttu-id="d06ac-137">Você poderá vê-los no arquivo de contexto local.</span><span class="sxs-lookup"><span data-stu-id="d06ac-137">You can see them in the local context file.</span></span> <span data-ttu-id="d06ac-138">Se você ativar a persistência de parâmetro novamente, esses valores já estarão definidos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-138">If you turn on parameter persistence again, those values are already set.</span></span>

<span data-ttu-id="d06ac-139">Para obter mais informações sobre como usar os comandos [az config param-persist](/cli/azure/config/param-persist), confira [Usar parâmetros persistentes para simplificar os comandos sequenciais da CLI do Azure](/cli/azure/param-persist-tutorial).</span><span class="sxs-lookup"><span data-stu-id="d06ac-139">For more information about using the [az config param-persist](/cli/azure/config/param-persist) commands, see [Use persisted parameters to simplify sequential Azure CLI commands](/cli/azure/param-persist-tutorial).</span></span>

## <a name="set-a-default-resource-group"></a><span data-ttu-id="d06ac-140">Definir um grupo de recursos padrão</span><span class="sxs-lookup"><span data-stu-id="d06ac-140">Set a default resource group</span></span>

<span data-ttu-id="d06ac-141">Você pode definir um grupo de recursos padrão para todos os comandos executados da CLI do Azure local ou do Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="d06ac-141">You can set a default resource group for all the commands that you run from your local Azure CLI or from Azure Cloud Shell.</span></span> <span data-ttu-id="d06ac-142">A CLI do Azure armazena essa configuração localmente em um arquivo *config*.</span><span class="sxs-lookup"><span data-stu-id="d06ac-142">Azure CLI stores this configuration locally in a *config* file.</span></span> <span data-ttu-id="d06ac-143">Para ver a configuração atual, execute o comando [az config get](/cli/azure/config#az_config_get):</span><span class="sxs-lookup"><span data-stu-id="d06ac-143">To see your current configuration, run the [az config get](/cli/azure/config#az_config_get) command:</span></span>

```azurecli
az config get
```

<span data-ttu-id="d06ac-144">O resultado mostra os grupos de recursos padrão e outros valores padrão.</span><span class="sxs-lookup"><span data-stu-id="d06ac-144">The result shows default resource groups and other default values.</span></span> <span data-ttu-id="d06ac-145">Se você estiver usando a CLI do Azure pela primeira vez, os resultados poderão estar vazios.</span><span class="sxs-lookup"><span data-stu-id="d06ac-145">If you're using Azure CLI for the first time, the results might be empty.</span></span>

<span data-ttu-id="d06ac-146">Para definir um grupo de recursos padrão para a instalação da CLI do Azure, execute o comando [az config set](/cli/azure/config#az_config_set):</span><span class="sxs-lookup"><span data-stu-id="d06ac-146">To set a default resource group for your Azure CLI installation, run the [az config set](/cli/azure/config#az_config_set) command:</span></span>

```azurecli
az config set defaults.group=MyResourceGroup
```

<span data-ttu-id="d06ac-147">O comando define um valor para uma chave especificada, neste caso, `defaults.group`.</span><span class="sxs-lookup"><span data-stu-id="d06ac-147">The command sets a value for a specified key, in this case `defaults.group`.</span></span> <span data-ttu-id="d06ac-148">Para obter as opções de configuração disponíveis, confira [Configuração da CLI do Azure](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="d06ac-148">For available configuration options, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>

> [!NOTE]
> <span data-ttu-id="d06ac-149">O comando [az config set](/cli/azure/config#az_config_set) não valida a existência do grupo de recursos inserido.</span><span class="sxs-lookup"><span data-stu-id="d06ac-149">The [az config set](/cli/azure/config#az_config_set) command does not validate the existence of the resource group you enter.</span></span> <span data-ttu-id="d06ac-150">O comando apenas armazena o par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="d06ac-150">The command simply stores the key-value pair.</span></span>

<span data-ttu-id="d06ac-151">Depois que você executar o comando, os dois seguintes comandos fornecerão o mesmo resultado:</span><span class="sxs-lookup"><span data-stu-id="d06ac-151">After you run the command, the following two commands would give you the same result:</span></span>

```azurecli
az storage account create --resource-group MyResourceGroup --name storage01  --location eastus --sku Standard_LRS
az storage account create --name storage01 --location eastus --sku Standard_LRS
```

<span data-ttu-id="d06ac-152">Um grupo de recursos pertence a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d06ac-152">A resource group belongs to a subscription.</span></span> <span data-ttu-id="d06ac-153">Se a sua organização tiver mais de uma assinatura, você precisará definir essa assinatura antes de trabalhar com um grupo de recursos na assinatura.</span><span class="sxs-lookup"><span data-stu-id="d06ac-153">If your organization has more than one subscription, you need to set that subscription before working with a resource group in the subscription.</span></span> <span data-ttu-id="d06ac-154">Se o valor padrão de um grupo de recursos não pertencer à sua assinatura atual, ocorrerá um erro.</span><span class="sxs-lookup"><span data-stu-id="d06ac-154">If the default value of a resource group does not belong to your current subscription, an error results.</span></span> <span data-ttu-id="d06ac-155">Para obter mais informações sobre o uso de várias assinaturas, confira [Usar várias assinaturas do Azure](manage-azure-subscriptions-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="d06ac-155">For more information about multiple subscriptions, see [Use multiple Azure subscriptions](manage-azure-subscriptions-azure-cli.md).</span></span>

<span data-ttu-id="d06ac-156">Você não precisa redefinir o padrão para usar outros grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="d06ac-156">You don't have to reset the default to use other resource groups.</span></span> <span data-ttu-id="d06ac-157">Em vez disso, especifique o grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="d06ac-157">Instead, specify the resource group:</span></span>

```azurecli
az group create --name OtherResourceGroup --location eastus
az storage account create --resource-group StorageGroups --name storage03  --location westus --sku Standard_LRS
```

<span data-ttu-id="d06ac-158">O valor padrão destina-se apenas a você.</span><span class="sxs-lookup"><span data-stu-id="d06ac-158">The default value is for you only.</span></span> <span data-ttu-id="d06ac-159">Ele não afetará outros usuários ou as alterações feitas por meio do portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d06ac-159">It won't affect other users or changes you make through the Azure portal.</span></span>

<span data-ttu-id="d06ac-160">Se você estiver usando valores de parâmetros persistentes, conforme descrito neste artigo, esses valores terão precedência sobre os padrões definidos no arquivo *config*.</span><span class="sxs-lookup"><span data-stu-id="d06ac-160">If you are using persisted parameter values, as described in this article, those values take precedence over defaults set in the *config* file.</span></span>

## <a name="clean-up-resources"></a><span data-ttu-id="d06ac-161">Limpar os recursos</span><span class="sxs-lookup"><span data-stu-id="d06ac-161">Clean up resources</span></span>

<span data-ttu-id="d06ac-162">Se você testou um dos comandos deste artigo, remova todos os recursos criados com o comando [az group delete](/cli/azure/group#az_group_delete):</span><span class="sxs-lookup"><span data-stu-id="d06ac-162">If you tried any of the commands in this article, you can remove any resources you created by using the [az group delete](/cli/azure/group#az_group_delete) command:</span></span>

```azurecli
az group delete --name MyResourceGroup
az group delete --name OtherResourceGroup
az group delete --name StorageGroups
```

<span data-ttu-id="d06ac-163">Esse comando remove o grupo e todos os recursos que ele contém ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="d06ac-163">This command removes the group and all the resources that it contains at once.</span></span>

<span data-ttu-id="d06ac-164">Remova os parâmetros persistentes executando o comando [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete):</span><span class="sxs-lookup"><span data-stu-id="d06ac-164">You can remove the persistent parameters by running the [az config param-persist delete](/cli/azure/config/param-persist#az_config_param_persist_delete) command:</span></span>

```azurecli
az config param-persist delete --all
```

## <a name="see-also"></a><span data-ttu-id="d06ac-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="d06ac-165">See also</span></span>

[<span data-ttu-id="d06ac-166">Configuração da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d06ac-166">Azure CLI configuration</span></span>](/cli/azure/azure-cli-configuration)

[<span data-ttu-id="d06ac-167">Tutorial: usar parâmetros persistentes para simplificar comandos sequenciais da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d06ac-167">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>](/cli/azure/param-persist-tutorial)

[<span data-ttu-id="d06ac-168">Usar várias assinaturas do Azure</span><span class="sxs-lookup"><span data-stu-id="d06ac-168">Use multiple Azure subscriptions</span></span>](manage-azure-subscriptions-azure-cli.md)
