---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4337f2203841d6247e4b487d245138424c63e448
ms.sourcegitcommit: 71c0ccd475524cf4d6db45bba8139fef3262d764
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "58175126"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="6b3f4-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-103">Azure CLI release notes</span></span>
## <a name="march-12-2019"></a><span data-ttu-id="6b3f4-104">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-104">March 12, 2019</span></span>

<span data-ttu-id="6b3f4-105">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="6b3f4-105">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-106">Core</span></span>

* <span data-ttu-id="6b3f4-107">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-107">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-108">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-108">ACR</span></span>

* <span data-ttu-id="6b3f4-109">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-109">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-110">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-110">ACS</span></span>

* <span data-ttu-id="6b3f4-111">Alterado para ignorar o argumento `--listen-address` para `aks browse` se `kubectl` não lhe dar suporte.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-111">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-112">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-112">AppService</span></span>

* <span data-ttu-id="6b3f4-113">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-113">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="6b3f4-114">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-114">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="6b3f4-115">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-115">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="6b3f4-116">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-116">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="6b3f4-117">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-117">Botservice</span></span>

* <span data-ttu-id="6b3f4-118">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-118">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="6b3f4-119">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-119">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="6b3f4-120">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-120">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="6b3f4-121">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-121">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-122">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-122">Container</span></span>

* <span data-ttu-id="6b3f4-123">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-123">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="6b3f4-124">EventHub</span><span class="sxs-lookup"><span data-stu-id="6b3f4-124">EventHub</span></span>

* <span data-ttu-id="6b3f4-125">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-125">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="6b3f4-126">Localizar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-126">Find</span></span>

* <span data-ttu-id="6b3f4-127">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="6b3f4-127">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6b3f4-128">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6b3f4-128">HDInsight</span></span>

* <span data-ttu-id="6b3f4-129">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-129">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-130">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-130">Network</span></span>

* <span data-ttu-id="6b3f4-131">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-131">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-132">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6b3f4-132">Rdbms</span></span>

* <span data-ttu-id="6b3f4-133">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-133">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-134">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-134">Role</span></span>

* <span data-ttu-id="6b3f4-135">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-135">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="6b3f4-136">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-136">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6b3f4-137">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6b3f4-137">Service Fabric</span></span>

* <span data-ttu-id="6b3f4-138">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-138">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="6b3f4-139">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-139">February 26, 2019</span></span>

<span data-ttu-id="6b3f4-140">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="6b3f4-140">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-141">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-141">Core</span></span>

* <span data-ttu-id="6b3f4-142">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="6b3f4-142">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-143">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-143">ACR</span></span>

* <span data-ttu-id="6b3f4-144">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-144">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="6b3f4-145">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-145">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-146">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-146">ACS</span></span>

* <span data-ttu-id="6b3f4-147">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-147">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-148">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-148">AppService</span></span>

* <span data-ttu-id="6b3f4-149">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-149">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-150">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-150">Batch</span></span>
* <span data-ttu-id="6b3f4-151">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-151">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="6b3f4-152">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-152">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="6b3f4-153">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-153">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="6b3f4-154">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="6b3f4-154">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="6b3f4-155">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="6b3f4-155">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="6b3f4-156">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-156">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-157">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-157">CosmosDB</span></span>

* <span data-ttu-id="6b3f4-158">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-158">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="6b3f4-159">Kusto</span><span class="sxs-lookup"><span data-stu-id="6b3f4-159">Kusto</span></span>

* <span data-ttu-id="6b3f4-160">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="6b3f4-160">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-161">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-161">Network</span></span>

* <span data-ttu-id="6b3f4-162">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-162">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="6b3f4-163">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-163">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="6b3f4-164">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-164">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="6b3f4-165">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-165">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="6b3f4-166">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-166">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="6b3f4-167">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-167">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="6b3f4-168">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-168">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-169">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-169">Resource</span></span>

* <span data-ttu-id="6b3f4-170">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-170">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="6b3f4-171">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-171">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="6b3f4-172">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-172">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="6b3f4-173">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-173">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="6b3f4-174">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-174">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-175">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-175">Role</span></span>

* <span data-ttu-id="6b3f4-176">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-176">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-177">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-177">VM</span></span>

* <span data-ttu-id="6b3f4-178">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-178">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="6b3f4-179">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-179">February 12, 2019</span></span>

<span data-ttu-id="6b3f4-180">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="6b3f4-180">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-181">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-181">Core</span></span>

* <span data-ttu-id="6b3f4-182">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-182">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="6b3f4-183">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-183">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-184">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-184">ACR</span></span>
* <span data-ttu-id="6b3f4-185">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-185">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="6b3f4-186">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-186">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-187">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-187">ACS</span></span>
* <span data-ttu-id="6b3f4-188">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-188">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="6b3f4-189">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-189">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="6b3f4-190">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-190">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="6b3f4-191">AMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-191">AMS</span></span>
* <span data-ttu-id="6b3f4-192">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-192">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="6b3f4-193">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-193">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-194">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-194">Appservice</span></span>
* <span data-ttu-id="6b3f4-195">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-195">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="6b3f4-196">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="6b3f4-196">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="6b3f4-197">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-197">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="6b3f4-198">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="6b3f4-198">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="6b3f4-199">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-199">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="6b3f4-200">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-200">Botservice</span></span>
* <span data-ttu-id="6b3f4-201">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-201">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="6b3f4-202">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-202">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="6b3f4-203">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-203">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="6b3f4-204">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="6b3f4-204">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="6b3f4-205">[PRETERIDO] O argumento `--proj-name` em favor de `--proj-file-path` foi preterido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-205">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="6b3f4-206">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-206">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="6b3f4-207">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-207">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="6b3f4-208">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="6b3f4-208">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="6b3f4-209">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-209">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="6b3f4-210">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="6b3f4-210">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="6b3f4-211">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-211">Key Vault</span></span>
* <span data-ttu-id="6b3f4-212">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-212">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-213">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-213">Monitor</span></span>
* <span data-ttu-id="6b3f4-214">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-214">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-215">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-215">Network</span></span>
* <span data-ttu-id="6b3f4-216">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="6b3f4-216">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="6b3f4-217">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-217">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="6b3f4-218">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-218">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="6b3f4-219">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-219">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6b3f4-220">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="6b3f4-220">Policy Insights</span></span>
* <span data-ttu-id="6b3f4-221">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-221">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-222">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-222">RDBMS</span></span>
* <span data-ttu-id="6b3f4-223">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-223">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="6b3f4-224">Redis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-224">Redis</span></span>
* <span data-ttu-id="6b3f4-225">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-225">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="6b3f4-226">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-226">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="6b3f4-227">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-227">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="6b3f4-228">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-228">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="6b3f4-229">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-229">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="6b3f4-230">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-230">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="6b3f4-231">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-231">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-232">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-232">Role</span></span>
* <span data-ttu-id="6b3f4-233">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-233">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="6b3f4-234">SQL VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-234">SQL VM</span></span>
* <span data-ttu-id="6b3f4-235">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-235">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-236">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-236">VM</span></span>
* <span data-ttu-id="6b3f4-237">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-237">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="6b3f4-238">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-238">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="6b3f4-239">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-239">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="6b3f4-240">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-240">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="6b3f4-241">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-241">January 31, 2019</span></span>

<span data-ttu-id="6b3f4-242">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="6b3f4-242">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-243">Core</span></span>

* <span data-ttu-id="6b3f4-244">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="6b3f4-244">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="6b3f4-245">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-245">January 28, 2019</span></span>

<span data-ttu-id="6b3f4-246">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="6b3f4-246">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-247">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-247">ACR</span></span>
* <span data-ttu-id="6b3f4-248">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="6b3f4-248">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-249">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-249">ACS</span></span>
* <span data-ttu-id="6b3f4-250">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-250">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6b3f4-251">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-251">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="6b3f4-252">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-252">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="6b3f4-253">AMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-253">AMS</span></span>
* <span data-ttu-id="6b3f4-254">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-254">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="6b3f4-255">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-255">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-256">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-256">Appservice</span></span>
* <span data-ttu-id="6b3f4-257">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-257">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="6b3f4-258">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="6b3f4-258">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="6b3f4-259">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="6b3f4-259">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-260">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-260">Container</span></span>
* <span data-ttu-id="6b3f4-261">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-261">Added `container start` command</span></span>
* <span data-ttu-id="6b3f4-262">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-262">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6b3f4-263">EventGrid</span><span class="sxs-lookup"><span data-stu-id="6b3f4-263">EventGrid</span></span>
* <span data-ttu-id="6b3f4-264">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-264">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="6b3f4-265">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-265">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="6b3f4-266">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-266">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="6b3f4-267">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-267">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="6b3f4-268">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-268">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6b3f4-269">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6b3f4-269">HDInsight</span></span>
* <span data-ttu-id="6b3f4-270">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-270">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="6b3f4-271">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="6b3f4-271">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="6b3f4-272">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-272">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="6b3f4-273">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-273">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="6b3f4-274">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-274">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="6b3f4-275">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-275">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-276">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-276">IoT</span></span>
* <span data-ttu-id="6b3f4-277">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="6b3f4-277">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="6b3f4-278">Kusto</span><span class="sxs-lookup"><span data-stu-id="6b3f4-278">Kusto</span></span>
* <span data-ttu-id="6b3f4-279">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-279">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-280">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-280">Monitor</span></span>
* <span data-ttu-id="6b3f4-281">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-281">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-282">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-282">Profile</span></span>
* <span data-ttu-id="6b3f4-283">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-283">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-284">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-284">Network</span></span>
* <span data-ttu-id="6b3f4-285">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-285">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="6b3f4-286">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="6b3f4-286">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-287">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-287">Resource</span></span>
* <span data-ttu-id="6b3f4-288">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-288">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="6b3f4-289">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-289">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="6b3f4-290">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-290">SQL Virtual Machine</span></span>
* <span data-ttu-id="6b3f4-291">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-291">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-292">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-292">Storage</span></span>
* <span data-ttu-id="6b3f4-293">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="6b3f4-293">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="6b3f4-294">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-294">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-295">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-295">VM</span></span>
* <span data-ttu-id="6b3f4-296">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="6b3f4-296">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="6b3f4-297">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-297">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="6b3f4-298">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="6b3f4-298">January 15, 2019</span></span>

<span data-ttu-id="6b3f4-299">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="6b3f4-299">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-300">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-300">ACR</span></span>
* <span data-ttu-id="6b3f4-301">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="6b3f4-301">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="6b3f4-302">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-302">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="6b3f4-303">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-303">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="6b3f4-304">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-304">ACS</span></span>
* <span data-ttu-id="6b3f4-305">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-305">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-306">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-306">Appservice</span></span>
* <span data-ttu-id="6b3f4-307">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-307">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="6b3f4-308">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="6b3f4-308">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="6b3f4-309">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-309">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="6b3f4-310">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-310">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="6b3f4-311">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-311">Botservice</span></span>
* <span data-ttu-id="6b3f4-312">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-312">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="6b3f4-313">Configurar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-313">Configure</span></span>
* <span data-ttu-id="6b3f4-314">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="6b3f4-314">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-315">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-315">CosmosDB</span></span>
* <span data-ttu-id="6b3f4-316">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-316">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6b3f4-317">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6b3f4-317">HDInsight</span></span>
* <span data-ttu-id="6b3f4-318">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-318">Added commands for managing applications</span></span>
* <span data-ttu-id="6b3f4-319">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="6b3f4-319">Added commands for managing script actions</span></span>
* <span data-ttu-id="6b3f4-320">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-320">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="6b3f4-321">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-321">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="6b3f4-322">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-322">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-323">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-323">Network</span></span>
* <span data-ttu-id="6b3f4-324">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-324">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="6b3f4-325">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="6b3f4-325">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="6b3f4-326">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-326">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="6b3f4-327">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-327">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-328">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-328">Role</span></span>
* <span data-ttu-id="6b3f4-329">[PRETERIDO] O argumento `--password` para `create-for-rbac` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-329">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="6b3f4-330">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-330">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="6b3f4-331">Segurança</span><span class="sxs-lookup"><span data-stu-id="6b3f4-331">Security</span></span>
* <span data-ttu-id="6b3f4-332">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-332">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-333">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-333">Storage</span></span>
* <span data-ttu-id="6b3f4-334">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-334">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="6b3f4-335">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-335">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="6b3f4-336">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-336">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="6b3f4-337">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-337">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="6b3f4-338">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-338">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-339">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-339">VM</span></span>
* <span data-ttu-id="6b3f4-340">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-340">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="6b3f4-341">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-341">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6b3f4-342">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-342">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="6b3f4-343">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-343">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="6b3f4-344">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-344">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="6b3f4-345">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-345">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="6b3f4-346">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-346">December 20, 2018</span></span>

<span data-ttu-id="6b3f4-347">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="6b3f4-347">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="6b3f4-348">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-348">Appservice</span></span>
* <span data-ttu-id="6b3f4-349">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-349">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="6b3f4-350">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="6b3f4-350">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="6b3f4-351">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-351">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6b3f4-352">IoT Central</span><span class="sxs-lookup"><span data-stu-id="6b3f4-352">IoTCentral</span></span>
* <span data-ttu-id="6b3f4-353">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-353">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-354">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-354">Role</span></span>
* <span data-ttu-id="6b3f4-355">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-355">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-356">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-356">SQL</span></span>
* <span data-ttu-id="6b3f4-357">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-357">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-358">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-358">VM</span></span>
* <span data-ttu-id="6b3f4-359">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-359">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="6b3f4-360">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-360">December 18, 2018</span></span>

