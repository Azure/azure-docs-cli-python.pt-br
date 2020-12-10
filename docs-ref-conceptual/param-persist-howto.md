---
title: Opções de parâmetro persistente da CLI do Azure
description: Como usar o parâmetro persistente da CLI do Azure para armazenar valores de parâmetro reutilizáveis
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.prod: azure
ms.date: 10/30/2020
ms.topic: conceptual
ms.devlang: azurecli
ms.technology: azure-cli
ms.custom: devex-track-azurecli
ms.openlocfilehash: 087f5f05d6a4a6b25e6aebd0d2c482ebba656b01
ms.sourcegitcommit: 9beaf9abb794f1006a56acee4e1cfb8ea7fe2405
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2020
ms.locfileid: "96850211"
---
# <a name="azure-cli-persisted-parameter"></a><span data-ttu-id="013e6-103">Parâmetro persistente da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-103">Azure CLI persisted parameter</span></span>

<span data-ttu-id="013e6-104">A referência do [az config param-persist](/cli/azure/param-persist) da CLI do Azure fornece a capacidade de reter valores de parâmetros persistentes locais para os comandos da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="013e6-104">The Azure CLI [az config param-persist](/cli/azure/param-persist) reference provides the ability to retain local persisted parameter values for Azure CLI commands.</span></span>  <span data-ttu-id="013e6-105">Isso elimina a necessidade de redigitar com frequência os parâmetros comuns.</span><span class="sxs-lookup"><span data-stu-id="013e6-105">This removes the need to continually retype common parameters.</span></span> <span data-ttu-id="013e6-106">Por exemplo, a localização e o grupo de recursos são parâmetros obrigatórios em muitos comandos da CLI, mas eles não contribuem para a _intenção_ do comando.</span><span class="sxs-lookup"><span data-stu-id="013e6-106">For example, location and resource-group are required parameters in many CLI commands, but they don't contribute to the _intent_ of the command.</span></span>  <span data-ttu-id="013e6-107">Ao armazenar valores de parâmetro por meio de parâmetros persistentes, você diminui a redundância e pode reduzir significativamente a sintaxe dos comandos da CLI.</span><span class="sxs-lookup"><span data-stu-id="013e6-107">When you store parameter values with persisted parameter, you reduce redundancy and can significantly shorten CLI command syntax.</span></span>

<span data-ttu-id="013e6-108">Os valores da configuração usados pela CLI são avaliados na seguinte precedência, com os itens na parte superior da lista sendo prioridade.</span><span class="sxs-lookup"><span data-stu-id="013e6-108">Configuration values used by the CLI are evaluated in the following precedence, with items higher on the list taking priority.</span></span>

1. <span data-ttu-id="013e6-109">Parâmetros de linha de comando</span><span class="sxs-lookup"><span data-stu-id="013e6-109">Command-line parameters</span></span>
1. <span data-ttu-id="013e6-110">Valores do diretório de trabalho local definidos pelo **az config param-persist**</span><span class="sxs-lookup"><span data-stu-id="013e6-110">Values in the local working directory set by **az config param-persist**</span></span>
1. <span data-ttu-id="013e6-111">Variáveis de ambiente</span><span class="sxs-lookup"><span data-stu-id="013e6-111">Environment variables</span></span>
1. <span data-ttu-id="013e6-112">Valores do arquivo de configuração ou definidos com o **az config**</span><span class="sxs-lookup"><span data-stu-id="013e6-112">Values in the configuration file or set with **az config**</span></span>

