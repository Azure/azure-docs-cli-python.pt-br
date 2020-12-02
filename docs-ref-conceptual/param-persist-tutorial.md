---
title: Tutorial sobre como usar parâmetros persistentes com a CLI do Azure
description: Tutorial sobre como usar o az config param-persist a fim de armazenar valores de parâmetro da CLI do Azure para uso recorrente
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 11/25/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 9db3035c9a50a2a3cc356f3fd7a49ab4f28652ee
ms.sourcegitcommit: 05b58a872cdd165805df62614000637144d80066
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96470427"
---
# <a name="tutorial-use-persisted-parameters-to-simplify-sequential-azure-cli-commands"></a><span data-ttu-id="5e8ba-103">Tutorial: usar parâmetros persistentes para simplificar comandos sequenciais da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5e8ba-103">Tutorial: Use persisted parameters to simplify sequential Azure CLI commands</span></span>

<span data-ttu-id="5e8ba-104">A CLI do Azure oferece os parâmetros persistentes que lhe permitem armazenar valores de parâmetro para uso contínuo.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-104">Azure CLI offers persisted parameters that enable you to store parameter values for continued use.</span></span>  <span data-ttu-id="5e8ba-105">Neste tutorial, você aprende a trabalhar com valores persistentes e a usar esses valores locais para executar com eficiência comandos sequenciais.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-105">In this tutorial, you learn how to work with persisted values, and use these local values to efficiently execute sequential commands.</span></span>

<span data-ttu-id="5e8ba-106">Neste tutorial, você aprenderá a:</span><span class="sxs-lookup"><span data-stu-id="5e8ba-106">In this tutorial, you will learn to:</span></span>

> [!div class="checklist"]
> * <span data-ttu-id="5e8ba-107">Usar comandos de referência do **az config param-persist**</span><span class="sxs-lookup"><span data-stu-id="5e8ba-107">Use **az config param-persist** reference commands</span></span>
> * <span data-ttu-id="5e8ba-108">Executar comandos sequenciais usando os parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-108">Execute sequential commands using persisted parameters</span></span>

<span data-ttu-id="5e8ba-109">Este tutorial usa os comandos da CLI do Azure a seguir</span><span class="sxs-lookup"><span data-stu-id="5e8ba-109">This tutorial uses the following Azure CLI commands</span></span>