<span data-ttu-id="6b3f4-361">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="6b3f4-361">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="6b3f4-362">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-362">ACR</span></span>
* <span data-ttu-id="6b3f4-363">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-363">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="6b3f4-364">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-364">Condensed the table layout for task list</span></span>
* <span data-ttu-id="6b3f4-365">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="6b3f4-365">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-366">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-366">ACS</span></span>
* <span data-ttu-id="6b3f4-367">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-367">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="6b3f4-368">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-368">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="6b3f4-369">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-369">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="6b3f4-370">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="6b3f4-370">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="6b3f4-371">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-371">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="6b3f4-372">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="6b3f4-372">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-373">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-373">Appservice</span></span>
* <span data-ttu-id="6b3f4-374">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-374">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="6b3f4-375">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-375">Botservice</span></span>
* <span data-ttu-id="6b3f4-376">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-376">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="6b3f4-377">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="6b3f4-377">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="6b3f4-378">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-378">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="6b3f4-379">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="6b3f4-379">Reduced Kudu network calls</span></span>
* <span data-ttu-id="6b3f4-380">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-380">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-381">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-381">Consumption</span></span>
* <span data-ttu-id="6b3f4-382">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="6b3f4-382">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-383">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-383">CosmosDB</span></span>
* <span data-ttu-id="6b3f4-384">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="6b3f4-384">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="6b3f4-385">Mapas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-385">Maps</span></span>
* <span data-ttu-id="6b3f4-386">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-386">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-387">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-387">Network</span></span>
* <span data-ttu-id="6b3f4-388">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-388">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="6b3f4-389">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="6b3f4-389">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-390">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-390">Resource</span></span>
* <span data-ttu-id="6b3f4-391">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-391">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="6b3f4-392">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-392">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-393">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-393">Storage</span></span>
*  <span data-ttu-id="6b3f4-394">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-394">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-395">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-395">VM</span></span>
* <span data-ttu-id="6b3f4-396">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="6b3f4-396">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="6b3f4-397">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-397">December 4, 2018</span></span>