<span data-ttu-id="013e6-113">[Instale a CLI do Azure](install-azure-cli.md) ou abra o [Azure Cloud Shell](https://shell.azure.com) para executar os scripts deste artigo.</span><span class="sxs-lookup"><span data-stu-id="013e6-113">[Install the Azure CLI](install-azure-cli.md) or open [Azure Cloud Shell](https://shell.azure.com) to run the scripts in this article.</span></span>  <span data-ttu-id="013e6-114">Se você estiver usando uma instalação local da CLI do Azure, será necessário ter a versão 2.12.0 (ou posterior) para executar os comandos do **az config param-persist**.</span><span class="sxs-lookup"><span data-stu-id="013e6-114">If you are using a local install of the Azure CLI, version 2.12.0 or later is needed to run **az config param-persist** commands.</span></span>  <span data-ttu-id="013e6-115">Execute [az version](/cli/azure/reference-index#az_version) para localizar a versão e as bibliotecas dependentes que estão instaladas.</span><span class="sxs-lookup"><span data-stu-id="013e6-115">Run [az version](/cli/azure/reference-index#az_version) to find the version and dependent libraries that are installed.</span></span> <span data-ttu-id="013e6-116">Para fazer a atualização para a versão mais recente, execute [az upgrade](/cli/azure/reference-index#az_upgrade).</span><span class="sxs-lookup"><span data-stu-id="013e6-116">To upgrade to the latest version, run [az upgrade](/cli/azure/reference-index#az_upgrade).</span></span>  <span data-ttu-id="013e6-117">O Azure Cloud Shell sempre tem a última versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="013e6-117">Azure Cloud Shell always has the latest version of the Azure CLI.</span></span>

## <a name="persisted-parameter-data-file"></a><span data-ttu-id="013e6-118">Arquivo de dados do parâmetro persistente</span><span class="sxs-lookup"><span data-stu-id="013e6-118">Persisted parameter data file</span></span>

<span data-ttu-id="013e6-119">Os valores dos parâmetros persistentes são mantidos em um arquivo chamado **.param_persist**, armazenado no diretório de trabalho.</span><span class="sxs-lookup"><span data-stu-id="013e6-119">Persisted parameter values are kept in a file named **.param_persist** which is stored in your working directory.</span></span>  <span data-ttu-id="013e6-120">Se você estiver usando o [Azure Cloud Shell](https://shell.azure.com) para executar comandos da CLI do Azure, o diretório de trabalho estará na conta de armazenamento usada pela CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="013e6-120">If you are using [Azure Cloud Shell](https://shell.azure.com) to execute Azure CLI commands, your working directory is in the storage account being used by the Azure CLI.</span></span>  <span data-ttu-id="013e6-121">Se você estiver usando uma [instalação local](/install-azure-cli) da CLI do Azure, o diretório de trabalho estará no computador local.</span><span class="sxs-lookup"><span data-stu-id="013e6-121">If you are using a [local install](/install-azure-cli) of the Azure CLI, your working directory is on your local machine.</span></span>  <span data-ttu-id="013e6-122">Seja em qualquer um dos locais, o arquivo **.param_persist** fica oculto e não deve ser atualizado manualmente.</span><span class="sxs-lookup"><span data-stu-id="013e6-122">In either location, the **.param_persist** file is hidden and should not be manually updated.</span></span>

## <a name="persisted-parameter-storage-and-support"></a><span data-ttu-id="013e6-123">Armazenamento e suporte de parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="013e6-123">Persisted parameter storage and support</span></span>

<span data-ttu-id="013e6-124">Os parâmetros da CLI do Azure a seguir são compatíveis com parâmetros persistentes.</span><span class="sxs-lookup"><span data-stu-id="013e6-124">The following Azure CLI parameters are supported by persisted parameter.</span></span>  <span data-ttu-id="013e6-125">Os parâmetros **resource_group_name** e **location** são armazenados de maneira diferente, de modo que você pode adicioná-los a parâmetros persistentes _sem_ executar o comando create.</span><span class="sxs-lookup"><span data-stu-id="013e6-125">The **resource_group_name** and **location** parameters are stored differently in that you can add them to persisted parameter _without_ executing a create command.</span></span>

| <span data-ttu-id="013e6-126">Parâmetro persistente</span><span class="sxs-lookup"><span data-stu-id="013e6-126">Persisted parameter</span></span> | <span data-ttu-id="013e6-127">Ação de armazenamento</span><span class="sxs-lookup"><span data-stu-id="013e6-127">Storage action</span></span> | <span data-ttu-id="013e6-128">Com suporte por</span><span class="sxs-lookup"><span data-stu-id="013e6-128">Supported by</span></span>
|-|-|-|
| <span data-ttu-id="013e6-129">local</span><span class="sxs-lookup"><span data-stu-id="013e6-129">location</span></span> | <span data-ttu-id="013e6-130">Executar qualquer comando</span><span class="sxs-lookup"><span data-stu-id="013e6-130">Execute any command</span></span> | <span data-ttu-id="013e6-131">Todas as referências da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-131">All Azure CLI references</span></span>
| <span data-ttu-id="013e6-132">resource_group_name</span><span class="sxs-lookup"><span data-stu-id="013e6-132">resource_group_name</span></span> | <span data-ttu-id="013e6-133">Executar qualquer comando</span><span class="sxs-lookup"><span data-stu-id="013e6-133">Execute any command</span></span> | <span data-ttu-id="013e6-134">Todas as referências da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-134">All Azure CLI references</span></span>
| <span data-ttu-id="013e6-135">vnet_name</span><span class="sxs-lookup"><span data-stu-id="013e6-135">vnet_name</span></span> | <span data-ttu-id="013e6-136">Executar um comando create</span><span class="sxs-lookup"><span data-stu-id="013e6-136">Execute a create command</span></span> | <span data-ttu-id="013e6-137">Somente Aplicativos Web do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-137">Azure Web Apps only</span></span>
| <span data-ttu-id="013e6-138">storage_account_name</span><span class="sxs-lookup"><span data-stu-id="013e6-138">storage_account_name</span></span> | <span data-ttu-id="013e6-139">Executar um comando create</span><span class="sxs-lookup"><span data-stu-id="013e6-139">Execute a create command</span></span> |  <span data-ttu-id="013e6-140">Somente Aplicativos Web do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-140">Azure Web Apps only</span></span>
| <span data-ttu-id="013e6-141">webapp_name</span><span class="sxs-lookup"><span data-stu-id="013e6-141">webapp_name</span></span> | <span data-ttu-id="013e6-142">Executar um comando create</span><span class="sxs-lookup"><span data-stu-id="013e6-142">Execute a create command</span></span> | <span data-ttu-id="013e6-143">Somente Aplicativos Web do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-143">Azure Web Apps only</span></span>
| <span data-ttu-id="013e6-144">function_app_name</span><span class="sxs-lookup"><span data-stu-id="013e6-144">function_app_name</span></span> | <span data-ttu-id="013e6-145">Executar um comando create</span><span class="sxs-lookup"><span data-stu-id="013e6-145">Execute a create command</span></span> | <span data-ttu-id="013e6-146">Somente Azure Functions</span><span class="sxs-lookup"><span data-stu-id="013e6-146">Azure Functions only</span></span>

## <a name="sample-script-using-persisted-parameters"></a><span data-ttu-id="013e6-147">Script de exemplo usando parâmetros persistentes</span><span class="sxs-lookup"><span data-stu-id="013e6-147">Sample script using persisted parameters</span></span>

<span data-ttu-id="013e6-148">Sem os parâmetros persistentes, os comandos sequenciais da CLI devem repetir os mesmos valores de parâmetro.</span><span class="sxs-lookup"><span data-stu-id="013e6-148">Without persisted parameters, sequential CLI commands must repeat the same parameter values.</span></span>  <span data-ttu-id="013e6-149">Com os parâmetros persistentes habilitados, os valores de parâmetros armazenados podem ser omitidos nos comandos sequenciais.</span><span class="sxs-lookup"><span data-stu-id="013e6-149">With persisted parameters enabled, your stored parameter values can be omitted from sequential commands.</span></span>  <span data-ttu-id="013e6-150">Neste exemplo, o **local**, o **nome do grupo de recursos** ou o **nome da conta de armazenamento** são repetidos nos comandos subsequentes.</span><span class="sxs-lookup"><span data-stu-id="013e6-150">In this example, the **location**, **resource group name** or **storage account name** are repeated in subsequent commands.</span></span>

```azurecli
# Reminder: function app and storage account names must be unique.

# turn persisted parameters on
az config param-persist on

# Create a resource group which will store "resource group" and "location" in persisted parameter.
az group create --name RGlocalContext --location westeurope

# Create an Azure storage account omitting location and resource group.
az storage account create \
  --name sa1localcontext \
  --sku Standard_LRS

# Create a serverless function app in the resource group omitting storage account and resource group.
az functionapp create \
  --name FAlocalContext \
  --consumption-plan-location westeurope \
  --functions-version 2

# See the stored parameter values
az config param-persist show
```

## <a name="persisted-parameter-and-global-variable-comparison"></a><span data-ttu-id="013e6-151">Comparação entre o parâmetro persistente e a variável global</span><span class="sxs-lookup"><span data-stu-id="013e6-151">Persisted parameter and global variable comparison</span></span>

<span data-ttu-id="013e6-152">Há dois comandos da CLI do Azure que podem ser usados para valores de parâmetro padrão: o **az configure** e o **az config param-persist**.</span><span class="sxs-lookup"><span data-stu-id="013e6-152">There are two Azure CLI commands that can be used to default parameter values: **az configure** and **az config param-persist**.</span></span>  <span data-ttu-id="013e6-153">Use o comando **az configure** para especificar _variáveis globais_, como grupo, local ou Web.</span><span class="sxs-lookup"><span data-stu-id="013e6-153">Use the **az configure** command to specify _global variables_ such as group, location, or web.</span></span>  <span data-ttu-id="013e6-154">Use **az param-persist** para especificar _valores padrão locais_ exclusivos para a carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="013e6-154">Use **az param-persist** to specify _local default values_ unique to your workload.</span></span>  <span data-ttu-id="013e6-155">Os valores armazenados são usados pela CLI no lugar dos argumentos necessários.</span><span class="sxs-lookup"><span data-stu-id="013e6-155">Stored values are used by the CLI in place of required arguments.</span></span>

> [!Important]
> <span data-ttu-id="013e6-156">Parâmetros persistentes substituem os valores de contexto global.</span><span class="sxs-lookup"><span data-stu-id="013e6-156">Persisted parameters override global context values.</span></span>
>

| <span data-ttu-id="013e6-157">Referência</span><span class="sxs-lookup"><span data-stu-id="013e6-157">Reference</span></span> | <span data-ttu-id="013e6-158">Escopo</span><span class="sxs-lookup"><span data-stu-id="013e6-158">Scope</span></span> | <span data-ttu-id="013e6-159">Definir</span><span class="sxs-lookup"><span data-stu-id="013e6-159">Set</span></span> | <span data-ttu-id="013e6-160">Use</span><span class="sxs-lookup"><span data-stu-id="013e6-160">Use</span></span>
|-|-|-|-|
[<span data-ttu-id="013e6-161">az configure</span><span class="sxs-lookup"><span data-stu-id="013e6-161">az configure</span></span>](/cli/azure/reference-index#az_configure) | <span data-ttu-id="013e6-162">Com escopo global em toda a CLI</span><span class="sxs-lookup"><span data-stu-id="013e6-162">Scoped globally across the CLI</span></span> | <span data-ttu-id="013e6-163">Definir explicitamente usando **az configure --defaults**</span><span class="sxs-lookup"><span data-stu-id="013e6-163">Set explicitly using **az configure --defaults**</span></span> | <span data-ttu-id="013e6-164">Usar para configurações como registro em log, coleta de dados e valores de argumento padrão</span><span class="sxs-lookup"><span data-stu-id="013e6-164">Use for settings such as logging, data collection, and default argument values</span></span>
[<span data-ttu-id="013e6-165">az config param-persist</span><span class="sxs-lookup"><span data-stu-id="013e6-165">az config param-persist</span></span>](/cli/azure/config/param-persist) | <span data-ttu-id="013e6-166">Com escopo definido localmente para um diretório de trabalho específico</span><span class="sxs-lookup"><span data-stu-id="013e6-166">Scoped locally to a specific working directory</span></span> | <span data-ttu-id="013e6-167">Definir automaticamente quando os parâmetros persistentes forem ativados</span><span class="sxs-lookup"><span data-stu-id="013e6-167">Set automatically once persisted parameters are turned on</span></span> | <span data-ttu-id="013e6-168">Use para comandos sequenciais de uma carga de trabalho individual.</span><span class="sxs-lookup"><span data-stu-id="013e6-168">Use for individual workload sequential commands.</span></span>

### <a name="command-examples"></a><span data-ttu-id="013e6-169">Exemplos de comando</span><span class="sxs-lookup"><span data-stu-id="013e6-169">Command examples</span></span>

<span data-ttu-id="013e6-170">Use o **az config param-persist** para definir uma variável global usada na criação de uma conta de armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="013e6-170">Use **az config param-persist** to set a global variable used in the creation of an Azure storage account.</span></span>

```azurecli
# set the global variable for resource group
az configure --defaults group=myGlobalVariableRG

# Create an Azure storage account omitting the resource group relying on the global variable value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount1 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="013e6-171">A saída do comando da CLI mostra que foi criada uma conta de armazenamento no grupo de recursos encontrado na variável global, 'myGlobalVariableRG'.</span><span class="sxs-lookup"><span data-stu-id="013e6-171">CLI command output shows that a new storage account was created in the resource group found in the global variable, \`myGlobalVariableRG'.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myGlobalVariableRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

<span data-ttu-id="013e6-172">Use o **az config param-persist** para definir parâmetros persistentes usados na criação de uma conta de armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="013e6-172">Use **az config param-persist** to set persisted parameters used in the creation of an Azure storage account.</span></span>  <span data-ttu-id="013e6-173">Se uma variável global for definida para o mesmo objeto, o parâmetro persistente substituirá a variável global.</span><span class="sxs-lookup"><span data-stu-id="013e6-173">If a global variable is set for the same object, the persisted parameter will override the global variable.</span></span>

```azurecli
# turn persisted parameter on
az config param-persist on

# Create a resource group in order to write to persisted parameter
az group create --name myParamPersistRG --location westeurope

# Create an Azure storage account omitting the resource group relying on the persisted parameter value
# Substitute the storage account name parameter with a unique value
az storage account create \
  --name mystorageaccount2 \
  --location westeurope \
  --sku Standard_LRS
```

<span data-ttu-id="013e6-174">Mesmo com uma variável global definida para o grupo de recursos com o valor `myGlobalVariableRG`, com os parâmetros persistentes ativados a nova conta de armazenamento foi criada com `myParamPersistRG`.</span><span class="sxs-lookup"><span data-stu-id="013e6-174">Even with a global variable set for resource group with a value of `myGlobalVariableRG`, with persisted parameters turned on, the new storage account was created with `myParamPersistRG`.</span></span>

```output
...
},
  "primaryLocation": "westeurope",
  "privateEndpointConnections": [],
  "provisioningState": "Succeeded",
  "resourceGroup": "myParamPersistRG",
  "routingPreference": null,
  "secondaryEndpoints": null,
  "secondaryLocation": null,
  "sku": {
    "name": "Standard_LRS",
    "tier": "Standard"
},
...
```

## <a name="see-also"></a><span data-ttu-id="013e6-175">Confira também</span><span class="sxs-lookup"><span data-stu-id="013e6-175">See also</span></span>

* [<span data-ttu-id="013e6-176">Tutorial: usar parâmetros persistentes com comandos sequenciais da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="013e6-176">Tutorial: Use persisted parameter with sequential Azure CLI commands</span></span>](param-persist-tutorial.md)
* [<span data-ttu-id="013e6-177">Configuração da CLI do Azure usando o az configure</span><span class="sxs-lookup"><span data-stu-id="013e6-177">Azure CLI Configuration using az configure</span></span>](azure-cli-configuration.md)