- [<span data-ttu-id="5e8ba-110">az config param-persist delete</span><span class="sxs-lookup"><span data-stu-id="5e8ba-110">az config param-persist delete</span></span>](/cli/azure/config/param-persist#az_config_param_persist_delete)
- [<span data-ttu-id="5e8ba-111">az config param-persist off</span><span class="sxs-lookup"><span data-stu-id="5e8ba-111">az config param-persist off</span></span>](/cli/azure/config/param-persist#az_config_param_persist_off)
- [<span data-ttu-id="5e8ba-112">az config param-persist on</span><span class="sxs-lookup"><span data-stu-id="5e8ba-112">az config param-persist on</span></span>](/cli/azure/config/param-persist#az_config_param_persist_on)
- [<span data-ttu-id="5e8ba-113">az config param-persist show</span><span class="sxs-lookup"><span data-stu-id="5e8ba-113">az config param-persist show</span></span>](/cli/azure/config/param-persist#az_config_param_persist_show)
- [<span data-ttu-id="5e8ba-114">az function app create</span><span class="sxs-lookup"><span data-stu-id="5e8ba-114">az function app create</span></span>](/cli/azure/functionapp#az_functionapp_create)
- [<span data-ttu-id="5e8ba-115">az group create</span><span class="sxs-lookup"><span data-stu-id="5e8ba-115">az group create</span></span>](/cli/azure/group#az_group_create)
- [<span data-ttu-id="5e8ba-116">az storage account create</span><span class="sxs-lookup"><span data-stu-id="5e8ba-116">az storage account create</span></span>](/cli/azure/storage/account#az_storage_account_create)


<span data-ttu-id="5e8ba-117">Se você não tiver uma assinatura do Azure, crie uma [conta gratuita](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) antes de começar.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-117">If you don't have an Azure subscription, create a [free account](https://azure.microsoft.com/free/?WT.mc_id=A261C142F) before you begin.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e8ba-118">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5e8ba-118">Prerequisites</span></span>

1. [<span data-ttu-id="5e8ba-119">Instalar a CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5e8ba-119">Install the Azure CLI</span></span>](install-azure-cli.md)

   <span data-ttu-id="5e8ba-120">Se preferir, você também pode usar o Azure Cloud Shell para concluir as etapas deste tutorial.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-120">If you prefer, you can also use Azure Cloud Shell to complete the steps in this tutorial.</span></span>  <span data-ttu-id="5e8ba-121">O Azure Cloud Shell é um ambiente de shell interativo usado por meio do navegador.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-121">Azure Cloud Shell is an interactive shell environment that you use through your browser.</span></span>  <span data-ttu-id="5e8ba-122">Inicie o Cloud Shell usando um destes métodos:</span><span class="sxs-lookup"><span data-stu-id="5e8ba-122">Start Cloud Shell by using one of these methods:</span></span>

   - <span data-ttu-id="5e8ba-123">Abra o Cloud Shell acessando [https://shell.azure.com](https://shell.azure.com)</span><span class="sxs-lookup"><span data-stu-id="5e8ba-123">Open Cloud Shell by going to [https://shell.azure.com](https://shell.azure.com)</span></span>

   - <span data-ttu-id="5e8ba-124">Selecione o botão **Cloud Shell** na barra de menus, no canto superior direito do [portal do Azure](https://portal.azure.com)</span><span class="sxs-lookup"><span data-stu-id="5e8ba-124">Select the **Cloud Shell** button on the menu bar at the upper right corner in the [Azure portal](https://portal.azure.com)</span></span>

1. <span data-ttu-id="5e8ba-125">Se estiver usando uma instalação local da CLI do Azure, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="5e8ba-125">If you are using a local install of the Azure CLI, complete the following:</span></span>
   - <span data-ttu-id="5e8ba-126">Entre usando o comando [az login](/cli/azure/reference-index#az-login) e siga as etapas exibidas no terminal para concluir o processo de autenticação.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-126">Sign in using the [az login](/cli/azure/reference-index#az-login) command, then follow the steps displayed in your terminal to complete the authentication process.</span></span>

     ```azurecli
     az login
     ```
    - <span data-ttu-id="5e8ba-127">Este tutorial requer a versão 2.12.0 (ou posterior) da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-127">This tutorial requires version 2.12.0 or later of the Azure CLI.</span></span>  <span data-ttu-id="5e8ba-128">Execute [az version](/cli/azure/reference-index?#az_version) para localizar a versão e as bibliotecas dependentes que estão instaladas.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-128">Run [az version](/cli/azure/reference-index?#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="5e8ba-129">Para fazer a atualização para a versão mais recente, execute [az upgrade](/cli/azure/reference-index?#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="5e8ba-129">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index?#az_upgrade).</span></span>

## <a name="1-determine-your-local-directory"></a><span data-ttu-id="5e8ba-130">1. Determinar o diretório local</span><span class="sxs-lookup"><span data-stu-id="5e8ba-130">1. Determine your local directory</span></span>

<span data-ttu-id="5e8ba-131">Os valores dos parâmetros persistentes são armazenados no diretório de trabalho da conta de armazenamento do Azure usada pelo Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-131">Persisted parameter values are stored in the working directory of the Azure storage account used by Azure Cloud Shell.</span></span>  <span data-ttu-id="5e8ba-132">Se você estiver usando uma instalação local da CLI do Azure, os valores serão armazenados no diretório de trabalho do computador.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-132">If you are using a local install of the Azure CLI, values are stored in the working directory on your machine.</span></span>

<span data-ttu-id="5e8ba-133">Para localizar, criar ou alterar o diretório de trabalho que está sendo usado pela CLI do Azure, use estes comandos familiares da CLI.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-133">To find, create or change the working directory being used by the Azure CLI, use these familiar CLI commands.</span></span>

```azurecli
# List directories
dir

# Make directory
mkdir azCLI

# Change directory
cd azCLI
```

## <a name="2-turn-on-persisted-parameters"></a><span data-ttu-id="5e8ba-134">2. Ativar os parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-134">2. Turn on Persisted parameters</span></span>

<span data-ttu-id="5e8ba-135">Os [Parâmetros persistentes](/cli/azure/param-persist) devem ser ativados para que seja possível armazenar valores de parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-135">[Persisted parameters](/cli/azure/param-persist) must be turned on before parameter values can be stored.</span></span>  <span data-ttu-id="5e8ba-136">Você receberá um aviso até que o **az config param-persist** saia da fase experimental.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-136">You will receive a warning until **az config param-persist** moves out of the experimental stage.</span></span>  <span data-ttu-id="5e8ba-137">Confira [Visão geral: tipos de referência e status da CLI do Azure](/cli/azure/reference-types-and-status) para saber mais sobre os tipos de referência, os status e os níveis de suporte da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-137">See [Overview: Azure CLI reference types and status](/cli/azure/reference-types-and-status) to learn about the Azure CLI reference types, status, and support levels.</span></span>

```azurecli
az config param-persist on
```

## <a name="3-create-persisted-parameters"></a><span data-ttu-id="5e8ba-138">3. Criar parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-138">3. Create persisted parameters</span></span>

<span data-ttu-id="5e8ba-139">Para armazenar valores em parâmetros persistentes, execute o comando que preferir da CLI do Azure que contenha os parâmetros que você deseja armazenar.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-139">To store values for persisted parameters, execute an Azure CLI command of your choice that contains the parameters you want to store.</span></span>  <span data-ttu-id="5e8ba-140">Por exemplo, crie um grupo de recursos e os parâmetros **--location** e **--name** serão armazenados para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-140">For example, create a resource group and the **--location** and **--name** parameters are stored for future use.</span></span>

1. <span data-ttu-id="5e8ba-141">Armazene o local e o nome do grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-141">Store the location and resource group name.</span></span>
   ```azurecli
   # With persisted parameters turned on, create a resource group
   az group create --name RG1forTutorial --location eastus2

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

1. <span data-ttu-id="5e8ba-142">Usando os novos parâmetros persistentes, crie uma conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-142">Using the new persisted parameters, create a storage account.</span></span>

   ```azurecli
   # Create a storage account
   az storage account create --name sa1fortutorial

   # See that storage_account_name has been added to persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="5e8ba-143">Crie um parâmetro persistente sem criar um recurso.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-143">Create a persisted parameter without creating a new resource.</span></span>

   <span data-ttu-id="5e8ba-144">Se você não quiser criar um recurso do Azure, os parâmetros **resource_group_name** e **location** poderão ser armazenados usando comandos que não são de criação, como o **show** ou **list**.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-144">If you do not want to create a new Azure resource, **resource_group_name** and **location** parameters can be stored by using non-create commands like **show** or **list**.</span></span>   <span data-ttu-id="5e8ba-145">Confira [Parâmetros persistentes da CLI do Azure](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) para obter uma lista completa dos parâmetros com suporte e a ação necessária para manter os valores.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-145">See [Azure CLI persisted parameters](/cli/azure/param-persist-howto#compare-parameter-persistence-and-global-variables) for a full list of supported parameters,   and the action needed to retain values.</span></span>  <span data-ttu-id="5e8ba-146">Este exemplo também remove todos os valores de parâmetro usando o comando [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete).</span><span class="sxs-lookup"><span data-stu-id="5e8ba-146">This example also removes all parameter values by using the [az config param-persist delete](/cli/azure/config/param-persist#az-param-persist-delete) command.</span></span>

   ```azurecli
   # Clear all persisted parameters for demonstration.
   az config param-persist delete --all

   # List all storage accounts which will create the **resource_group_name** stored parameter value.
   az storage account show --resource-group RG1forTutorial --name sa1fortutorial

   # See the new stored value created for resource group.  The storage account name is only stored with a 'create' command.
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "resource_group_name": "RG1forTutorial"
     }
   }
   ```

## <a name="4-replace-persisted-parameters"></a><span data-ttu-id="5e8ba-147">4. Substituir parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-147">4. Replace persisted parameters</span></span>

<span data-ttu-id="5e8ba-148">Substituir um valor de parâmetro armazenado é tão simples quanto executar um comando que contém um valor diferente.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-148">Replacing a stored parameter value is as simple as executing a command containing a different value.</span></span>

1. <span data-ttu-id="5e8ba-149">Crie parâmetros persistentes.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-149">Create new persisted parameters.</span></span>
   ```azurecli
   # Clear all persisted parameters for demonstration
   az config param-persist delete --all

   # Create a storage account placing "location", "resource_group_name", and "storage_account_name" into persisted parameters
   az storage account create --name sa1fortutorial --resource-group RG1forTutorial --location eastus2

   # See persisted parameters entries
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "eastus2",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa1fortutorial"
     }
   }
   ```

1. <span data-ttu-id="5e8ba-150">Substitua os valores recém-armazenados.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-150">Replace the newly stored values.</span></span>

   ```azurecli
   # Create a second storage account while changing both the "storage_account_name" and "location" persisted parameters
   az storage account create --name sa2fortutorial --location westeurope

   # See new persisted parameters
   az config param-persist show
   ```

   ```output
   {
     "all": {
       "location": "westeurope",
       "resource_group_name": "RG1forTutorial",
       "storage_account_name": "sa2fortutorial"
     }
   }
   ```

   > [!NOTE]
   >
   > <span data-ttu-id="5e8ba-151">Mesmo se os parâmetros persistentes estiverem ativados, você não precisará usá-los.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-151">Even if persisted parameters are turned on, you don't have to use them.</span></span>  <span data-ttu-id="5e8ba-152">Você ainda pode executar os comandos com todos os valores de parâmetro especificados.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-152">You can still execute commands with all parameter values specified.</span></span>  <span data-ttu-id="5e8ba-153">No entanto, lembre-se de que, com os parâmetros persistentes ativados, _você sempre criará parâmetros persistentes ou substituirá os parâmetros persistentes existentes._</span><span class="sxs-lookup"><span data-stu-id="5e8ba-153">However, be aware that with persisted parameters turned on, _you will be creating new persisted parameters, or overwriting existing ones._</span></span>

## <a name="5-execute-sequential-commands"></a><span data-ttu-id="5e8ba-154">5. Executar comandos sequenciais</span><span class="sxs-lookup"><span data-stu-id="5e8ba-154">5. Execute sequential commands</span></span>

<span data-ttu-id="5e8ba-155">Esses scripts criam um Aplicativo de funções do Azure usando o Plano de consumo.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-155">These scripts create an Azure Function app using the Consumption plan.</span></span>

### <a name="using-persisted-parameters"></a>[<span data-ttu-id="5e8ba-156">Usando parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-156">Using persisted parameters</span></span>](#tab/azure-cli)

```azurecli
# Reminder: function app and storage account names must be unique.

# Turn persisted parameters on.
az config param-persist on

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group omitting "--location" and "--resource-group" parameters.
az storage account create \
  --name sa3fortutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting "--storage-account" and "--resource-group" parameters.
az functionapp create \
  --name FAforTutorial \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values.
az config param-persist show
```

### <a name="without-persisted-parameters"></a>[<span data-ttu-id="5e8ba-157">Sem parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-157">Without persisted parameters</span></span>](#tab/azure-portal)

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters off
az config param-persist off

# Create a resource group.
az group create --name RG2forTutorial --location westeurope

# Create an Azure storage account in the resource group.
az storage account create \
  --name sa3fortutorial \
  --location westeurope \
  --resource-group RG2forTutorial \
  --sku Standard_LRS

# Create a serverless function app in the resource group.
az functionapp create \
  --name FAforTutorial \
  --storage-account sa3fortutorial \
  --consumption-plan-location westeurope \
  --resource-group RG2forTutorial \
  --functions-version 2
```

* * *

## <a name="6-delete-persisted-parameters"></a><span data-ttu-id="5e8ba-158">6. Excluir parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-158">6. Delete persisted parameters</span></span>

<span data-ttu-id="5e8ba-159">Use o comando [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) para remover entradas.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-159">Use the [az config param-persist delete](/cli/azure/param-persist#az-param-persist-delete) command to remove entries.</span></span>

```azurecli
# Remove a single persisted parameters entry by specifying the name, not the value
az config param-persist delete resource_group_name

# Remove all persisted parameters entries and do not prompt for confirmation
az config param-persist delete --all --yes
```

> [!IMPORTANT]
>
> <span data-ttu-id="5e8ba-160">Os parâmetros persistentes não são atualizados quando um recurso do Azure é excluído.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-160">Persisted parameters do not get updated when an Azure resource is deleted.</span></span>
>
> ```azurecli
> # delete a resource group
> az group delete --name RG1forTutorial
>
> # verify that the resource group no longer exists
> az group list --output table
>
> # See that the resource group name remains in persisted parameters
> az config param-persist show
> ```

## <a name="7-turn-persisted-parameters-off"></a><span data-ttu-id="5e8ba-161">7. Desativar os parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="5e8ba-161">7. Turn persisted parameters off</span></span>

<span data-ttu-id="5e8ba-162">Você pode desativar os parâmetros persistentes usando o comando [az config param-persist off](/cli/azure/param-persist#az-param-persist-off), mas os dados de parâmetros persistentes salvos não serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-162">You can turn persisted parameters off by using the [az config param-persist off](/cli/azure/param-persist#az-param-persist-off) command, but your saved persisted parameters data won't be deleted.</span></span>

```azurecli
# Turn persisted parameters off
az config param-persist off

# See that your persisted parameters still exist
az config param-persist show

# Try to create a new resource relying on persisted parameters and receive error "...the following arguments are required:..."
az storage account create --name SA4inAzCLI --sku Standard_LRS
```

## <a name="8-clean-up-resources"></a><span data-ttu-id="5e8ba-163">8. Limpar os recursos</span><span class="sxs-lookup"><span data-stu-id="5e8ba-163">8. Clean up resources</span></span>

<span data-ttu-id="5e8ba-164">Quando não forem mais necessários, use o comando [az group delete](/cli/azure/group) para remover o grupo de recursos e todos os recursos relacionados.</span><span class="sxs-lookup"><span data-stu-id="5e8ba-164">When no longer needed, use the [az group delete](/cli/azure/group) command to remove the resource group, and all related resources.</span></span>

```azurecli
az group delete --name RG1forTutorial
```

## <a name="see-also"></a><span data-ttu-id="5e8ba-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="5e8ba-165">See also</span></span>

- [<span data-ttu-id="5e8ba-166">Como trabalhar com os parâmetros persistentes da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5e8ba-166">(How to work with Azure CLI persisted parameters</span></span>](param-persist-howto.md)
- [<span data-ttu-id="5e8ba-167">Configuração da CLI do Azure usando o az configure</span><span class="sxs-lookup"><span data-stu-id="5e8ba-167">Azure CLI Configuration using az configure</span></span>](/cli/azure/azure-cli-configuration)