<span data-ttu-id="6b3f4-398">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="6b3f4-398">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="6b3f4-399">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-399">Core</span></span>
* <span data-ttu-id="6b3f4-400">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="6b3f4-400">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="6b3f4-401">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-401">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-402">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-402">Appservice</span></span>
* <span data-ttu-id="6b3f4-403">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-403">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="6b3f4-404">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="6b3f4-404">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-405">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-405">Network</span></span>
* <span data-ttu-id="6b3f4-406">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="6b3f4-406">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-407">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-407">Role</span></span>
* <span data-ttu-id="6b3f4-408">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="6b3f4-408">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="6b3f4-409">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-409">VM</span></span>
* <span data-ttu-id="6b3f4-410">[PRETERIDO] Parâmetro preterido `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-410">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="6b3f4-411">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="6b3f4-411">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="6b3f4-412">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="6b3f4-412">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="6b3f4-413">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-413">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="6b3f4-414">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-414">November 20, 2018</span></span>

<span data-ttu-id="6b3f4-415">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="6b3f4-415">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="6b3f4-416">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-416">Core</span></span>
* <span data-ttu-id="6b3f4-417">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="6b3f4-417">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-418">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-418">ACR</span></span>
* <span data-ttu-id="6b3f4-419">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="6b3f4-419">Added context token to task step</span></span>
* <span data-ttu-id="6b3f4-420">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="6b3f4-420">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="6b3f4-421">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-421">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-422">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-422">Appservice</span></span>
* <span data-ttu-id="6b3f4-423">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-423">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="6b3f4-424">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-424">Updated the default `node_version`.</span></span> <span data-ttu-id="6b3f4-425">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-425">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="6b3f4-426">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-426">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="6b3f4-427">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="6b3f4-427">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="6b3f4-428">Iot Central</span><span class="sxs-lookup"><span data-stu-id="6b3f4-428">IotCentral</span></span>
* <span data-ttu-id="6b3f4-429">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="6b3f4-429">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-430">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-430">KeyVault</span></span>
* <span data-ttu-id="6b3f4-431">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-431">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-432">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-432">Network</span></span>
* <span data-ttu-id="6b3f4-433">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="6b3f4-433">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="6b3f4-434">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-434">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="6b3f4-435">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-435">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="6b3f4-436">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-436">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-437">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6b3f4-437">Rdbms</span></span>
* <span data-ttu-id="6b3f4-438">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-438">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="6b3f4-439">Rbac</span><span class="sxs-lookup"><span data-stu-id="6b3f4-439">Rbac</span></span>
* <span data-ttu-id="6b3f4-440">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-440">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="6b3f4-441">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-441">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="6b3f4-442">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-442">Storage</span></span>
* <span data-ttu-id="6b3f4-443">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-443">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="6b3f4-444">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-444">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="6b3f4-445">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-445">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="6b3f4-446">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-446">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-447">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-447">VM</span></span>
* <span data-ttu-id="6b3f4-448">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-448">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="6b3f4-449">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-449">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="6b3f4-450">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-450">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="6b3f4-451">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-451">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="6b3f4-452">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-452">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="6b3f4-453">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-453">Added `snapshot wait` command</span></span>
* <span data-ttu-id="6b3f4-454">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-454">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="6b3f4-455">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-455">November 6, 2018</span></span>

<span data-ttu-id="6b3f4-456">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="6b3f4-456">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-457">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-457">Core</span></span>
* <span data-ttu-id="6b3f4-458">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-458">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-459">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-459">ACR</span></span>
* <span data-ttu-id="6b3f4-460">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="6b3f4-460">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="6b3f4-461">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-461">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-462">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-462">ACS</span></span>
* <span data-ttu-id="6b3f4-463">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-463">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="6b3f4-464">Supervisor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-464">Advisor</span></span>
* <span data-ttu-id="6b3f4-465">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="6b3f4-465">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="6b3f4-466">AMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-466">AMS</span></span>
* <span data-ttu-id="6b3f4-467">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-467">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="6b3f4-468">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-468">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="6b3f4-469">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-469">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="6b3f4-470">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-470">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="6b3f4-471">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-471">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="6b3f4-472">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-472">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="6b3f4-473">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-473">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="6b3f4-474">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-474">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="6b3f4-475">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-475">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="6b3f4-476">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-476">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="6b3f4-477">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-477">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="6b3f4-478">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-478">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="6b3f4-479">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="6b3f4-479">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="6b3f4-480">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-480">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="6b3f4-481">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-481">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="6b3f4-482">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-482">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="6b3f4-483">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="6b3f4-483">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-484">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-484">AppService</span></span>
* <span data-ttu-id="6b3f4-485">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-485">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="6b3f4-486">Configurar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-486">Configure</span></span>
* <span data-ttu-id="6b3f4-487">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="6b3f4-487">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-488">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-488">Container</span></span>
* <span data-ttu-id="6b3f4-489">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="6b3f4-489">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="6b3f4-490">EventHub</span><span class="sxs-lookup"><span data-stu-id="6b3f4-490">EventHub</span></span>
* <span data-ttu-id="6b3f4-491">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-491">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-492">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-492">Interactive</span></span>
* <span data-ttu-id="6b3f4-493">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-493">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-494">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-494">Monitor</span></span>
* <span data-ttu-id="6b3f4-495">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-495">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-496">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-496">Network</span></span>
* <span data-ttu-id="6b3f4-497">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-497">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="6b3f4-498">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="6b3f4-498">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="6b3f4-499">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-499">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="6b3f4-500">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-500">Profile</span></span>
* <span data-ttu-id="6b3f4-501">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-501">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-502">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-502">RDBMS</span></span>
* <span data-ttu-id="6b3f4-503">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="6b3f4-503">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-504">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-504">Resource</span></span>
* <span data-ttu-id="6b3f4-505">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-505">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-506">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-506">Role</span></span>
* <span data-ttu-id="6b3f4-507">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-507">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="6b3f4-508">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-508">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="6b3f4-509">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="6b3f4-509">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-510">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-510">Storage</span></span>
* <span data-ttu-id="6b3f4-511">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-511">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-512">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-512">VM</span></span>
* <span data-ttu-id="6b3f4-513">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-513">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="6b3f4-514">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-514">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="6b3f4-515">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-515">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="6b3f4-516">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-516">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="6b3f4-517">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-517">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="6b3f4-518">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-518">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="6b3f4-519">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-519">October 23, 2018</span></span>

<span data-ttu-id="6b3f4-520">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="6b3f4-520">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-521">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-521">Core</span></span>
* <span data-ttu-id="6b3f4-522">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-522">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="6b3f4-523">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-523">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-524">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-524">ACR</span></span>
* <span data-ttu-id="6b3f4-525">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="6b3f4-525">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="6b3f4-526">CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-526">CDN</span></span>
* <span data-ttu-id="6b3f4-527">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="6b3f4-527">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="6b3f4-528">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-528">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-529">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-529">Container</span></span>
* <span data-ttu-id="6b3f4-530">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="6b3f4-530">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="6b3f4-531">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-531">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="6b3f4-532">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-532">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="6b3f4-533">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-533">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="6b3f4-534">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="6b3f4-534">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="6b3f4-535">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="6b3f4-535">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="6b3f4-536">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-536">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-537">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-537">CosmosDB</span></span>
* <span data-ttu-id="6b3f4-538">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-538">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-539">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-539">Interactive</span></span>
* <span data-ttu-id="6b3f4-540">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="6b3f4-540">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="6b3f4-541">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-541">IoT Central</span></span>
* <span data-ttu-id="6b3f4-542">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="6b3f4-542">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="6b3f4-543">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="6b3f4-543">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-544">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-544">Monitor</span></span>
* <span data-ttu-id="6b3f4-545">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-545">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="6b3f4-546">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-546">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="6b3f4-547">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6b3f4-548">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="6b3f4-549">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-549">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="6b3f4-550">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-550">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="6b3f4-551">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-551">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="6b3f4-552">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-552">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="6b3f4-553">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-553">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="6b3f4-554">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-554">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-555">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-555">Network</span></span>
* <span data-ttu-id="6b3f4-556">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="6b3f4-556">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="6b3f4-557">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="6b3f4-557">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="6b3f4-558">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6b3f4-558">ServiceBus</span></span>
* <span data-ttu-id="6b3f4-559">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-559">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-560">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-560">SQL</span></span>
* <span data-ttu-id="6b3f4-561">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="6b3f4-561">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-562">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-562">Storage</span></span>
* <span data-ttu-id="6b3f4-563">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="6b3f4-563">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="6b3f4-564">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="6b3f4-564">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-565">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-565">VM</span></span>
* <span data-ttu-id="6b3f4-566">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-566">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="6b3f4-567">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-567">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="6b3f4-568">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-568">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="6b3f4-569">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-569">October 16, 2018</span></span>

<span data-ttu-id="6b3f4-570">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="6b3f4-570">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-571">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-571">VM</span></span>
* <span data-ttu-id="6b3f4-572">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="6b3f4-572">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="6b3f4-573">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-573">October 9, 2018</span></span>

<span data-ttu-id="6b3f4-574">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="6b3f4-574">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-575">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-575">Core</span></span>
* <span data-ttu-id="6b3f4-576">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="6b3f4-576">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-577">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-577">ACR</span></span>
* <span data-ttu-id="6b3f4-578">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="6b3f4-578">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-579">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-579">ACS</span></span>
* <span data-ttu-id="6b3f4-580">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="6b3f4-580">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="6b3f4-581">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="6b3f4-581">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="6b3f4-582">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-582">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="6b3f4-583">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-583">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-584">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-584">Container</span></span>
* <span data-ttu-id="6b3f4-585">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-585">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="6b3f4-586">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-586">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="6b3f4-587">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-587">Event Hub</span></span>
* <span data-ttu-id="6b3f4-588">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-588">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="6b3f4-589">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-589">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="6b3f4-590">Extensões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-590">Extensions</span></span>
* <span data-ttu-id="6b3f4-591">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-591">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="6b3f4-592">HDInsight</span><span class="sxs-lookup"><span data-stu-id="6b3f4-592">HDInsight</span></span>
* <span data-ttu-id="6b3f4-593">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-593">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-594">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-594">IoT</span></span>
* <span data-ttu-id="6b3f4-595">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-595">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-596">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-596">KeyVault</span></span>
* <span data-ttu-id="6b3f4-597">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-597">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-598">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-598">Network</span></span>
* <span data-ttu-id="6b3f4-599">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-599">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="6b3f4-600">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="6b3f4-600">See #6052</span></span>
* <span data-ttu-id="6b3f4-601">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-601">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="6b3f4-602">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="6b3f4-602">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="6b3f4-603">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-603">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="6b3f4-604">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-604">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="6b3f4-605">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-605">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="6b3f4-606">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-606">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-607">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-607">Role</span></span>
* <span data-ttu-id="6b3f4-608">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-608">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="6b3f4-609">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-609">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="6b3f4-610">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-610">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="6b3f4-611">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="6b3f4-611">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="6b3f4-612">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-612">Service Bus</span></span>
* <span data-ttu-id="6b3f4-613">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-613">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-614">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-614">VM</span></span>
* <span data-ttu-id="6b3f4-615">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-615">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="6b3f4-616">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-616">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="6b3f4-617">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-617">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="6b3f4-618">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-618">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="6b3f4-619">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-619">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="6b3f4-620">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="6b3f4-620">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="6b3f4-621">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-621">September 21, 2018</span></span>

<span data-ttu-id="6b3f4-622">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="6b3f4-622">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-623">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-623">ACR</span></span>
* <span data-ttu-id="6b3f4-624">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-624">Added ACR Task commands</span></span>
* <span data-ttu-id="6b3f4-625">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-625">Added quick run command</span></span>
* <span data-ttu-id="6b3f4-626">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-626">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="6b3f4-627">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-627">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="6b3f4-628">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-628">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="6b3f4-629">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="6b3f4-629">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-630">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-630">ACS</span></span>
* <span data-ttu-id="6b3f4-631">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-631">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="6b3f4-632">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="6b3f4-632">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-633">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-633">AppService</span></span>

* <span data-ttu-id="6b3f4-634">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-634">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="6b3f4-635">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="6b3f4-635">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="6b3f4-636">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="6b3f4-636">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="6b3f4-637">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-637">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-638">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-638">Batch</span></span>
* <span data-ttu-id="6b3f4-639">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="6b3f4-639">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="6b3f4-640">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-640">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="6b3f4-641">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-641">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="6b3f4-642">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-642">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6b3f4-643">Lote AI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-643">Batch AI</span></span> 
* <span data-ttu-id="6b3f4-644">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-644">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6b3f4-645">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-645">Cognitive Services</span></span>
* <span data-ttu-id="6b3f4-646">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-646">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="6b3f4-647">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-647">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="6b3f4-648">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-648">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="6b3f4-649">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-649">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="6b3f4-650">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-650">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="6b3f4-651">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-651">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-652">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-652">Container</span></span>
* <span data-ttu-id="6b3f4-653">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="6b3f4-653">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="6b3f4-654">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-654">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="6b3f4-655">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="6b3f4-655">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="6b3f4-656">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-656">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="6b3f4-657">DataLake</span><span class="sxs-lookup"><span data-stu-id="6b3f4-657">Datalake</span></span>
* <span data-ttu-id="6b3f4-658">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="6b3f4-658">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="6b3f4-659">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-659">Interactive Shell</span></span>
* <span data-ttu-id="6b3f4-660">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-660">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="6b3f4-661">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-661">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-662">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-662">IoT</span></span>
* <span data-ttu-id="6b3f4-663">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-663">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="6b3f4-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-664">Key Vault</span></span>
* <span data-ttu-id="6b3f4-665">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="6b3f4-665">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-666">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-666">Network</span></span>
* <span data-ttu-id="6b3f4-667">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="6b3f4-667">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="6b3f4-668">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-668">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="6b3f4-669">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="6b3f4-669">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="6b3f4-670">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="6b3f4-670">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="6b3f4-671">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-671">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="6b3f4-672">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-672">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="6b3f4-673">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-673">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="6b3f4-674">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-674">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="6b3f4-675">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-675">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="6b3f4-676">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-676">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="6b3f4-677">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-677">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="6b3f4-678">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-678">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="6b3f4-679">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-679">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="6b3f4-680">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-680">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="6b3f4-681">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-681">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="6b3f4-682">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="6b3f4-682">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="6b3f4-683">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-683">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="6b3f4-684">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-684">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-685">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-685">RDBMS</span></span>
* <span data-ttu-id="6b3f4-686">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-686">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="6b3f4-687">Reserva</span><span class="sxs-lookup"><span data-stu-id="6b3f4-687">Reservation</span></span>
* <span data-ttu-id="6b3f4-688">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-688">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="6b3f4-689">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="6b3f4-689">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="6b3f4-690">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-690">Manage App</span></span>
* <span data-ttu-id="6b3f4-691">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="6b3f4-691">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="6b3f4-692">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="6b3f4-692">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-693">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-693">Role</span></span>
* <span data-ttu-id="6b3f4-694">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="6b3f4-694">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="6b3f4-695">SignalR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-695">SignalR</span></span>
* <span data-ttu-id="6b3f4-696">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-696">First release</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-697">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-697">Storage</span></span>
* <span data-ttu-id="6b3f4-698">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="6b3f4-698">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="6b3f4-699">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="6b3f4-699">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-700">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-700">VM</span></span>
* <span data-ttu-id="6b3f4-701">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-701">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="6b3f4-702">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-702">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="6b3f4-703">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-703">August 28, 2018</span></span>

<span data-ttu-id="6b3f4-704">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="6b3f4-704">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-705">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-705">Core</span></span>

* <span data-ttu-id="6b3f4-706">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="6b3f4-706">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="6b3f4-707">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6b3f4-707">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-708">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-708">ACR</span></span>

* <span data-ttu-id="6b3f4-709">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-709">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="6b3f4-710">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-710">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-711">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-711">ACS</span></span>

* <span data-ttu-id="6b3f4-712">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-712">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="6b3f4-713">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="6b3f4-713">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-714">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-714">AppService</span></span>

* <span data-ttu-id="6b3f4-715">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="6b3f4-715">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="6b3f4-716">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-716">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="6b3f4-717">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-717">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="6b3f4-718">Backup</span><span class="sxs-lookup"><span data-stu-id="6b3f4-718">Backup</span></span>

* <span data-ttu-id="6b3f4-719">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-719">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="6b3f4-720">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-720">Bot Service</span></span>

* <span data-ttu-id="6b3f4-721">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-721">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6b3f4-722">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-722">Cognitive Services</span></span>

* <span data-ttu-id="6b3f4-723">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="6b3f4-723">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-724">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-724">IoT</span></span>

* <span data-ttu-id="6b3f4-725">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-725">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-726">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-726">Monitor</span></span>

* <span data-ttu-id="6b3f4-727">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="6b3f4-727">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="6b3f4-728">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-728">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-729">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-729">Network</span></span>

* <span data-ttu-id="6b3f4-730">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-730">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-731">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-731">Resource</span></span>

* <span data-ttu-id="6b3f4-732">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-732">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-733">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-733">Storage</span></span>

* <span data-ttu-id="6b3f4-734">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-734">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-735">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-735">VM</span></span>

* <span data-ttu-id="6b3f4-736">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-736">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="6b3f4-737">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-737">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="6b3f4-738">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-738">Auguest 14, 2018</span></span>

<span data-ttu-id="6b3f4-739">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="6b3f4-739">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-740">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-740">Core</span></span>

* <span data-ttu-id="6b3f4-741">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-741">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="6b3f4-742">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="6b3f4-742">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="6b3f4-743">Telemetria</span><span class="sxs-lookup"><span data-stu-id="6b3f4-743">Telemetry</span></span>

* <span data-ttu-id="6b3f4-744">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="6b3f4-744">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-745">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-745">ACR</span></span>

* <span data-ttu-id="6b3f4-746">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-746">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="6b3f4-747">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-747">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-748">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-748">ACS</span></span>

* <span data-ttu-id="6b3f4-749">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-749">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="6b3f4-750">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-750">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="6b3f4-751">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-751">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="6b3f4-752">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-752">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="6b3f4-753">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="6b3f4-753">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="6b3f4-754">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-754">AppService</span></span>

* <span data-ttu-id="6b3f4-755">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-755">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="6b3f4-756">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="6b3f4-756">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="6b3f4-757">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-757">BatchAI</span></span>

* <span data-ttu-id="6b3f4-758">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-758">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="6b3f4-759">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-759">Container</span></span>

* <span data-ttu-id="6b3f4-760">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-760">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="6b3f4-761">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-761">IoT</span></span>

* <span data-ttu-id="6b3f4-762">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="6b3f4-762">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="6b3f4-763">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-763">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="6b3f4-764">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-764">Iot Central</span></span>

* <span data-ttu-id="6b3f4-765">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="6b3f4-765">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-766">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-766">KeyVault</span></span>


* <span data-ttu-id="6b3f4-767">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-767">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="6b3f4-768">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-768">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="6b3f4-769">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-769">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="6b3f4-770">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="6b3f4-770">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="6b3f4-771">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="6b3f4-771">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="6b3f4-772">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-772">Relay</span></span>

* <span data-ttu-id="6b3f4-773">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-773">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-774">Sql</span><span class="sxs-lookup"><span data-stu-id="6b3f4-774">Sql</span></span>

* <span data-ttu-id="6b3f4-775">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-775">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-776">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-776">Storage</span></span>

* <span data-ttu-id="6b3f4-777">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="6b3f4-777">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="6b3f4-778">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-778">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="6b3f4-779">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-779">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="6b3f4-780">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-780">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="6b3f4-781">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-781">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-782">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-782">VM</span></span>

* <span data-ttu-id="6b3f4-783">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-783">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="6b3f4-784">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-784">July 31, 2018</span></span>

<span data-ttu-id="6b3f4-785">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="6b3f4-785">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-786">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-786">ACR</span></span>

* <span data-ttu-id="6b3f4-787">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-787">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="6b3f4-788">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-788">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-789">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-789">ACS</span></span>

* <span data-ttu-id="6b3f4-790">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-790">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-791">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-791">Batch</span></span>

* <span data-ttu-id="6b3f4-792">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="6b3f4-792">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-793">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-793">Container</span></span>

* <span data-ttu-id="6b3f4-794">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-794">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-795">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-795">Network</span></span>

* <span data-ttu-id="6b3f4-796">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6b3f4-796">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="6b3f4-797">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-797">Resource</span></span>

* <span data-ttu-id="6b3f4-798">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-798">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="6b3f4-799">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-799">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-800">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-800">Role</span></span>

* <span data-ttu-id="6b3f4-801">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="6b3f4-801">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="6b3f4-802">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-802">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="6b3f4-803">Search</span><span class="sxs-lookup"><span data-stu-id="6b3f4-803">Search</span></span>

* <span data-ttu-id="6b3f4-804">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="6b3f4-804">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="6b3f4-805">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-805">Service Bus</span></span>

* <span data-ttu-id="6b3f4-806">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="6b3f4-806">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="6b3f4-807">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-807">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="6b3f4-808">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-808">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="6b3f4-809">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-810">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-810">Storage</span></span>

* <span data-ttu-id="6b3f4-811">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-811">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="6b3f4-812">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-812">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-813">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-813">VM</span></span>

* <span data-ttu-id="6b3f4-814">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-814">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="6b3f4-815">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-815">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="6b3f4-816">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-816">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="6b3f4-817">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-817">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="6b3f4-818">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-818">July 18, 2018</span></span>

<span data-ttu-id="6b3f4-819">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="6b3f4-819">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-820">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-820">Core</span></span>

* <span data-ttu-id="6b3f4-821">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-821">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="6b3f4-822">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="6b3f4-822">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="6b3f4-823">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-823">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-824">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-824">ACR</span></span>

* <span data-ttu-id="6b3f4-825">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="6b3f4-825">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="6b3f4-826">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-826">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="6b3f4-827">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-827">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="6b3f4-828">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-828">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-829">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-829">ACS</span></span>

* <span data-ttu-id="6b3f4-830">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="6b3f4-830">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-831">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-831">AppService</span></span>

* <span data-ttu-id="6b3f4-832">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="6b3f4-832">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-833">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-833">Batch</span></span>

* <span data-ttu-id="6b3f4-834">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6b3f4-834">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="6b3f4-835">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-835">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6b3f4-836">Lote AI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-836">Batch AI</span></span>

* <span data-ttu-id="6b3f4-837">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-837">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-838">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-838">Container</span></span>

* <span data-ttu-id="6b3f4-839">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="6b3f4-839">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="6b3f4-840">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="6b3f4-840">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-841">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-841">Network</span></span>

* <span data-ttu-id="6b3f4-842">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-842">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="6b3f4-843">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-843">Added `network nic wait`</span></span>
* <span data-ttu-id="6b3f4-844">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-844">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="6b3f4-845">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-845">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="6b3f4-846">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-846">Resource</span></span>

* <span data-ttu-id="6b3f4-847">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-847">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="6b3f4-848">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-848">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="6b3f4-849">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-849">Added `deployment wait` command</span></span>
* <span data-ttu-id="6b3f4-850">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="6b3f4-850">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-851">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-851">SQL</span></span>

* <span data-ttu-id="6b3f4-852">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-852">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="6b3f4-853">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-853">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="6b3f4-854">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-854">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-855">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-855">Storage</span></span>

* <span data-ttu-id="6b3f4-856">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="6b3f4-856">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-857">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-857">VM</span></span>

* <span data-ttu-id="6b3f4-858">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-858">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="6b3f4-859">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-859">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="6b3f4-860">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-860">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6b3f4-861">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-861">July 3, 2018</span></span>

<span data-ttu-id="6b3f4-862">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="6b3f4-862">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="6b3f4-863">AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-863">AKS</span></span>

* <span data-ttu-id="6b3f4-864">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-864">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="6b3f4-865">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-865">July 3, 2018</span></span>

<span data-ttu-id="6b3f4-866">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="6b3f4-866">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-867">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-867">Core</span></span>

* <span data-ttu-id="6b3f4-868">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-868">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-869">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-869">ACR</span></span>

* <span data-ttu-id="6b3f4-870">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-870">Added polling build status</span></span>
* <span data-ttu-id="6b3f4-871">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-871">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="6b3f4-872">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-872">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-873">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-873">ACS</span></span>

* <span data-ttu-id="6b3f4-874">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-874">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="6b3f4-875">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="6b3f4-875">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="6b3f4-876">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-876">Updated options for `aks browse` command.</span></span> <span data-ttu-id="6b3f4-877">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-877">Added `--listen-port` support</span></span>
* <span data-ttu-id="6b3f4-878">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-878">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="6b3f4-879">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="6b3f4-879">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="6b3f4-880">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-880">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-881">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-881">AppService</span></span>

* <span data-ttu-id="6b3f4-882">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-882">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="6b3f4-883">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="6b3f4-883">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="6b3f4-884">Backup</span><span class="sxs-lookup"><span data-stu-id="6b3f4-884">Backup</span></span>

* <span data-ttu-id="6b3f4-885">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-885">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="6b3f4-886">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-886">BatchAI</span></span>

* <span data-ttu-id="6b3f4-887">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-887">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="6b3f4-888">Nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-888">Cloud</span></span>

* <span data-ttu-id="6b3f4-889">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-889">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-890">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-890">Container</span></span>

* <span data-ttu-id="6b3f4-891">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="6b3f4-891">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="6b3f4-892">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-892">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="6b3f4-893">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-893">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-894">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-894">Extension</span></span>

* <span data-ttu-id="6b3f4-895">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-895">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-896">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-896">Network</span></span>

* <span data-ttu-id="6b3f4-897">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-897">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="6b3f4-898">Rdbms</span></span>

* <span data-ttu-id="6b3f4-899">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-899">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-900">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-900">Resource</span></span>

* <span data-ttu-id="6b3f4-901">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-901">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-902">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-902">VM</span></span>

* <span data-ttu-id="6b3f4-903">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="6b3f4-903">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="6b3f4-904">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-904">June 25, 2018</span></span>

<span data-ttu-id="6b3f4-905">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="6b3f4-905">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="6b3f4-906">CLI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-906">CLI</span></span>

* <span data-ttu-id="6b3f4-907">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-907">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="6b3f4-908">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-908">June 19, 2018</span></span>

<span data-ttu-id="6b3f4-909">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="6b3f4-909">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-910">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-910">Core</span></span>

* <span data-ttu-id="6b3f4-911">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-911">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-912">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-912">ACR</span></span>

* <span data-ttu-id="6b3f4-913">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="6b3f4-913">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="6b3f4-914">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-914">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-915">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-915">ACS</span></span>

* <span data-ttu-id="6b3f4-916">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-916">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="6b3f4-917">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-917">Added `--update` support</span></span>
* <span data-ttu-id="6b3f4-918">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-918">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="6b3f4-919">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-919">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="6b3f4-920">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-920">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="6b3f4-921">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-921">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="6b3f4-922">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-922">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="6b3f4-923">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-923">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-924">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-924">AppService</span></span>

* <span data-ttu-id="6b3f4-925">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="6b3f4-925">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="6b3f4-926">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-926">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-927">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-927">Batch</span></span>

* <span data-ttu-id="6b3f4-928">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-928">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6b3f4-929">Lote AI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-929">Batch AI</span></span>

* <span data-ttu-id="6b3f4-930">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-930">Added support for workspaces.</span></span> <span data-ttu-id="6b3f4-931">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-931">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="6b3f4-932">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-932">Added support for experiments.</span></span> <span data-ttu-id="6b3f4-933">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-933">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="6b3f4-934">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="6b3f4-934">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="6b3f4-935">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-935">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="6b3f4-936">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-936">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="6b3f4-937">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-937">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="6b3f4-938">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="6b3f4-938">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="6b3f4-939">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="6b3f4-939">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="6b3f4-940">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-940">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="6b3f4-941">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-941">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="6b3f4-942">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-942">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="6b3f4-943">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-943">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="6b3f4-944">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-944">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="6b3f4-945">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-945">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="6b3f4-946">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-946">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="6b3f4-947">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-947">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="6b3f4-948">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-948">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="6b3f4-949">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-949">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6b3f4-950">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-950">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="6b3f4-951">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-951">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="6b3f4-952">Mapas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-952">Maps</span></span>

* <span data-ttu-id="6b3f4-953">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-953">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-954">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-954">Network</span></span>

* <span data-ttu-id="6b3f4-955">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-955">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="6b3f4-956">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-956">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="6b3f4-957">#6502</span><span class="sxs-lookup"><span data-stu-id="6b3f4-957">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="6b3f4-958">Reservas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-958">Reservations</span></span>

* <span data-ttu-id="6b3f4-959">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-959">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="6b3f4-960">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-960">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="6b3f4-961">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-961">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="6b3f4-962">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-962">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="6b3f4-963">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-963">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="6b3f4-964">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-964">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-965">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-965">Role</span></span>

* <span data-ttu-id="6b3f4-966">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-966">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-967">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-967">SQL</span></span>

* <span data-ttu-id="6b3f4-968">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-968">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-969">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-969">Storage</span></span>

* <span data-ttu-id="6b3f4-970">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="6b3f4-970">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-971">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-971">VM</span></span>

* <span data-ttu-id="6b3f4-972">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-972">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="6b3f4-973">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-973">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="6b3f4-974">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-974">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6b3f4-975">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-975">June 13, 2018</span></span>

<span data-ttu-id="6b3f4-976">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="6b3f4-976">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-977">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-977">Core</span></span>

* <span data-ttu-id="6b3f4-978">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-978">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="6b3f4-979">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-979">June 13, 2018</span></span>

<span data-ttu-id="6b3f4-980">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="6b3f4-980">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="6b3f4-981">AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-981">AKS</span></span>

* <span data-ttu-id="6b3f4-982">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-982">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="6b3f4-983">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="6b3f4-983">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="6b3f4-984">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-984">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="6b3f4-985">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-985">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="6b3f4-986">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-986">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-987">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-987">AppService</span></span>

* <span data-ttu-id="6b3f4-988">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-988">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6b3f4-989">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-989">June 5, 2018</span></span>

<span data-ttu-id="6b3f4-990">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="6b3f4-990">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-991">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-991">Interactive</span></span>

* <span data-ttu-id="6b3f4-992">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-992">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="6b3f4-993">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-993">June 5, 2018</span></span>

<span data-ttu-id="6b3f4-994">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="6b3f4-994">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-995">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-995">Core</span></span>

* <span data-ttu-id="6b3f4-996">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-996">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="6b3f4-997">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="6b3f4-997">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-998">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-998">ACR</span></span>

* <span data-ttu-id="6b3f4-999">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="6b3f4-999">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="6b3f4-1000">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1000">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="6b3f4-1001">AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1001">AKS</span></span>

* <span data-ttu-id="6b3f4-1002">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1002">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1003">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1003">Batch</span></span>

* <span data-ttu-id="6b3f4-1004">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1004">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1005">IOT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1005">IOT</span></span>

* <span data-ttu-id="6b3f4-1006">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1006">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1007">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1007">Network</span></span>

* <span data-ttu-id="6b3f4-1008">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1008">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="6b3f4-1009">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1009">Policy Insights</span></span>

* <span data-ttu-id="6b3f4-1010">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1010">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="6b3f4-1011">ARM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1011">ARM</span></span>

* <span data-ttu-id="6b3f4-1012">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1012">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1013">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1013">SQL</span></span>

* <span data-ttu-id="6b3f4-1014">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1014">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="6b3f4-1015">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1015">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="6b3f4-1016">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1016">Storage</span></span>

* <span data-ttu-id="6b3f4-1017">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1017">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1018">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1018">VM</span></span>

* <span data-ttu-id="6b3f4-1019">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1019">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="6b3f4-1020">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1020">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="6b3f4-1021">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1021">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="6b3f4-1022">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1022">May 22, 2018</span></span>

<span data-ttu-id="6b3f4-1023">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1023">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1024">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1024">Core</span></span>

* <span data-ttu-id="6b3f4-1025">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1025">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1026">ACS</span></span>

* <span data-ttu-id="6b3f4-1027">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1027">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="6b3f4-1028">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1028">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1029">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1029">AppService</span></span>

* <span data-ttu-id="6b3f4-1030">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1030">Improved generic update commands</span></span>
* <span data-ttu-id="6b3f4-1031">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1031">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1032">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1032">Container</span></span>

* <span data-ttu-id="6b3f4-1033">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1033">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="6b3f4-1034">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1034">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1035">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1035">Extension</span></span>

* <span data-ttu-id="6b3f4-1036">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1036">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1037">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1037">Interactive</span></span>

* <span data-ttu-id="6b3f4-1038">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1038">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="6b3f4-1039">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1039">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-1040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1040">KeyVault</span></span>

* <span data-ttu-id="6b3f4-1041">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1041">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1042">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1042">Network</span></span>

* <span data-ttu-id="6b3f4-1043">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1043">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="6b3f4-1044">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1044">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1045">SQL</span></span>

* <span data-ttu-id="6b3f4-1046">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1046">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="6b3f4-1047">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1047">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="6b3f4-1048">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1048">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="6b3f4-1049">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1049">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="6b3f4-1050">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1050">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="6b3f4-1051">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1051">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="6b3f4-1052">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1052">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="6b3f4-1053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1053">`edition`.</span></span> <span data-ttu-id="6b3f4-1054">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1054">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="6b3f4-1055">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1055">`elasticPoolName`.</span></span> <span data-ttu-id="6b3f4-1056">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1056">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="6b3f4-1057">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1057">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="6b3f4-1058">`edition`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1058">`edition`.</span></span> <span data-ttu-id="6b3f4-1059">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1059">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="6b3f4-1060">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1060">`dtu`.</span></span> <span data-ttu-id="6b3f4-1061">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1061">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="6b3f4-1062">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1062">`databaseDtuMin`.</span></span> <span data-ttu-id="6b3f4-1063">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1063">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="6b3f4-1064">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1064">`databaseDtuMax`.</span></span> <span data-ttu-id="6b3f4-1065">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1065">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="6b3f4-1066">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1066">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="6b3f4-1067">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1067">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1068">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1068">Storage</span></span>

* <span data-ttu-id="6b3f4-1069">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1069">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="6b3f4-1070">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1070">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1071">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1071">VM</span></span>

* <span data-ttu-id="6b3f4-1072">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1072">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="6b3f4-1073">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1073">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="6b3f4-1074">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1074">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="6b3f4-1075">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1075">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="6b3f4-1076">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1076">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="6b3f4-1077">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1077">May 7, 2018</span></span>

<span data-ttu-id="6b3f4-1078">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1078">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1079">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1079">Core</span></span>

* <span data-ttu-id="6b3f4-1080">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1080">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="6b3f4-1081">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1081">Added limited support for positional arguments</span></span>
* <span data-ttu-id="6b3f4-1082">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1082">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="6b3f4-1083">#5591</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1083">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="6b3f4-1084">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1084">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="6b3f4-1085">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1085">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="6b3f4-1086">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1086">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="6b3f4-1087">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1087">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="6b3f4-1088">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1088">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1089">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1089">ACR</span></span>

* <span data-ttu-id="6b3f4-1090">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1090">Added ACR Build commands</span></span>
* <span data-ttu-id="6b3f4-1091">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1091">Improved resource not found error messages</span></span>
* <span data-ttu-id="6b3f4-1092">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1092">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="6b3f4-1093">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1093">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="6b3f4-1094">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1094">Improved repository commands error messages</span></span>
* <span data-ttu-id="6b3f4-1095">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1095">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1096">ACS</span></span>

* <span data-ttu-id="6b3f4-1097">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1097">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="6b3f4-1098">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1098">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="6b3f4-1099">AMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1099">AMS</span></span>

* <span data-ttu-id="6b3f4-1100">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1100">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1101">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1101">Appservice</span></span>

* <span data-ttu-id="6b3f4-1102">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1102">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="6b3f4-1103">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1103">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="6b3f4-1104">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1104">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="6b3f4-1105">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1105">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="6b3f4-1106">Lote AI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1106">Batch AI</span></span>

* <span data-ttu-id="6b3f4-1107">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1107">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6b3f4-1108">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1108">Cognitive Services</span></span>

* <span data-ttu-id="6b3f4-1109">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1109">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-1110">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1110">Consumption</span></span>

* <span data-ttu-id="6b3f4-1111">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1111">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1112">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1112">Container</span></span>

* <span data-ttu-id="6b3f4-1113">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1113">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="6b3f4-1114">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1114">Cosmos DB</span></span>

* <span data-ttu-id="6b3f4-1115">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1115">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="6b3f4-1116">DMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1116">DMS</span></span>

* <span data-ttu-id="6b3f4-1117">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1117">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1118">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1118">Extension</span></span>

* <span data-ttu-id="6b3f4-1119">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1119">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1120">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1120">Interactive</span></span>

* <span data-ttu-id="6b3f4-1121">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1121">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="6b3f4-1122">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1122">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="6b3f4-1123">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1123">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="6b3f4-1124">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1124">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="6b3f4-1125">Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1125">Lab</span></span>

* <span data-ttu-id="6b3f4-1126">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1126">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1127">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1127">Network</span></span>

* <span data-ttu-id="6b3f4-1128">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1128">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="6b3f4-1129">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1129">Profile</span></span>

* <span data-ttu-id="6b3f4-1130">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1130">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="6b3f4-1131">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1131">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="6b3f4-1132">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1132">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="6b3f4-1133">Redis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1133">Redis</span></span>

* <span data-ttu-id="6b3f4-1134">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1134">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="6b3f4-1135">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1135">Deprecated `redis list-all`.</span></span> <span data-ttu-id="6b3f4-1136">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1136">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="6b3f4-1137">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1137">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="6b3f4-1138">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1138">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-1139">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1139">Role</span></span>

* <span data-ttu-id="6b3f4-1140">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1140">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1141">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1141">Storage</span></span>

* <span data-ttu-id="6b3f4-1142">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1142">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="6b3f4-1143">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1143">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="6b3f4-1144">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1144">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="6b3f4-1145">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1145">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="6b3f4-1146">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1146">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1147">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1147">VM</span></span>

* <span data-ttu-id="6b3f4-1148">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1148">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="6b3f4-1149">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1149">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="6b3f4-1150">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1150">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="6b3f4-1151">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1151">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="6b3f4-1152">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1152">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="6b3f4-1153">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1153">Added write accelerator support</span></span>
* <span data-ttu-id="6b3f4-1154">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1154">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="6b3f4-1155">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1155">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="6b3f4-1156">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1156">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="6b3f4-1157">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1157">April 10, 2018</span></span>

<span data-ttu-id="6b3f4-1158">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1158">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1159">ACR</span></span>

* <span data-ttu-id="6b3f4-1160">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1160">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1161">ACS</span></span>

* <span data-ttu-id="6b3f4-1162">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1162">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1163">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1163">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="6b3f4-1165">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1165">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="6b3f4-1166">BatchAI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1166">BatchAI</span></span>

* <span data-ttu-id="6b3f4-1167">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1167">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="6b3f4-1168">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1168">Job level mounting</span></span>
  - <span data-ttu-id="6b3f4-1169">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1169">Environment variables with secret values</span></span>
  - <span data-ttu-id="6b3f4-1170">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1170">Performance counters settings</span></span>
  - <span data-ttu-id="6b3f4-1171">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1171">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="6b3f4-1172">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1172">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="6b3f4-1173">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1173">Usage and limits reporting</span></span>
  - <span data-ttu-id="6b3f4-1174">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1174">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="6b3f4-1175">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1175">Support for custom images</span></span>
  - <span data-ttu-id="6b3f4-1176">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1176">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="6b3f4-1177">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1177">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="6b3f4-1178">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1178">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="6b3f4-1179">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1179">National clouds are supported</span></span>
* <span data-ttu-id="6b3f4-1180">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1180">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="6b3f4-1181">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1181">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="6b3f4-1182">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1182">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="6b3f4-1183">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1183">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="6b3f4-1184">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1184">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="6b3f4-1185">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1185">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="6b3f4-1186">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1186">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="6b3f4-1187">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1187">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="6b3f4-1188">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1188">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="6b3f4-1189">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1189">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="6b3f4-1190">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1190">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="6b3f4-1191">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1191">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="6b3f4-1192">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1192">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="6b3f4-1193">Cobrança</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1193">Billing</span></span>

* <span data-ttu-id="6b3f4-1194">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1194">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-1195">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1195">Consumption</span></span>

* <span data-ttu-id="6b3f4-1196">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1196">Added `marketplace` commands</span></span>
* <span data-ttu-id="6b3f4-1197">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1197">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="6b3f4-1198">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1198">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="6b3f4-1199">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1199">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="6b3f4-1200">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1200">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="6b3f4-1201">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1201">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1202">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1202">Container</span></span>

* <span data-ttu-id="6b3f4-1203">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1203">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="6b3f4-1204">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1204">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1205">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1205">Extension</span></span>

* <span data-ttu-id="6b3f4-1206">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1206">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1207">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1207">Interactive</span></span>

* <span data-ttu-id="6b3f4-1208">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1208">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="6b3f4-1209">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1209">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="6b3f4-1210">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1210">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1211">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1211">Network</span></span>

* <span data-ttu-id="6b3f4-1212">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1212">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="6b3f4-1213">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1213">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="6b3f4-1214">#4910</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1214">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="6b3f4-1215">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1215">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="6b3f4-1216">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1216">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="6b3f4-1217">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1217">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1218">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1218">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1219">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1219">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1220">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1220">Profile</span></span>

* <span data-ttu-id="6b3f4-1221">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1221">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="6b3f4-1222">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1222">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-1223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1223">RDBMS</span></span>

* <span data-ttu-id="6b3f4-1224">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1224">Added `georestore` command</span></span>
* <span data-ttu-id="6b3f4-1225">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1225">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1226">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1226">Resource</span></span>

* <span data-ttu-id="6b3f4-1227">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1227">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="6b3f4-1228">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1228">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1229">SQL</span></span>

* <span data-ttu-id="6b3f4-1230">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1230">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1231">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1231">Storage</span></span>

* <span data-ttu-id="6b3f4-1232">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1232">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1233">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1233">VM</span></span>

* <span data-ttu-id="6b3f4-1234">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1234">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="6b3f4-1235">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1235">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="6b3f4-1237">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1237">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="6b3f4-1238">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1238">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="6b3f4-1239">#5718</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1239">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="6b3f4-1240">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1240">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="6b3f4-1241">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1241">March 27, 2018</span></span>

<span data-ttu-id="6b3f4-1242">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1242">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1243">Core</span></span>

* <span data-ttu-id="6b3f4-1244">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1244">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1245">ACS</span></span>

* <span data-ttu-id="6b3f4-1246">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1246">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1247">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1247">Appservice</span></span>

* <span data-ttu-id="6b3f4-1248">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1248">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="6b3f4-1249">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1249">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6b3f4-1250">Backup</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1250">Backup</span></span>

* <span data-ttu-id="6b3f4-1251">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1251">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="6b3f4-1252">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1252">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="6b3f4-1253">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1253">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
  * `backup container show`
  * `backup item set-policy`
  * `backup item show`
  * `backup job show`
  * `backup job stop`
  * `backup job wait`
  * `backup policy delete`
  * `backup policy get-default-for-vm`
  * `backup policy list-associated-items`
  * `backup policy set`
  * `backup policy show`
  * `backup protection backup-now`
  * `backup protection disable`
  * `backup protection enable-for-vm`
  * `backup recoverypoint show`
  * `backup restore files mount-rp`
  * `backup restore files unmount-rp`
  * `backup restore restore-disks`
  * `backup vault delete`
  * `backup vault show`
* <span data-ttu-id="6b3f4-1254">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1254">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1255">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1255">Container</span></span>

* <span data-ttu-id="6b3f4-1256">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1256">Added `container exec` command.</span></span> <span data-ttu-id="6b3f4-1257">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1257">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="6b3f4-1258">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1258">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1259">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1259">Extension</span></span>

* <span data-ttu-id="6b3f4-1260">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1260">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="6b3f4-1261">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1261">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="6b3f4-1262">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1262">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1263">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1263">Interactive</span></span>

* <span data-ttu-id="6b3f4-1264">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1264">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="6b3f4-1265">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1265">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="6b3f4-1266">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1266">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="6b3f4-1267">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1267">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="6b3f4-1268">Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1268">Lab</span></span>

* <span data-ttu-id="6b3f4-1269">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1269">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1270">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1270">Monitor</span></span>

* <span data-ttu-id="6b3f4-1271">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1271">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="6b3f4-1272">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1272">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="6b3f4-1273">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1273">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1274">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1274">Network</span></span>

* <span data-ttu-id="6b3f4-1275">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1275">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1276">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1276">Profile</span></span>

* <span data-ttu-id="6b3f4-1277">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1277">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-1278">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1278">RDBMS</span></span>

* <span data-ttu-id="6b3f4-1279">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1279">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1280">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1280">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="6b3f4-1282">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1282">Role</span></span>

* <span data-ttu-id="6b3f4-1283">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1283">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="6b3f4-1284">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1284">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="6b3f4-1285">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1285">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="6b3f4-1286">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1286">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="6b3f4-1287">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1287">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1288">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1288">Storage</span></span>

* <span data-ttu-id="6b3f4-1289">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1289">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="6b3f4-1290">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1290">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1291">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1291">VM</span></span>

* <span data-ttu-id="6b3f4-1292">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1292">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="6b3f4-1293">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1293">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="6b3f4-1294">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1294">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="6b3f4-1295">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1295">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="6b3f4-1296">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1296">March 13, 2018</span></span>

<span data-ttu-id="6b3f4-1297">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1297">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1298">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1298">ACR</span></span>

* <span data-ttu-id="6b3f4-1299">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1299">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="6b3f4-1300">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1300">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="6b3f4-1301">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1301">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1302">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1302">ACS</span></span>

* <span data-ttu-id="6b3f4-1303">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1303">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="6b3f4-1304">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1304">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="6b3f4-1305">Supervisor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1305">Advisor</span></span>

* <span data-ttu-id="6b3f4-1306">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1306">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="6b3f4-1307">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1307">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="6b3f4-1308">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1308">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="6b3f4-1309">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1309">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="6b3f4-1310">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1310">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1311">Appservice</span></span>

* <span data-ttu-id="6b3f4-1312">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1312">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="6b3f4-1313">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1313">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="6b3f4-1314">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1314">Eventhubs</span></span>

* <span data-ttu-id="6b3f4-1315">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1315">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1316">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1316">Extension</span></span>

* <span data-ttu-id="6b3f4-1317">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1317">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1318">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1318">Interactive</span></span>

* <span data-ttu-id="6b3f4-1319">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1319">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="6b3f4-1320">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1320">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="6b3f4-1321">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1321">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="6b3f4-1322">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1322">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1323">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1323">Monitor</span></span>

* <span data-ttu-id="6b3f4-1324">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1324">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="6b3f4-1325">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1325">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="6b3f4-1326">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1326">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="6b3f4-1327">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1327">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1328">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1328">Network</span></span>

* <span data-ttu-id="6b3f4-1329">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1329">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="6b3f4-1330">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1330">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="6b3f4-1331">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1331">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="6b3f4-1332">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1332">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1333">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1333">Profile</span></span>

* <span data-ttu-id="6b3f4-1334">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1334">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="6b3f4-1335">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1335">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-1336">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1336">RDBMS</span></span>

* <span data-ttu-id="6b3f4-1337">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1337">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="6b3f4-1338">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1338">Service Bus</span></span>

* <span data-ttu-id="6b3f4-1339">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1339">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1340">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1340">Storage</span></span>

* <span data-ttu-id="6b3f4-1341">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1341">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="6b3f4-1342">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1342">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1343">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1343">VM</span></span>

* <span data-ttu-id="6b3f4-1344">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1344">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="6b3f4-1345">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1345">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="6b3f4-1346">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1346">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="6b3f4-1347">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1347">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="6b3f4-1348">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1348">February 27, 2018</span></span>

<span data-ttu-id="6b3f4-1349">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1349">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1350">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1350">Core</span></span>

* <span data-ttu-id="6b3f4-1351">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1351">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="6b3f4-1352">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1352">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="6b3f4-1353">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1353">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1354">ACS</span></span>

* <span data-ttu-id="6b3f4-1355">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1355">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="6b3f4-1356">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1356">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="6b3f4-1357">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1357">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="6b3f4-1358">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1358">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1359">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1359">Appservice</span></span>

* <span data-ttu-id="6b3f4-1360">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1360">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="6b3f4-1361">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1361">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="6b3f4-1362">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1362">Cognitive Services</span></span>

* <span data-ttu-id="6b3f4-1363">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1363">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-1364">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1364">Consumption</span></span>

* <span data-ttu-id="6b3f4-1365">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1365">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="6b3f4-1366">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1366">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1367">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1367">Container</span></span>

* <span data-ttu-id="6b3f4-1368">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1368">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1369">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1369">Network</span></span>

* <span data-ttu-id="6b3f4-1370">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1370">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1371">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1371">Resource</span></span>

* <span data-ttu-id="6b3f4-1372">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1372">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-1373">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1373">Role</span></span>

* <span data-ttu-id="6b3f4-1374">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1374">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1375">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1375">SQL</span></span>

* <span data-ttu-id="6b3f4-1376">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1376">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1377">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1377">Storage</span></span>

* <span data-ttu-id="6b3f4-1378">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1378">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1379">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1379">VM</span></span>

* <span data-ttu-id="6b3f4-1380">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1380">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="6b3f4-1381">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1381">February 13, 2018</span></span>

<span data-ttu-id="6b3f4-1382">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1382">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1383">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1383">Core</span></span>

* <span data-ttu-id="6b3f4-1384">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1384">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1385">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1385">ACS</span></span>

* <span data-ttu-id="6b3f4-1386">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1386">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="6b3f4-1387">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1387">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="6b3f4-1388">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1388">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="6b3f4-1389">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1389">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="6b3f4-1390">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1390">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="6b3f4-1391">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1391">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="6b3f4-1392">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1392">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="6b3f4-1393">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1393">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1394">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1394">Appservice</span></span>

* <span data-ttu-id="6b3f4-1395">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1395">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="6b3f4-1396">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1396">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="6b3f4-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1397">CDN</span></span>

* <span data-ttu-id="6b3f4-1398">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1398">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1399">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1399">Container</span></span>

* <span data-ttu-id="6b3f4-1400">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1400">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="6b3f4-1401">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1401">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-1402">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1402">CosmosDB</span></span>

* <span data-ttu-id="6b3f4-1403">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1403">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1404">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1404">Extension</span></span>

* <span data-ttu-id="6b3f4-1405">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1405">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="6b3f4-1406">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1406">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="6b3f4-1407">Comentários</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1407">Feedback</span></span>

* <span data-ttu-id="6b3f4-1408">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1408">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1409">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1409">Interactive</span></span>

* <span data-ttu-id="6b3f4-1410">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1410">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="6b3f4-1411">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1411">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1412">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1412">IoT</span></span>

* <span data-ttu-id="6b3f4-1413">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1413">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6b3f4-1414">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1414">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="6b3f4-1415">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1415">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1416">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1416">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1417">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1417">Monitor</span></span>

* <span data-ttu-id="6b3f4-1418">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1418">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1419">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1419">Network</span></span>

* <span data-ttu-id="6b3f4-1420">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1420">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="6b3f4-1421">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1421">Profile</span></span>

* <span data-ttu-id="6b3f4-1422">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1422">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1423">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1423">Resource</span></span>

* <span data-ttu-id="6b3f4-1424">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1424">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-1425">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1425">Role</span></span>

* <span data-ttu-id="6b3f4-1426">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1426">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1427">SQL</span></span>

* <span data-ttu-id="6b3f4-1428">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1428">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="6b3f4-1429">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1429">Added `sql db rename`</span></span>
* <span data-ttu-id="6b3f4-1430">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1430">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1431">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1431">Storage</span></span>

* <span data-ttu-id="6b3f4-1432">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1432">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1433">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1433">VM</span></span>

* <span data-ttu-id="6b3f4-1434">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1434">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="6b3f4-1435">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1435">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="6b3f4-1436">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1436">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="6b3f4-1437">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1437">January 31, 2018</span></span>

<span data-ttu-id="6b3f4-1438">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1438">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1439">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1439">Core</span></span>

* <span data-ttu-id="6b3f4-1440">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1440">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="6b3f4-1441">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1441">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="6b3f4-1442">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1442">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="6b3f4-1443">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1443">Use `--verbose` to see</span></span>
* <span data-ttu-id="6b3f4-1444">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1444">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1445">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1445">ACS</span></span>

* <span data-ttu-id="6b3f4-1446">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1446">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="6b3f4-1447">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1447">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1448">Appservice</span></span>

* <span data-ttu-id="6b3f4-1449">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1449">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="6b3f4-1450">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1450">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="6b3f4-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1451">CDN</span></span>

* <span data-ttu-id="6b3f4-1452">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1452">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-1453">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1453">CosmosDB</span></span>

* <span data-ttu-id="6b3f4-1454">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1454">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1455">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1455">Interactive</span></span>

* <span data-ttu-id="6b3f4-1456">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1456">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1457">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1457">Network</span></span>

* <span data-ttu-id="6b3f4-1458">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1458">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="6b3f4-1459">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1459">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="6b3f4-1460">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1460">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="6b3f4-1461">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1461">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="6b3f4-1462">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1462">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="6b3f4-1463">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1463">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="6b3f4-1464">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1464">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="6b3f4-1465">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1465">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="6b3f4-1466">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1466">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="6b3f4-1467">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1467">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1468">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1468">Profile</span></span>

* <span data-ttu-id="6b3f4-1469">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1469">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1470">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1470">Resource</span></span>

* <span data-ttu-id="6b3f4-1471">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1471">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1472">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1472">Storage</span></span>

* <span data-ttu-id="6b3f4-1473">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1473">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="6b3f4-1474">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1474">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="6b3f4-1475">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1475">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="6b3f4-1476">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1476">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="6b3f4-1477">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1477">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1478">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1478">VM</span></span>

* <span data-ttu-id="6b3f4-1479">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1479">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="6b3f4-1480">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1480">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="6b3f4-1481">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1481">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="6b3f4-1482">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1482">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="6b3f4-1483">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1483">January 17, 2018</span></span>

<span data-ttu-id="6b3f4-1484">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1484">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1485">ACR</span></span>

* <span data-ttu-id="6b3f4-1486">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1486">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="6b3f4-1487">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1487">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1488">ACS</span></span>

* <span data-ttu-id="6b3f4-1489">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1489">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="6b3f4-1490">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1490">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1491">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1491">Appservice</span></span>

* <span data-ttu-id="6b3f4-1492">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1492">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="6b3f4-1493">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1493">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="6b3f4-1494">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1494">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="6b3f4-1495">Backup</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1495">Backup</span></span>

* <span data-ttu-id="6b3f4-1496">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1496">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="6b3f4-1497">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1497">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="6b3f4-1498">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1498">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="6b3f4-1499">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1499">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="6b3f4-1500">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1500">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1501">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1501">Batch</span></span>

* <span data-ttu-id="6b3f4-1502">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1502">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="6b3f4-1503">Nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1503">Cloud</span></span>

* <span data-ttu-id="6b3f4-1504">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1504">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-1505">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1505">Consumption</span></span>

* <span data-ttu-id="6b3f4-1506">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1506">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="6b3f4-1507">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1507">Event Grid</span></span>

* <span data-ttu-id="6b3f4-1508">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1508">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6b3f4-1509">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1509">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="6b3f4-1510">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1510">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="6b3f4-1511">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="6b3f4-1512">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1512">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="6b3f4-1513">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1513">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="6b3f4-1514">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1514">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="6b3f4-1515">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1515">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1516">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1516">Interactive</span></span>

* <span data-ttu-id="6b3f4-1517">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1517">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="6b3f4-1518">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1518">Fixed errors on startup</span></span>
* <span data-ttu-id="6b3f4-1519">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1519">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1520">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1520">IoT</span></span>

* <span data-ttu-id="6b3f4-1521">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1521">Added support for device provisioning service</span></span>
* <span data-ttu-id="6b3f4-1522">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1522">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="6b3f4-1523">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1523">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1524">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1524">Monitor</span></span>

* <span data-ttu-id="6b3f4-1525">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1525">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="6b3f4-1526">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1526">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="6b3f4-1527">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1527">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1528">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1528">Network</span></span>

* <span data-ttu-id="6b3f4-1529">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1529">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="6b3f4-1530">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1530">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1531">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1531">Profile</span></span>

* <span data-ttu-id="6b3f4-1532">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1532">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-1533">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1533">Role</span></span>

* <span data-ttu-id="6b3f4-1534">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1534">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6b3f4-1535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1535">Service Fabric</span></span>

* <span data-ttu-id="6b3f4-1536">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1536">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="6b3f4-1537">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1537">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1538">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1538">VM</span></span>

* <span data-ttu-id="6b3f4-1539">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1539">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="6b3f4-1540">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1540">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="6b3f4-1541">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1541">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="6b3f4-1542">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1542">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="6b3f4-1543">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1543">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="6b3f4-1544">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1544">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="6b3f4-1545">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1545">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="6b3f4-1546">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1546">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="6b3f4-1547">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1547">December 19, 2017</span></span>

<span data-ttu-id="6b3f4-1548">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1548">Version 2.0.23</span></span>

* <span data-ttu-id="6b3f4-1549">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1549">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1550">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1550">Container</span></span>

* <span data-ttu-id="6b3f4-1551">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1551">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1552">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1552">Network</span></span>

* <span data-ttu-id="6b3f4-1553">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1553">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1554">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1554">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1555">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1555">Storage</span></span>

* <span data-ttu-id="6b3f4-1556">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1556">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1557">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1557">VM</span></span>

* <span data-ttu-id="6b3f4-1558">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1558">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="6b3f4-1559">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1559">December 5, 2017</span></span>

<span data-ttu-id="6b3f4-1560">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1560">Version 2.0.22</span></span>

* <span data-ttu-id="6b3f4-1561">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1561">Removed `az component` commands.</span></span> <span data-ttu-id="6b3f4-1562">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1562">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1563">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1563">Core</span></span>
* <span data-ttu-id="6b3f4-1564">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1564">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="6b3f4-1565">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1565">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1566">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1566">ACS</span></span>

* <span data-ttu-id="6b3f4-1567">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1567">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="6b3f4-1568">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1568">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="6b3f4-1569">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1569">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="6b3f4-1570">Supervisor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1570">Advisor</span></span>

* <span data-ttu-id="6b3f4-1571">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1571">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1572">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1572">Appservice</span></span>

* <span data-ttu-id="6b3f4-1573">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1573">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="6b3f4-1574">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1574">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="6b3f4-1575">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1575">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="6b3f4-1576">Consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1576">Consumption</span></span>

* <span data-ttu-id="6b3f4-1577">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1577">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1578">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1578">Container</span></span>

* <span data-ttu-id="6b3f4-1579">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1579">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1580">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1580">Monitor</span></span>

* <span data-ttu-id="6b3f4-1581">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1581">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1582">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1582">Resource</span></span>

* <span data-ttu-id="6b3f4-1583">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1583">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-1584">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1584">Role</span></span>

* <span data-ttu-id="6b3f4-1585">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1585">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="6b3f4-1586">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1586">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="6b3f4-1587">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1587">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1588">SQL</span></span>

* <span data-ttu-id="6b3f4-1589">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1589">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="6b3f4-1590">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1590">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1591">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1591">VM</span></span>

* <span data-ttu-id="6b3f4-1592">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1592">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="6b3f4-1593">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1593">November 14, 2017</span></span>

<span data-ttu-id="6b3f4-1594">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1594">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1595">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1595">ACR</span></span>

* <span data-ttu-id="6b3f4-1596">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1596">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="6b3f4-1597">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1597">ACS</span></span>

* <span data-ttu-id="6b3f4-1598">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1598">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="6b3f4-1599">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1599">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="6b3f4-1600">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1600">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="6b3f4-1601">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1601">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="6b3f4-1602">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1602">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1603">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1603">Appservice</span></span>

* <span data-ttu-id="6b3f4-1604">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1604">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="6b3f4-1605">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1605">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="6b3f4-1606">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1606">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="6b3f4-1607">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1607">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="6b3f4-1608">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1608">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="6b3f4-1609">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1609">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1610">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1610">Batch</span></span>

* <span data-ttu-id="6b3f4-1611">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1611">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="6b3f4-1612">Batchai</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1612">Batchai</span></span>

* <span data-ttu-id="6b3f4-1613">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1613">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="6b3f4-1614">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1614">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="6b3f4-1615">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1615">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="6b3f4-1616">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1616">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="6b3f4-1617">Nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1617">Cloud</span></span>

* <span data-ttu-id="6b3f4-1618">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1618">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1619">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1619">Container</span></span>

* <span data-ttu-id="6b3f4-1620">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1620">Added support to open multiple ports</span></span>
* <span data-ttu-id="6b3f4-1621">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1621">Added container group restart policy</span></span>
* <span data-ttu-id="6b3f4-1622">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1622">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="6b3f4-1623">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1623">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6b3f4-1624">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1624">Data Lake Analytics</span></span>

* <span data-ttu-id="6b3f4-1625">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1625">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6b3f4-1626">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1626">Data Lake Store</span></span>

* <span data-ttu-id="6b3f4-1627">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1627">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1628">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1628">Extension</span></span>

* <span data-ttu-id="6b3f4-1629">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1629">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="6b3f4-1630">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1630">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1631">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1631">IoT</span></span>

* <span data-ttu-id="6b3f4-1632">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1632">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1633">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1633">Monitor</span></span>

* <span data-ttu-id="6b3f4-1634">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1634">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1635">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1635">Network</span></span>

* <span data-ttu-id="6b3f4-1636">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1636">Added support for CAA DNS records</span></span>
* <span data-ttu-id="6b3f4-1637">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1637">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="6b3f4-1638">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1638">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="6b3f4-1639">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1639">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="6b3f4-1640">Reservas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1640">Reservations</span></span>

* <span data-ttu-id="6b3f4-1641">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1641">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1642">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1642">Resource</span></span>

* <span data-ttu-id="6b3f4-1643">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1643">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1644">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1644">SQL</span></span>

* <span data-ttu-id="6b3f4-1645">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1645">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1646">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1646">Storage</span></span>

* <span data-ttu-id="6b3f4-1647">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1647">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="6b3f4-1648">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1648">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="6b3f4-1649">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1649">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="6b3f4-1650">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1650">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="6b3f4-1651">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1651">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="6b3f4-1652">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1652">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="6b3f4-1653">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1653">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1654">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1654">VM</span></span>

* <span data-ttu-id="6b3f4-1655">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1655">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="6b3f4-1656">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1656">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="6b3f4-1657">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1657">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="6b3f4-1658">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1658">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="6b3f4-1659">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1659">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="6b3f4-1660">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1660">October 24, 2017</span></span>

<span data-ttu-id="6b3f4-1661">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1661">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1662">Core</span></span>

* <span data-ttu-id="6b3f4-1663">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1663">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1664">ACR</span></span>

* <span data-ttu-id="6b3f4-1665">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1665">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="6b3f4-1666">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1666">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="6b3f4-1667">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1667">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1668">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1668">ACS</span></span>

* <span data-ttu-id="6b3f4-1669">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1669">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="6b3f4-1670">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1670">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1671">Appservice</span></span>

* <span data-ttu-id="6b3f4-1672">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1672">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="6b3f4-1673">Componente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1673">Component</span></span>

* <span data-ttu-id="6b3f4-1674">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1674">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1675">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1675">Monitor</span></span>

* <span data-ttu-id="6b3f4-1676">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1676">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1677">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1677">Resource</span></span>

* <span data-ttu-id="6b3f4-1678">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1678">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="6b3f4-1679">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1679">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1680">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1680">VM</span></span>

* <span data-ttu-id="6b3f4-1681">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1681">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="6b3f4-1682">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1682">October 9, 2017</span></span>

<span data-ttu-id="6b3f4-1683">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1683">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1684">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1684">Core</span></span>

* <span data-ttu-id="6b3f4-1685">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1685">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1686">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1686">Appservice</span></span>

* <span data-ttu-id="6b3f4-1687">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1687">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1688">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1688">Batch</span></span>

* <span data-ttu-id="6b3f4-1689">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1689">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="6b3f4-1690">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1690">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="6b3f4-1691">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1691">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="6b3f4-1692">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1692">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="6b3f4-1693">Batchai</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1693">Batchai</span></span>

* <span data-ttu-id="6b3f4-1694">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1694">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-1695">Keyvault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1695">Keyvault</span></span>

* <span data-ttu-id="6b3f4-1696">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1696">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="6b3f4-1697">(#4448)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1697">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="6b3f4-1698">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1698">Network</span></span>

* <span data-ttu-id="6b3f4-1699">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1699">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="6b3f4-1700">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1700">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1701">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1701">Resource</span></span>

* <span data-ttu-id="6b3f4-1702">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1702">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="6b3f4-1703">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1703">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="6b3f4-1704">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1704">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="6b3f4-1705">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1705">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1706">Sql</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1706">Sql</span></span>

* <span data-ttu-id="6b3f4-1707">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1707">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="6b3f4-1708">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1708">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="6b3f4-1709">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1709">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1710">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1710">Storage</span></span>

* <span data-ttu-id="6b3f4-1711">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1711">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1712">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1712">Vm</span></span>

* <span data-ttu-id="6b3f4-1713">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1713">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="6b3f4-1714">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1714">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="6b3f4-1715">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1715">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="6b3f4-1716">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1716">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="6b3f4-1717">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1717">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="6b3f4-1718">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1718">September 22, 2017</span></span>

<span data-ttu-id="6b3f4-1719">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1719">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1720">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1720">Resource</span></span>

* <span data-ttu-id="6b3f4-1721">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1721">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="6b3f4-1722">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1722">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="6b3f4-1723">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1723">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="6b3f4-1724">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1724">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1725">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1725">Network</span></span>

* <span data-ttu-id="6b3f4-1726">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1726">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="6b3f4-1727">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1727">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="6b3f4-1728">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1728">Added `asg` application security group commands</span></span>
* <span data-ttu-id="6b3f4-1729">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1729">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="6b3f4-1730">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1730">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1731">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1731">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1732">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1732">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1733">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1733">Storage</span></span>

* <span data-ttu-id="6b3f4-1734">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1734">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="6b3f4-1735">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1735">Eventgrid</span></span>

* <span data-ttu-id="6b3f4-1736">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1736">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1737">SQL</span></span>

* <span data-ttu-id="6b3f4-1738">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1738">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="6b3f4-1739">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1739">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="6b3f4-1740">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1740">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-1741">Keyvault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1741">Keyvault</span></span>

* <span data-ttu-id="6b3f4-1742">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1742">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1743">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1743">VM</span></span>

* <span data-ttu-id="6b3f4-1744">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1744">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="6b3f4-1745">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1745">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="6b3f4-1746">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1746">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="6b3f4-1747">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1747">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="6b3f4-1748">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1748">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="6b3f4-1749">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1749">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1750">ACS</span></span>

* <span data-ttu-id="6b3f4-1751">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1751">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1752">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1752">Appservice</span></span>

* <span data-ttu-id="6b3f4-1753">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1753">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="6b3f4-1754">Backup</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1754">Backup</span></span>

* <span data-ttu-id="6b3f4-1755">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1755">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="6b3f4-1756">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1756">September 11, 2017</span></span>

<span data-ttu-id="6b3f4-1757">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1757">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="6b3f4-1758">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1758">Core</span></span>

* <span data-ttu-id="6b3f4-1759">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1759">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="6b3f4-1760">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1760">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1761">Acs</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1761">Acs</span></span>

* <span data-ttu-id="6b3f4-1762">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1762">Added `acs list-locations` command</span></span>
* <span data-ttu-id="6b3f4-1763">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1763">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1764">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1764">Appservice</span></span>

* <span data-ttu-id="6b3f4-1765">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1765">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="6b3f4-1766">CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1766">CDN</span></span>

* <span data-ttu-id="6b3f4-1767">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1767">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="6b3f4-1768">Extensão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1768">Extension</span></span>

* <span data-ttu-id="6b3f4-1769">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1769">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-1770">Keyvault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1770">Keyvault</span></span>

* <span data-ttu-id="6b3f4-1771">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1771">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1772">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1772">Network</span></span>

* <span data-ttu-id="6b3f4-1773">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1773">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6b3f4-1774">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1774">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="6b3f4-1775">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1775">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="6b3f4-1776">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1776">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6b3f4-1777">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1777">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-1778">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1778">Resource</span></span>

* <span data-ttu-id="6b3f4-1779">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1779">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="6b3f4-1780">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1780">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="6b3f4-1781">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1781">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="6b3f4-1782">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1782">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-1783">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1783">SQL</span></span>

* <span data-ttu-id="6b3f4-1784">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1784">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1785">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1785">VM</span></span>

* <span data-ttu-id="6b3f4-1786">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1786">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="6b3f4-1787">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1787">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="6b3f4-1788">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1788">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="6b3f4-1789">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1789">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="6b3f4-1790">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1790">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="6b3f4-1791">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1791">August 31, 2017</span></span>

<span data-ttu-id="6b3f4-1792">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1792">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-1793">Keyvault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1793">Keyvault</span></span>

* <span data-ttu-id="6b3f4-1794">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1794">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="6b3f4-1795">Sf</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1795">Sf</span></span>

* <span data-ttu-id="6b3f4-1796">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1796">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1797">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1797">Storage</span></span>

* <span data-ttu-id="6b3f4-1798">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1798">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="6b3f4-1799">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1799">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="6b3f4-1800">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1800">August 28, 2017</span></span>

<span data-ttu-id="6b3f4-1801">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1801">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="6b3f4-1802">CLI</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1802">CLI</span></span>

* <span data-ttu-id="6b3f4-1803">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1803">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1804">ACS</span></span>

* <span data-ttu-id="6b3f4-1805">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1805">Corrected preview regions</span></span>
* <span data-ttu-id="6b3f4-1806">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1806">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="6b3f4-1807">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1807">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1808">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1808">Appservice</span></span>

* <span data-ttu-id="6b3f4-1809">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1809">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="6b3f4-1810">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1810">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="6b3f4-1811">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1811">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="6b3f4-1812">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1812">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="6b3f4-1813">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1813">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1814">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1814">IoT</span></span>

* <span data-ttu-id="6b3f4-1815">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1815">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1816">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1816">Network</span></span>

* <span data-ttu-id="6b3f4-1817">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1817">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="6b3f4-1818">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1818">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1819">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1819">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="6b3f4-1820">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1820">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="6b3f4-1821">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1821">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1822">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1822">Profile</span></span>

* <span data-ttu-id="6b3f4-1823">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1823">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6b3f4-1824">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1824">Service Fabric</span></span>

* <span data-ttu-id="6b3f4-1825">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1825">Preview release</span></span>
* <span data-ttu-id="6b3f4-1826">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1826">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="6b3f4-1827">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1827">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="6b3f4-1828">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1828">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1829">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1829">Storage</span></span>

* <span data-ttu-id="6b3f4-1830">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1830">Enabled setting blob tier</span></span>
* <span data-ttu-id="6b3f4-1831">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1831">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="6b3f4-1832">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1832">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="6b3f4-1833">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1833">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="6b3f4-1834">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1834">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="6b3f4-1835">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1835">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1836">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1836">VM</span></span>

* <span data-ttu-id="6b3f4-1837">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1837">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="6b3f4-1838">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1838">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="6b3f4-1839">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1839">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="6b3f4-1840">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1840">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="6b3f4-1841">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1841">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="6b3f4-1842">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1842">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="6b3f4-1843">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1843">August 15, 2017</span></span>

<span data-ttu-id="6b3f4-1844">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1844">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1845">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1845">ACS</span></span>

* <span data-ttu-id="6b3f4-1846">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1846">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1847">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1847">Appservice</span></span>

* <span data-ttu-id="6b3f4-1848">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1848">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="6b3f4-1849">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1849">Event Grid</span></span>

* <span data-ttu-id="6b3f4-1850">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1850">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="6b3f4-1851">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1851">August 11, 2017</span></span>

<span data-ttu-id="6b3f4-1852">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1852">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1853">ACS</span></span>

* <span data-ttu-id="6b3f4-1854">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1854">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1855">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1855">Batch</span></span>

* <span data-ttu-id="6b3f4-1856">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1856">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="6b3f4-1857">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1857">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="6b3f4-1858">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1858">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="6b3f4-1859">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="6b3f4-1859">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="6b3f4-1860">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1860">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="6b3f4-1861">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1861">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="6b3f4-1862">Componente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1862">Component</span></span>

* <span data-ttu-id="6b3f4-1863">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1863">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="6b3f4-1864">Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1864">Container</span></span>

* <span data-ttu-id="6b3f4-1865">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1865">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="6b3f4-1866">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1866">Data Lake Store</span></span>

* <span data-ttu-id="6b3f4-1867">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1867">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="6b3f4-1868">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1868">Event Grid</span></span>

* <span data-ttu-id="6b3f4-1869">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1869">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1870">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1870">Network</span></span>

* <span data-ttu-id="6b3f4-1871">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1871">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="6b3f4-1872">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1872">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="6b3f4-1873">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1873">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="6b3f4-1874">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1874">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-1875">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1875">Profile</span></span>

* <span data-ttu-id="6b3f4-1876">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1876">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-1877">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1877">Storage</span></span>

* <span data-ttu-id="6b3f4-1878">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1878">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-1879">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1879">VM</span></span>

* <span data-ttu-id="6b3f4-1880">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1880">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="6b3f4-1881">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1881">Exposed `list-skus` command</span></span>
* <span data-ttu-id="6b3f4-1882">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1882">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="6b3f4-1883">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1883">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="6b3f4-1884">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1884">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="6b3f4-1885">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1885">July 28, 2017</span></span>

<span data-ttu-id="6b3f4-1886">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1886">Version 2.0.12</span></span>

* <span data-ttu-id="6b3f4-1887">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1887">Added container commands</span></span>
* <span data-ttu-id="6b3f4-1888">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1888">Added billing and consumption modules</span></span>

```text
azure-cli (2.0.12)

acr (2.0.9)
acs (2.0.11)
appservice (0.1.11)
batch (3.0.3)
billing (0.1.3)
cdn (0.0.6)
cloud (2.0.7)
cognitiveservices (0.1.6)
command-modules-nspkg (2.0.1)
component (2.0.6)
configure (2.0.10)
consumption (0.1.3)
container (0.1.7)
core (2.0.12)
cosmosdb (0.1.11)
dla (0.0.10)
dls (0.0.11)
feedback (2.0.6)
find (0.2.6)
interactive (0.3.7)
iot (0.1.10)
keyvault (2.0.8)
lab (0.0.9)
monitor (0.0.8)
network (2.0.11)
nspkg (3.0.1)
profile (2.0.9)
rdbms (0.0.5)
redis (0.2.7)
resource (2.0.11)
role (2.0.9)
sf (1.0.5)
sql (2.0.8)
storage (2.0.11)
vm (2.0.11)
```

### <a name="core"></a><span data-ttu-id="6b3f4-1889">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1889">Core</span></span>

* <span data-ttu-id="6b3f4-1890">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1890">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="6b3f4-1891">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1891">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="6b3f4-1892">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1892">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="6b3f4-1893">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1893">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="6b3f4-1894">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1894">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="6b3f4-1895">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1895">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="6b3f4-1896">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1896">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6b3f4-1897">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1897">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="6b3f4-1898">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1898">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="6b3f4-1899">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1899">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="6b3f4-1900">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1900">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="6b3f4-1901">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1901">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="6b3f4-1902">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1902">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="6b3f4-1903">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1903">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="6b3f4-1904">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1904">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="6b3f4-1905">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1905">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="6b3f4-1906">ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1906">ACR</span></span>

* <span data-ttu-id="6b3f4-1907">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1907">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="6b3f4-1908">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1908">Support SKU update for managed registries</span></span>
* <span data-ttu-id="6b3f4-1909">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1909">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="6b3f4-1910">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1910">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="6b3f4-1911">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1911">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="6b3f4-1912">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1912">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-1913">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1913">ACS</span></span>

* <span data-ttu-id="6b3f4-1914">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1914">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-1915">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1915">Appservice</span></span>

* <span data-ttu-id="6b3f4-1916">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1916">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="6b3f4-1917">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1917">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="6b3f4-1918">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1918">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="6b3f4-1919">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1919">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="6b3f4-1920">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1920">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="6b3f4-1921">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1921">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="6b3f4-1922">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1922">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="6b3f4-1923">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1923">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="6b3f4-1924">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1924">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="6b3f4-1925">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1925">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="6b3f4-1926">Lote</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1926">Batch</span></span>

* <span data-ttu-id="6b3f4-1927">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1927">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="6b3f4-1928">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1928">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="6b3f4-1929">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1929">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="6b3f4-1930">CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1930">CDN</span></span>

* <span data-ttu-id="6b3f4-1931">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1931">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="6b3f4-1932">Nuvem</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1932">Cloud</span></span>

* <span data-ttu-id="6b3f4-1933">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1933">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="6b3f4-1934">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1934">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="6b3f4-1935">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1935">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="6b3f4-1936">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1936">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="6b3f4-1937">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1937">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-1938">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1938">CosmosDB</span></span>

* <span data-ttu-id="6b3f4-1939">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1939">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="6b3f4-1940">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1940">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6b3f4-1941">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1941">Data Lake Analytics</span></span>

* <span data-ttu-id="6b3f4-1942">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1942">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="6b3f4-1943">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1943">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="6b3f4-1944">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1944">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6b3f4-1945">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1945">Data Lake Store</span></span>

* <span data-ttu-id="6b3f4-1946">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1946">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="6b3f4-1947">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1947">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="6b3f4-1948">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1948">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="6b3f4-1949">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1949">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="6b3f4-1950">Interativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1950">Interactive</span></span>

* <span data-ttu-id="6b3f4-1951">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1951">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="6b3f4-1952">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1952">Increased test coverage</span></span>
* <span data-ttu-id="6b3f4-1953">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1953">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="6b3f4-1954">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1954">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="6b3f4-1955">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1955">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="6b3f4-1956">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1956">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="6b3f4-1957">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1957">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="6b3f4-1958">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1958">Added `--progress` flag</span></span>
* <span data-ttu-id="6b3f4-1959">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1959">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="6b3f4-1960">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1960">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="6b3f4-1961">IoT</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1961">IoT</span></span>

* <span data-ttu-id="6b3f4-1962">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1962">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="6b3f4-1963">(#3934)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1963">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="6b3f4-1964">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1964">Key vault</span></span>

* <span data-ttu-id="6b3f4-1965">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1965">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="6b3f4-1966">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1966">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="6b3f4-1967">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1967">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6b3f4-1968">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1968">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="6b3f4-1969">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1969">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="6b3f4-1970">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1970">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="6b3f4-1971">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1971">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="6b3f4-1972">(#3307)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1972">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="6b3f4-1973">Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1973">Lab</span></span>

* <span data-ttu-id="6b3f4-1974">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1974">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="6b3f4-1975">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1975">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-1976">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1976">Monitor</span></span>

* <span data-ttu-id="6b3f4-1977">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1977">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="6b3f4-1978">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1978">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="6b3f4-1979">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1979">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="6b3f4-1980">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1980">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="6b3f4-1981">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1981">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="6b3f4-1982">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1982">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="6b3f4-1983">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1983">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="6b3f4-1984">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1984">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="6b3f4-1985">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1985">`location` no longer required</span></span>
  * <span data-ttu-id="6b3f4-1986">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1986">Add name and ID support for target</span></span>
  * <span data-ttu-id="6b3f4-1987">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1987">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="6b3f4-1988">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1988">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="6b3f4-1989">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1989">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="6b3f4-1990">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1990">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="6b3f4-1991">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1991">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="6b3f4-1992">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1992">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-1993">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1993">Network</span></span>

* <span data-ttu-id="6b3f4-1994">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1994">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="6b3f4-1995">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1995">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="6b3f4-1996">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1996">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="6b3f4-1997">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1997">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="6b3f4-1998">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1998">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="6b3f4-1999">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-1999">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="6b3f4-2000">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2000">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="6b3f4-2001">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2001">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="6b3f4-2002">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2002">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="6b3f4-2003">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2003">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="6b3f4-2004">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2004">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="6b3f4-2005">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2005">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="6b3f4-2006">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2006">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="6b3f4-2007">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2007">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="6b3f4-2008">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2008">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="6b3f4-2009">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2009">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="6b3f4-2010">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2010">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="6b3f4-2011">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2011">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="6b3f4-2012">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2012">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="6b3f4-2013">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2013">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="6b3f4-2014">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2014">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="6b3f4-2015">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2015">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="6b3f4-2016">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2016">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="6b3f4-2017">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2017">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="6b3f4-2018">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2018">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="6b3f4-2019">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2019">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="6b3f4-2020">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2020">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-2021">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2021">Profile</span></span>

* <span data-ttu-id="6b3f4-2022">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2022">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="6b3f4-2023">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2023">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="6b3f4-2024">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2024">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="6b3f4-2025">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2025">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="6b3f4-2026">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2026">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="6b3f4-2027">RDBMS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2027">RDBMS</span></span>

* <span data-ttu-id="6b3f4-2028">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2028">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="6b3f4-2029">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2029">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="6b3f4-2030">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2030">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="6b3f4-2031">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2031">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-2032">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2032">Resource</span></span>

* <span data-ttu-id="6b3f4-2033">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2033">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="6b3f4-2034">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2034">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="6b3f4-2035">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2035">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="6b3f4-2036">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2036">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="6b3f4-2037">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2037">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="6b3f4-2038">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2038">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="6b3f4-2039">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2039">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="6b3f4-2040">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2040">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-2041">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2041">Role</span></span>

* <span data-ttu-id="6b3f4-2042">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2042">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="6b3f4-2043">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2043">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="6b3f4-2044">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2044">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="6b3f4-2045">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2045">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="6b3f4-2046">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2046">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="6b3f4-2047">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2047">Service Fabric</span></span>
* <span data-ttu-id="6b3f4-2048">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2048">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="6b3f4-2049">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2049">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="6b3f4-2050">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2050">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2051">SQL</span></span>

* <span data-ttu-id="6b3f4-2052">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2052">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="6b3f4-2053">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2053">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="6b3f4-2054">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2054">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-2055">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2055">Storage</span></span>

* <span data-ttu-id="6b3f4-2056">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2056">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="6b3f4-2057">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2057">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="6b3f4-2058">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2058">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="6b3f4-2059">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2059">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="6b3f4-2060">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2060">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="6b3f4-2061">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2061">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-2062">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2062">VM</span></span>

* <span data-ttu-id="6b3f4-2063">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2063">Support configuring nsg</span></span>
* <span data-ttu-id="6b3f4-2064">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2064">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="6b3f4-2065">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2065">Support managed service identities</span></span>
* <span data-ttu-id="6b3f4-2066">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2066">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="6b3f4-2067">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2067">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="6b3f4-2068">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2068">May 10, 2017</span></span>

<span data-ttu-id="6b3f4-2069">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2069">Version 2.0.6</span></span>

* <span data-ttu-id="6b3f4-2070">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2070">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="6b3f4-2071">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2071">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="6b3f4-2072">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2072">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="6b3f4-2073">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2073">Include Cognitive Services module</span></span>
* <span data-ttu-id="6b3f4-2074">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2074">Include Service Fabric module</span></span>
* <span data-ttu-id="6b3f4-2075">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2075">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="6b3f4-2076">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2076">Add support for CDN commands</span></span>
* <span data-ttu-id="6b3f4-2077">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2077">Remove Container module</span></span>
* <span data-ttu-id="6b3f4-2078">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2078">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="6b3f4-2079">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2079">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```text
azure-cli (2.0.6)

acr (2.0.4)
acs (2.0.6)
appservice (0.1.6)
batch (2.0.4)
cdn (0.0.2)
cloud (2.0.2)
cognitiveservices (0.1.2)
command-modules-nspkg (2.0.0)
component (2.0.4)
configure (2.0.6)
core (2.0.6)
cosmosdb (0.1.6)
dla (0.0.6)
dls (0.0.6)
feedback (2.0.2)
find (0.2.2)
interactive (0.3.1)
iot (0.1.5)
keyvault (2.0.4)
lab (0.0.4)
monitor (0.0.4)
network (2.0.6)
nspkg (3.0.0)
profile (2.0.4)
rdbms (0.0.1)
redis (0.2.3)
resource (2.0.6)
role (2.0.4)
sf (1.0.1)
sql (2.0.3)
storage (2.0.6)
vm (2.0.6)
```

### <a name="core"></a><span data-ttu-id="6b3f4-2080">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2080">Core</span></span>

* <span data-ttu-id="6b3f4-2081">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2081">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="6b3f4-2082">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2082">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="6b3f4-2083">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2083">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="6b3f4-2084">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2084">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="6b3f4-2085">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2085">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="6b3f4-2086">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2086">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="6b3f4-2087">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2087">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="6b3f4-2088">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2088">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="6b3f4-2089">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2089">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="6b3f4-2090">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2090">core: Improved performance</span></span>
* <span data-ttu-id="6b3f4-2091">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2091">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="6b3f4-2092">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2092">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-2093">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2093">ACS</span></span>

* <span data-ttu-id="6b3f4-2094">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2094">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="6b3f4-2095">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2095">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="6b3f4-2096">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2096">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="6b3f4-2097">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2097">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-2098">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2098">AppService</span></span>

* <span data-ttu-id="6b3f4-2099">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2099">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="6b3f4-2100">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2100">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="6b3f4-2101">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2101">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="6b3f4-2102">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2102">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="6b3f4-2103">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2103">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="6b3f4-2104">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2104">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="6b3f4-2105">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2105">support slot swap with preview</span></span>
* <span data-ttu-id="6b3f4-2106">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2106">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="6b3f4-2107">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2107">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="6b3f4-2108">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2108">CosmosDB</span></span>

* <span data-ttu-id="6b3f4-2109">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2109">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="6b3f4-2110">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2110">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="6b3f4-2111">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2111">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="6b3f4-2112">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2112">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="6b3f4-2113">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2113">Data Lake Analytics</span></span>

* <span data-ttu-id="6b3f4-2114">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2114">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="6b3f4-2115">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2115">Add support for new catalog item type: package.</span></span> <span data-ttu-id="6b3f4-2116">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2116">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="6b3f4-2117">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2117">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="6b3f4-2118">Tabela</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2118">Table</span></span>
  * <span data-ttu-id="6b3f4-2119">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2119">Table valued function</span></span>
  * <span data-ttu-id="6b3f4-2120">Visualizar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2120">View</span></span>
  * <span data-ttu-id="6b3f4-2121">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2121">Table Statistics.</span></span> <span data-ttu-id="6b3f4-2122">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2122">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="6b3f4-2123">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2123">Data Lake Store</span></span>

* <span data-ttu-id="6b3f4-2124">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2124">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="6b3f4-2125">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2125">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="6b3f4-2126">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2126">missed help for access show.</span></span> <span data-ttu-id="6b3f4-2127">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2127">adding it.</span></span> <span data-ttu-id="6b3f4-2128">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="6b3f4-2129">Localizar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2129">Find</span></span>

* <span data-ttu-id="6b3f4-2130">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2130">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="6b3f4-2131">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2131">KeyVault</span></span>

* <span data-ttu-id="6b3f4-2132">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2132">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="6b3f4-2133">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2133">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="6b3f4-2134">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2134">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="6b3f4-2135">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2135">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="6b3f4-2136">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2136">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="6b3f4-2137">Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2137">Lab</span></span>

* <span data-ttu-id="6b3f4-2138">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2138">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="6b3f4-2139">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2139">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="6b3f4-2140">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2140">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="6b3f4-2141">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2141">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="6b3f4-2142">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2142">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="6b3f4-2143">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2143">Monitor</span></span>

* <span data-ttu-id="6b3f4-2144">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2144">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="6b3f4-2145">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2145">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="6b3f4-2146">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2146">Network</span></span>

* <span data-ttu-id="6b3f4-2147">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2147">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="6b3f4-2148">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2148">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="6b3f4-2149">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2149">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="6b3f4-2150">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2150">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="6b3f4-2151">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2151">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="6b3f4-2152">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2152">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="6b3f4-2153">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2153">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="6b3f4-2154">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2154">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="6b3f4-2155">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2155">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="6b3f4-2156">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2156">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="6b3f4-2157">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2157">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="6b3f4-2158">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2158">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="6b3f4-2159">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2159">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="6b3f4-2160">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2160">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="6b3f4-2161">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2161">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="6b3f4-2162">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2162">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="6b3f4-2163">Perfil</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2163">Profile</span></span>

* <span data-ttu-id="6b3f4-2164">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2164">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="6b3f4-2165">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2165">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="6b3f4-2166">Redis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2166">Redis</span></span>

* <span data-ttu-id="6b3f4-2167">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2167">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="6b3f4-2168">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2168">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="6b3f4-2169">Recurso</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2169">Resource</span></span>

* <span data-ttu-id="6b3f4-2170">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2170">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="6b3f4-2171">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2171">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="6b3f4-2172">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2172">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="6b3f4-2173">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2173">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="6b3f4-2174">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="6b3f4-2175">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2175">Add docs for az lock update.</span></span> <span data-ttu-id="6b3f4-2176">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="6b3f4-2177">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2177">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="6b3f4-2178">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="6b3f4-2179">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2179">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="6b3f4-2180">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="6b3f4-2181">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2181">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="6b3f4-2182">Função</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2182">Role</span></span>

* <span data-ttu-id="6b3f4-2183">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2183">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="6b3f4-2184">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2184">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="6b3f4-2185">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2185">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="6b3f4-2186">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2186">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="6b3f4-2187">SQL</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2187">SQL</span></span>

* <span data-ttu-id="6b3f4-2188">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2188">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="6b3f4-2189">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2189">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="6b3f4-2190">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2190">Storage</span></span>

* <span data-ttu-id="6b3f4-2191">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2191">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="6b3f4-2192">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2192">Add support for incremental blob copy</span></span>
* <span data-ttu-id="6b3f4-2193">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2193">Add support for large block blob upload</span></span>
* <span data-ttu-id="6b3f4-2194">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2194">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-2195">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2195">VM</span></span>

* <span data-ttu-id="6b3f4-2196">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2196">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="6b3f4-2197">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2197">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="6b3f4-2198">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2198">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="6b3f4-2199">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2199">az vm/vmss disk</span></span>
  3. <span data-ttu-id="6b3f4-2200">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2200">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="6b3f4-2201">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2201">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="6b3f4-2202">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2202">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="6b3f4-2203">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2203">April 3, 2017</span></span>

<span data-ttu-id="6b3f4-2204">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2204">Version 2.0.2</span></span>

<span data-ttu-id="6b3f4-2205">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2205">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

```text
azure-cli (2.0.2)

acr (2.0.0)
acs (2.0.2)
appservice (0.1.2)
batch (2.0.0)
cloud (2.0.0)
component (2.0.0)
configure (2.0.2)
container (0.1.2)
core (2.0.2)
documentdb (0.1.2)
feedback (2.0.0)
find (0.0.1b1)
iot (0.1.2)
keyvault (2.0.0)
lab (0.0.1)
monitor (0.0.1)
network (2.0.2)
nspkg (2.0.0)
profile (2.0.2)
redis (0.1.1b3)
resource (2.0.2)
role (2.0.1)
sql (2.0.0)
storage (2.0.2)
vm (2.0.2)
```

### <a name="core"></a><span data-ttu-id="6b3f4-2206">Núcleo</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2206">Core</span></span>

* <span data-ttu-id="6b3f4-2207">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2207">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="6b3f4-2208">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2208">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="6b3f4-2209">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2209">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="6b3f4-2210">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2210">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6b3f4-2211">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2211">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="6b3f4-2212">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2212">Add prompting for missing template parameters.</span></span> <span data-ttu-id="6b3f4-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="6b3f4-2214">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2214">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="6b3f4-2215">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2215">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="6b3f4-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2216">ACS</span></span>

* <span data-ttu-id="6b3f4-2217">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2217">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="6b3f4-2218">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2218">Add support for ssh key password prompting.</span></span> <span data-ttu-id="6b3f4-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="6b3f4-2220">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2220">Add support for windows clusters.</span></span> <span data-ttu-id="6b3f4-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="6b3f4-2222">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2222">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="6b3f4-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="6b3f4-2224">AppService</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2224">AppService</span></span>

* <span data-ttu-id="6b3f4-2225">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2225">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="6b3f4-2226">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2226">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="6b3f4-2227">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2227">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="6b3f4-2228">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2228">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="6b3f4-2229">DataLake</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2229">DataLake</span></span>

* <span data-ttu-id="6b3f4-2230">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2230">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="6b3f4-2231">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2231">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="6b3f4-2232">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2232">DocuemntDB</span></span>

* <span data-ttu-id="6b3f4-2233">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2233">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="6b3f4-2234">VM</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2234">VM</span></span>

* <span data-ttu-id="6b3f4-2235">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2235">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="6b3f4-2236">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2236">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="6b3f4-2237">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2237">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="6b3f4-2238">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2238">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="6b3f4-2239">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2239">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="6b3f4-2240">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2240">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="6b3f4-2241">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2241">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="6b3f4-2242">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2242">February 27, 2017</span></span>

<span data-ttu-id="6b3f4-2243">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2243">Version 2.0.0</span></span>

<span data-ttu-id="6b3f4-2244">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2244">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="6b3f4-2245">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2245">Container Service (acs)</span></span>
- <span data-ttu-id="6b3f4-2246">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2246">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="6b3f4-2247">Rede</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2247">Networking</span></span>
- <span data-ttu-id="6b3f4-2248">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2248">Storage</span></span>

<span data-ttu-id="6b3f4-2249">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2249">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="6b3f4-2250">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2250">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="6b3f4-2251">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2251">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

```text
azure-cli (2.0.0)

acs (2.0.0)
appservice (0.1.1b5)
batch (0.1.1b4)
cloud (2.0.0)
component (2.0.0)
configure (2.0.0)
container (0.1.1b4)
core (2.0.0)
documentdb (0.1.1b2)
feedback (2.0.0)
iot (0.1.1b3)
keyvault (0.1.1b5)
network (2.0.0)
nspkg (2.0.0)
profile (2.0.0)
redis (0.1.1b3)
resource (2.0.0)
role (2.0.0)
sql (0.1.1b5)
storage (2.0.0)
vm (2.0.0)

Python (Darwin) 2.7.10 (default, Jul 30 2016, 19:40:32)
[GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.34)]
```

> [!Note]
> <span data-ttu-id="6b3f4-2252">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2252">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="6b3f4-2253">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2253">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="6b3f4-2254">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2254">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="6b3f4-2255">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2255">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="6b3f4-2256">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2256">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="6b3f4-2257">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="6b3f4-2257">Provide feedback from the command line with the `az feedback` command</span></span>

