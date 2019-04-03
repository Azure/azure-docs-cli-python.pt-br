---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8307ca9797a9a780d7e08d6d21cb66446c7e289
ms.sourcegitcommit: 6d9e8ee6dd07cfd07239a2948304d7f50ef781cc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2019
ms.locfileid: "58508895"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="5bc9c-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-103">Azure CLI release notes</span></span>
## <a name="march-26-2019"></a><span data-ttu-id="5bc9c-104">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-104">March 26, 2019</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-105">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-105">Core</span></span>
* <span data-ttu-id="5bc9c-106">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-106">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="5bc9c-107">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-107">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="5bc9c-108">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-108">Cloud</span></span>
* <span data-ttu-id="5bc9c-109">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-109">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-110">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-110">ACR</span></span>
* <span data-ttu-id="5bc9c-111">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-111">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="5bc9c-112">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-112">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="5bc9c-113">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="5bc9c-113">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="5bc9c-114">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-114">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-115">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-115">AppService</span></span>
* <span data-ttu-id="5bc9c-116">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-116">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="5bc9c-117">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-117">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="5bc9c-118">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-118">BOT Service</span></span>
* <span data-ttu-id="5bc9c-119">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-119">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="5bc9c-120">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-120">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="5bc9c-121">[ALTERAÇÃO SIGNIFICATIVA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-121">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="5bc9c-122">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-122">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-123">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-123">CDN</span></span>
* <span data-ttu-id="5bc9c-124">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-124">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="5bc9c-126">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="5bc9c-126">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5bc9c-127">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-127">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-128">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="5bc9c-128">Cosmosdb</span></span>
* <span data-ttu-id="5bc9c-129">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="5bc9c-129">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="5bc9c-130">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-130">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-131">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-131">Interactive</span></span>
* <span data-ttu-id="5bc9c-132">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="5bc9c-132">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-133">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-133">Monitor</span></span>
* <span data-ttu-id="5bc9c-134">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-134">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-135">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-135">Network</span></span>
* <span data-ttu-id="5bc9c-136">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-136">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-137">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-137">Profile</span></span>
* <span data-ttu-id="5bc9c-138">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-138">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="5bc9c-139">Postgres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-139">Postgres</span></span> 
* <span data-ttu-id="5bc9c-140">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-140">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="5bc9c-141">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="5bc9c-141">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-142">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-142">Resource</span></span>
* <span data-ttu-id="5bc9c-143">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-143">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="5bc9c-144">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-144">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="5bc9c-145">Grafo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-145">Graph</span></span>
* <span data-ttu-id="5bc9c-146">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-146">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="5bc9c-147">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-147">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="5bc9c-148">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-148">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="5bc9c-149">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-149">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="5bc9c-150">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-150">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-151">storage</span><span class="sxs-lookup"><span data-stu-id="5bc9c-151">storage</span></span>
* <span data-ttu-id="5bc9c-152">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-152">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="5bc9c-153">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-153">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="5bc9c-154">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-154">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="5bc9c-155">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-155">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-156">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-156">VM</span></span>
* <span data-ttu-id="5bc9c-157">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-157">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="5bc9c-158">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-158">March 12, 2019</span></span>

<span data-ttu-id="5bc9c-159">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="5bc9c-159">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-160">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-160">Core</span></span>

* <span data-ttu-id="5bc9c-161">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-161">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-162">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-162">ACR</span></span>

* <span data-ttu-id="5bc9c-163">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-163">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-164">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-164">ACS</span></span>

* <span data-ttu-id="5bc9c-165">Alterado para ignorar o argumento `--listen-address` para `aks browse` se `kubectl` não lhe dar suporte.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-165">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-166">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-166">AppService</span></span>

* <span data-ttu-id="5bc9c-167">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-167">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="5bc9c-168">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-168">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="5bc9c-169">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-169">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="5bc9c-170">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-170">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="5bc9c-171">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-171">Botservice</span></span>

* <span data-ttu-id="5bc9c-172">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-172">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5bc9c-173">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-173">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="5bc9c-174">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-174">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="5bc9c-175">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-175">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-176">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-176">Container</span></span>

* <span data-ttu-id="5bc9c-177">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-177">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="5bc9c-178">EventHub</span><span class="sxs-lookup"><span data-stu-id="5bc9c-178">EventHub</span></span>

* <span data-ttu-id="5bc9c-179">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-179">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="5bc9c-180">Localizar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-180">Find</span></span>

* <span data-ttu-id="5bc9c-181">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="5bc9c-181">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5bc9c-182">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5bc9c-182">HDInsight</span></span>

* <span data-ttu-id="5bc9c-183">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-183">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-184">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-184">Network</span></span>

* <span data-ttu-id="5bc9c-185">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-185">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-186">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5bc9c-186">Rdbms</span></span>

* <span data-ttu-id="5bc9c-187">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-187">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-188">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-188">Role</span></span>

* <span data-ttu-id="5bc9c-189">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-189">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="5bc9c-190">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-190">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bc9c-191">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bc9c-191">Service Fabric</span></span>

* <span data-ttu-id="5bc9c-192">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-192">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="5bc9c-193">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-193">February 26, 2019</span></span>

<span data-ttu-id="5bc9c-194">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="5bc9c-194">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-195">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-195">Core</span></span>

* <span data-ttu-id="5bc9c-196">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="5bc9c-196">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-197">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-197">ACR</span></span>

* <span data-ttu-id="5bc9c-198">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-198">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="5bc9c-199">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-199">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-200">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-200">ACS</span></span>

* <span data-ttu-id="5bc9c-201">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-201">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-202">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-202">AppService</span></span>

* <span data-ttu-id="5bc9c-203">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-203">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-204">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-204">Batch</span></span>
* <span data-ttu-id="5bc9c-205">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-205">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="5bc9c-206">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-206">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="5bc9c-207">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-207">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="5bc9c-208">[ALTERAÇÃO SIGNIFICATIVA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="5bc9c-208">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="5bc9c-209">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="5bc9c-209">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="5bc9c-210">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-210">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-211">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-211">CosmosDB</span></span>

* <span data-ttu-id="5bc9c-212">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-212">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="5bc9c-213">Kusto</span><span class="sxs-lookup"><span data-stu-id="5bc9c-213">Kusto</span></span>

* <span data-ttu-id="5bc9c-214">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="5bc9c-214">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-215">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-215">Network</span></span>

* <span data-ttu-id="5bc9c-216">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-216">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="5bc9c-217">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-217">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="5bc9c-218">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-218">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="5bc9c-219">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-219">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="5bc9c-220">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-220">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="5bc9c-221">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-221">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="5bc9c-222">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-222">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-223">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-223">Resource</span></span>

* <span data-ttu-id="5bc9c-224">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-224">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="5bc9c-225">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-225">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="5bc9c-226">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-226">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="5bc9c-227">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-227">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="5bc9c-228">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-228">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-229">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-229">Role</span></span>

* <span data-ttu-id="5bc9c-230">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-230">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-231">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-231">VM</span></span>

* <span data-ttu-id="5bc9c-232">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-232">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="5bc9c-233">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-233">February 12, 2019</span></span>

<span data-ttu-id="5bc9c-234">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="5bc9c-234">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-235">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-235">Core</span></span>

* <span data-ttu-id="5bc9c-236">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-236">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="5bc9c-237">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-237">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-238">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-238">ACR</span></span>
* <span data-ttu-id="5bc9c-239">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-239">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="5bc9c-240">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-240">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-241">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-241">ACS</span></span>
* <span data-ttu-id="5bc9c-242">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-242">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="5bc9c-243">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-243">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="5bc9c-244">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-244">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="5bc9c-245">AMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-245">AMS</span></span>
* <span data-ttu-id="5bc9c-246">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-246">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="5bc9c-247">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-247">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-248">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-248">Appservice</span></span>
* <span data-ttu-id="5bc9c-249">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-249">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="5bc9c-250">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="5bc9c-250">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="5bc9c-251">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-251">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="5bc9c-252">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="5bc9c-252">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="5bc9c-253">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-253">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="5bc9c-254">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-254">Botservice</span></span>
* <span data-ttu-id="5bc9c-255">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-255">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="5bc9c-256">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-256">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="5bc9c-257">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-257">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="5bc9c-258">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="5bc9c-258">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="5bc9c-259">[PRETERIDO] O argumento `--proj-name` em favor de `--proj-file-path` foi preterido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-259">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="5bc9c-260">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-260">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="5bc9c-261">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-261">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="5bc9c-262">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="5bc9c-262">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="5bc9c-263">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-263">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="5bc9c-264">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="5bc9c-264">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="5bc9c-265">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-265">Key Vault</span></span>
* <span data-ttu-id="5bc9c-266">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-266">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-267">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-267">Monitor</span></span>
* <span data-ttu-id="5bc9c-268">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-268">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-269">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-269">Network</span></span>
* <span data-ttu-id="5bc9c-270">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="5bc9c-270">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="5bc9c-271">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-271">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="5bc9c-272">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-272">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="5bc9c-273">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-273">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5bc9c-274">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="5bc9c-274">Policy Insights</span></span>
* <span data-ttu-id="5bc9c-275">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-275">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-276">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-276">RDBMS</span></span>
* <span data-ttu-id="5bc9c-277">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-277">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="5bc9c-278">Redis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-278">Redis</span></span>
* <span data-ttu-id="5bc9c-279">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-279">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="5bc9c-280">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-280">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="5bc9c-281">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-281">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="5bc9c-282">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-282">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="5bc9c-283">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-283">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="5bc9c-284">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-284">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="5bc9c-285">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-285">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-286">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-286">Role</span></span>
* <span data-ttu-id="5bc9c-287">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-287">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="5bc9c-288">SQL VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-288">SQL VM</span></span>
* <span data-ttu-id="5bc9c-289">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-289">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-290">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-290">VM</span></span>
* <span data-ttu-id="5bc9c-291">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-291">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="5bc9c-292">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-292">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="5bc9c-293">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-293">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="5bc9c-294">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-294">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="5bc9c-295">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-295">January 31, 2019</span></span>

<span data-ttu-id="5bc9c-296">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="5bc9c-296">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-297">Core</span></span>

* <span data-ttu-id="5bc9c-298">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="5bc9c-298">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="5bc9c-299">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-299">January 28, 2019</span></span>

<span data-ttu-id="5bc9c-300">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="5bc9c-300">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-301">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-301">ACR</span></span>
* <span data-ttu-id="5bc9c-302">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="5bc9c-302">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-303">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-303">ACS</span></span>
* <span data-ttu-id="5bc9c-304">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-304">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5bc9c-305">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-305">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="5bc9c-306">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-306">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="5bc9c-307">AMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-307">AMS</span></span>
* <span data-ttu-id="5bc9c-308">[ALTERAÇÃO SIGNIFICATIVA] `ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-308">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="5bc9c-309">[ALTERAÇÃO SIGNIFICATIVA] `ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-309">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-310">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-310">Appservice</span></span>
* <span data-ttu-id="5bc9c-311">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-311">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="5bc9c-312">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="5bc9c-312">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="5bc9c-313">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="5bc9c-313">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-314">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-314">Container</span></span>
* <span data-ttu-id="5bc9c-315">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-315">Added `container start` command</span></span>
* <span data-ttu-id="5bc9c-316">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-316">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5bc9c-317">EventGrid</span><span class="sxs-lookup"><span data-stu-id="5bc9c-317">EventGrid</span></span>
* <span data-ttu-id="5bc9c-318">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-318">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="5bc9c-319">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-319">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="5bc9c-320">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-320">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="5bc9c-321">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-321">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="5bc9c-322">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-322">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5bc9c-323">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5bc9c-323">HDInsight</span></span>
* <span data-ttu-id="5bc9c-324">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-324">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="5bc9c-325">[ALTERAÇÃO SIGNIFICATIVA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="5bc9c-325">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="5bc9c-326">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-326">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="5bc9c-327">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-327">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="5bc9c-328">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-328">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="5bc9c-329">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-329">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-330">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-330">IoT</span></span>
* <span data-ttu-id="5bc9c-331">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="5bc9c-331">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="5bc9c-332">Kusto</span><span class="sxs-lookup"><span data-stu-id="5bc9c-332">Kusto</span></span>
* <span data-ttu-id="5bc9c-333">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-333">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-334">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-334">Monitor</span></span>
* <span data-ttu-id="5bc9c-335">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-335">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-336">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-336">Profile</span></span>
* <span data-ttu-id="5bc9c-337">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-337">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-338">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-338">Network</span></span>
* <span data-ttu-id="5bc9c-339">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-339">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="5bc9c-340">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="5bc9c-340">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-341">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-341">Resource</span></span>
* <span data-ttu-id="5bc9c-342">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-342">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="5bc9c-343">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-343">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="5bc9c-344">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-344">SQL Virtual Machine</span></span>
* <span data-ttu-id="5bc9c-345">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-345">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-346">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-346">Storage</span></span>
* <span data-ttu-id="5bc9c-347">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="5bc9c-347">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="5bc9c-348">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-348">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-349">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-349">VM</span></span>
* <span data-ttu-id="5bc9c-350">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="5bc9c-350">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="5bc9c-351">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-351">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="5bc9c-352">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="5bc9c-352">January 15, 2019</span></span>

<span data-ttu-id="5bc9c-353">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="5bc9c-353">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-354">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-354">ACR</span></span>
* <span data-ttu-id="5bc9c-355">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="5bc9c-355">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="5bc9c-356">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-356">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="5bc9c-357">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-357">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="5bc9c-358">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-358">ACS</span></span>
* <span data-ttu-id="5bc9c-359">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-359">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-360">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-360">Appservice</span></span>
* <span data-ttu-id="5bc9c-361">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-361">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="5bc9c-362">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="5bc9c-362">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="5bc9c-363">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-363">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="5bc9c-364">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-364">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="5bc9c-365">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-365">Botservice</span></span>
* <span data-ttu-id="5bc9c-366">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-366">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="5bc9c-367">Configurar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-367">Configure</span></span>
* <span data-ttu-id="5bc9c-368">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="5bc9c-368">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-369">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-369">CosmosDB</span></span>
* <span data-ttu-id="5bc9c-370">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-370">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5bc9c-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5bc9c-371">HDInsight</span></span>
* <span data-ttu-id="5bc9c-372">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-372">Added commands for managing applications</span></span>
* <span data-ttu-id="5bc9c-373">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="5bc9c-373">Added commands for managing script actions</span></span>
* <span data-ttu-id="5bc9c-374">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-374">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="5bc9c-375">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-375">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="5bc9c-376">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-376">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-377">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-377">Network</span></span>
* <span data-ttu-id="5bc9c-378">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-378">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="5bc9c-379">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="5bc9c-379">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="5bc9c-380">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-380">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="5bc9c-381">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-381">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-382">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-382">Role</span></span>
* <span data-ttu-id="5bc9c-383">[PRETERIDO] O argumento `--password` para `create-for-rbac` foi preterido.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-383">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="5bc9c-384">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-384">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="5bc9c-385">Segurança</span><span class="sxs-lookup"><span data-stu-id="5bc9c-385">Security</span></span>
* <span data-ttu-id="5bc9c-386">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-386">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-387">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-387">Storage</span></span>
* <span data-ttu-id="5bc9c-388">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-388">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="5bc9c-389">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-389">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="5bc9c-390">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-390">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="5bc9c-391">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-391">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="5bc9c-392">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-392">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-393">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-393">VM</span></span>
* <span data-ttu-id="5bc9c-394">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-394">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="5bc9c-395">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-395">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bc9c-396">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-396">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="5bc9c-397">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-397">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="5bc9c-398">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-398">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="5bc9c-399">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-399">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="5bc9c-400">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-400">December 20, 2018</span></span>

<span data-ttu-id="5bc9c-401">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="5bc9c-401">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="5bc9c-402">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-402">Appservice</span></span>
* <span data-ttu-id="5bc9c-403">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-403">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="5bc9c-404">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="5bc9c-404">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="5bc9c-405">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-405">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5bc9c-406">IoT Central</span><span class="sxs-lookup"><span data-stu-id="5bc9c-406">IoTCentral</span></span>
* <span data-ttu-id="5bc9c-407">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-407">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-408">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-408">Role</span></span>
* <span data-ttu-id="5bc9c-409">[ALTERAÇÃO SIGNIFICATIVA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-409">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-410">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-410">SQL</span></span>
* <span data-ttu-id="5bc9c-411">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-411">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-412">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-412">VM</span></span>
* <span data-ttu-id="5bc9c-413">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-413">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="5bc9c-414">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-414">December 18, 2018</span></span>

<span data-ttu-id="5bc9c-415">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="5bc9c-415">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="5bc9c-416">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-416">ACR</span></span>
* <span data-ttu-id="5bc9c-417">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-417">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="5bc9c-418">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-418">Condensed the table layout for task list</span></span>
* <span data-ttu-id="5bc9c-419">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="5bc9c-419">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-420">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-420">ACS</span></span>
* <span data-ttu-id="5bc9c-421">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-421">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="5bc9c-422">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-422">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="5bc9c-423">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-423">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="5bc9c-424">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="5bc9c-424">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="5bc9c-425">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-425">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="5bc9c-426">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="5bc9c-426">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-427">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-427">Appservice</span></span>
* <span data-ttu-id="5bc9c-428">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-428">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="5bc9c-429">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-429">Botservice</span></span>
* <span data-ttu-id="5bc9c-430">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-430">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="5bc9c-431">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="5bc9c-431">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="5bc9c-432">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-432">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="5bc9c-433">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="5bc9c-433">Reduced Kudu network calls</span></span>
* <span data-ttu-id="5bc9c-434">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-434">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-435">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-435">Consumption</span></span>
* <span data-ttu-id="5bc9c-436">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="5bc9c-436">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-437">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-437">CosmosDB</span></span>
* <span data-ttu-id="5bc9c-438">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="5bc9c-438">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="5bc9c-439">Mapas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-439">Maps</span></span>
* <span data-ttu-id="5bc9c-440">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-440">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-441">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-441">Network</span></span>
* <span data-ttu-id="5bc9c-442">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-442">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="5bc9c-443">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="5bc9c-443">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-444">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-444">Resource</span></span>
* <span data-ttu-id="5bc9c-445">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-445">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="5bc9c-446">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-446">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-447">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-447">Storage</span></span>
*  <span data-ttu-id="5bc9c-448">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-448">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-449">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-449">VM</span></span>
* <span data-ttu-id="5bc9c-450">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="5bc9c-450">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="5bc9c-451">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-451">December 4, 2018</span></span>

<span data-ttu-id="5bc9c-452">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="5bc9c-452">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="5bc9c-453">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-453">Core</span></span>
* <span data-ttu-id="5bc9c-454">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="5bc9c-454">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="5bc9c-455">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-455">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-456">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-456">Appservice</span></span>
* <span data-ttu-id="5bc9c-457">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-457">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="5bc9c-458">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="5bc9c-458">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-459">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-459">Network</span></span>
* <span data-ttu-id="5bc9c-460">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="5bc9c-460">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-461">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-461">Role</span></span>
* <span data-ttu-id="5bc9c-462">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="5bc9c-462">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="5bc9c-463">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-463">VM</span></span>
* <span data-ttu-id="5bc9c-464">[PRETERIDO] Parâmetro preterido `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-464">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="5bc9c-465">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="5bc9c-465">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="5bc9c-466">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="5bc9c-466">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="5bc9c-467">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-467">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="5bc9c-468">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-468">November 20, 2018</span></span>

<span data-ttu-id="5bc9c-469">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="5bc9c-469">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="5bc9c-470">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-470">Core</span></span>
* <span data-ttu-id="5bc9c-471">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="5bc9c-471">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-472">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-472">ACR</span></span>
* <span data-ttu-id="5bc9c-473">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="5bc9c-473">Added context token to task step</span></span>
* <span data-ttu-id="5bc9c-474">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="5bc9c-474">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="5bc9c-475">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-475">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-476">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-476">Appservice</span></span>
* <span data-ttu-id="5bc9c-477">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-477">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="5bc9c-478">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-478">Updated the default `node_version`.</span></span> <span data-ttu-id="5bc9c-479">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-479">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="5bc9c-480">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-480">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="5bc9c-481">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="5bc9c-481">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="5bc9c-482">Iot Central</span><span class="sxs-lookup"><span data-stu-id="5bc9c-482">IotCentral</span></span>
* <span data-ttu-id="5bc9c-483">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="5bc9c-483">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-484">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-484">KeyVault</span></span>
* <span data-ttu-id="5bc9c-485">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-485">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-486">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-486">Network</span></span>
* <span data-ttu-id="5bc9c-487">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="5bc9c-487">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="5bc9c-488">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-488">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="5bc9c-489">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-489">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="5bc9c-490">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-490">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-491">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5bc9c-491">Rdbms</span></span>
* <span data-ttu-id="5bc9c-492">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-492">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="5bc9c-493">Rbac</span><span class="sxs-lookup"><span data-stu-id="5bc9c-493">Rbac</span></span>
* <span data-ttu-id="5bc9c-494">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-494">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="5bc9c-495">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-495">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="5bc9c-496">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-496">Storage</span></span>
* <span data-ttu-id="5bc9c-497">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-497">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="5bc9c-498">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-498">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="5bc9c-499">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-499">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="5bc9c-500">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-500">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-501">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-501">VM</span></span>
* <span data-ttu-id="5bc9c-502">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-502">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="5bc9c-503">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-503">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="5bc9c-504">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-504">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="5bc9c-505">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-505">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="5bc9c-506">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-506">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="5bc9c-507">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-507">Added `snapshot wait` command</span></span>
* <span data-ttu-id="5bc9c-508">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-508">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="5bc9c-509">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-509">November 6, 2018</span></span>

<span data-ttu-id="5bc9c-510">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="5bc9c-510">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-511">Core</span></span>
* <span data-ttu-id="5bc9c-512">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-512">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-513">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-513">ACR</span></span>
* <span data-ttu-id="5bc9c-514">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="5bc9c-514">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="5bc9c-515">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-515">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-516">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-516">ACS</span></span>
* <span data-ttu-id="5bc9c-517">[ALTERAÇÃO SIGNIFICATIVA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-517">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="5bc9c-518">Supervisor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-518">Advisor</span></span>
* <span data-ttu-id="5bc9c-519">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="5bc9c-519">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="5bc9c-520">AMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-520">AMS</span></span>
* <span data-ttu-id="5bc9c-521">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-521">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="5bc9c-522">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-522">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="5bc9c-523">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-523">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="5bc9c-524">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-524">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="5bc9c-525">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-525">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="5bc9c-526">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-526">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="5bc9c-527">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-527">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="5bc9c-528">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-528">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="5bc9c-529">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-529">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="5bc9c-530">[ALTERAÇÃO SIGNIFICATIVA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-530">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="5bc9c-531">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-531">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="5bc9c-532">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-532">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="5bc9c-533">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="5bc9c-533">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="5bc9c-534">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-534">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="5bc9c-535">[ALTERAÇÃO SIGNIFICATIVA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-535">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="5bc9c-536">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-536">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="5bc9c-537">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="5bc9c-537">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-538">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-538">AppService</span></span>
* <span data-ttu-id="5bc9c-539">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-539">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="5bc9c-540">Configurar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-540">Configure</span></span>
* <span data-ttu-id="5bc9c-541">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="5bc9c-541">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-542">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-542">Container</span></span>
* <span data-ttu-id="5bc9c-543">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="5bc9c-543">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="5bc9c-544">EventHub</span><span class="sxs-lookup"><span data-stu-id="5bc9c-544">EventHub</span></span>
* <span data-ttu-id="5bc9c-545">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-545">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-546">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-546">Interactive</span></span>
* <span data-ttu-id="5bc9c-547">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-547">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-548">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-548">Monitor</span></span>
* <span data-ttu-id="5bc9c-549">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-549">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-550">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-550">Network</span></span>
* <span data-ttu-id="5bc9c-551">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-551">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="5bc9c-552">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="5bc9c-552">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="5bc9c-553">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-553">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="5bc9c-554">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-554">Profile</span></span>
* <span data-ttu-id="5bc9c-555">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-555">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-556">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-556">RDBMS</span></span>
* <span data-ttu-id="5bc9c-557">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="5bc9c-557">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-558">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-558">Resource</span></span>
* <span data-ttu-id="5bc9c-559">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-559">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-560">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-560">Role</span></span>
* <span data-ttu-id="5bc9c-561">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-561">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="5bc9c-562">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-562">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="5bc9c-563">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="5bc9c-563">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-564">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-564">Storage</span></span>
* <span data-ttu-id="5bc9c-565">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-565">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-566">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-566">VM</span></span>
* <span data-ttu-id="5bc9c-567">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-567">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="5bc9c-568">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-568">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="5bc9c-569">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-569">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="5bc9c-570">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-570">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="5bc9c-571">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-571">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="5bc9c-572">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-572">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="5bc9c-573">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-573">October 23, 2018</span></span>

<span data-ttu-id="5bc9c-574">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="5bc9c-574">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-575">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-575">Core</span></span>
* <span data-ttu-id="5bc9c-576">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-576">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="5bc9c-577">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-577">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-578">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-578">ACR</span></span>
* <span data-ttu-id="5bc9c-579">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="5bc9c-579">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-580">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-580">CDN</span></span>
* <span data-ttu-id="5bc9c-581">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="5bc9c-581">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="5bc9c-582">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-582">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-583">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-583">Container</span></span>
* <span data-ttu-id="5bc9c-584">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="5bc9c-584">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="5bc9c-585">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-585">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="5bc9c-586">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-586">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="5bc9c-587">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-587">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="5bc9c-588">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="5bc9c-588">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="5bc9c-589">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="5bc9c-589">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="5bc9c-590">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-590">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-591">CosmosDB</span></span>
* <span data-ttu-id="5bc9c-592">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-592">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-593">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-593">Interactive</span></span>
* <span data-ttu-id="5bc9c-594">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="5bc9c-594">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="5bc9c-595">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-595">IoT Central</span></span>
* <span data-ttu-id="5bc9c-596">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="5bc9c-596">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="5bc9c-597">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="5bc9c-597">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-598">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-598">Monitor</span></span>
* <span data-ttu-id="5bc9c-599">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-599">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="5bc9c-600">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-600">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="5bc9c-601">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-601">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5bc9c-602">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-602">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="5bc9c-603">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-603">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="5bc9c-604">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-604">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="5bc9c-605">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-605">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="5bc9c-606">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-606">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="5bc9c-607">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-607">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="5bc9c-608">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-608">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-609">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-609">Network</span></span>
* <span data-ttu-id="5bc9c-610">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="5bc9c-610">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="5bc9c-611">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="5bc9c-611">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="5bc9c-612">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="5bc9c-612">ServiceBus</span></span>
* <span data-ttu-id="5bc9c-613">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-613">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-614">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-614">SQL</span></span>
* <span data-ttu-id="5bc9c-615">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-615">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-616">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-616">Storage</span></span>
* <span data-ttu-id="5bc9c-617">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="5bc9c-617">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="5bc9c-618">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="5bc9c-618">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-619">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-619">VM</span></span>
* <span data-ttu-id="5bc9c-620">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-620">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bc9c-621">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-621">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="5bc9c-622">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-622">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="5bc9c-623">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-623">October 16, 2018</span></span>

<span data-ttu-id="5bc9c-624">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="5bc9c-624">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-625">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-625">VM</span></span>
* <span data-ttu-id="5bc9c-626">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="5bc9c-626">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="5bc9c-627">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-627">October 9, 2018</span></span>

<span data-ttu-id="5bc9c-628">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="5bc9c-628">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-629">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-629">Core</span></span>
* <span data-ttu-id="5bc9c-630">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="5bc9c-630">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-631">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-631">ACR</span></span>
* <span data-ttu-id="5bc9c-632">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="5bc9c-632">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-633">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-633">ACS</span></span>
* <span data-ttu-id="5bc9c-634">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="5bc9c-634">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="5bc9c-635">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="5bc9c-635">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="5bc9c-636">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-636">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="5bc9c-637">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-637">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-638">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-638">Container</span></span>
* <span data-ttu-id="5bc9c-639">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-639">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="5bc9c-640">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-640">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="5bc9c-641">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-641">Event Hub</span></span>
* <span data-ttu-id="5bc9c-642">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-642">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="5bc9c-643">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-643">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="5bc9c-644">Extensões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-644">Extensions</span></span>
* <span data-ttu-id="5bc9c-645">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-645">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="5bc9c-646">HDInsight</span><span class="sxs-lookup"><span data-stu-id="5bc9c-646">HDInsight</span></span>
* <span data-ttu-id="5bc9c-647">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-647">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-648">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-648">IoT</span></span>
* <span data-ttu-id="5bc9c-649">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-649">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-650">KeyVault</span></span>
* <span data-ttu-id="5bc9c-651">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-651">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-652">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-652">Network</span></span>
* <span data-ttu-id="5bc9c-653">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-653">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="5bc9c-654">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="5bc9c-654">See #6052</span></span>
* <span data-ttu-id="5bc9c-655">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-655">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="5bc9c-656">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="5bc9c-656">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="5bc9c-657">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-657">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="5bc9c-658">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-658">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="5bc9c-659">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-659">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="5bc9c-660">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-660">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-661">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-661">Role</span></span>
* <span data-ttu-id="5bc9c-662">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-662">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="5bc9c-663">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-663">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="5bc9c-664">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-664">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="5bc9c-665">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="5bc9c-665">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="5bc9c-666">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-666">Service Bus</span></span>
* <span data-ttu-id="5bc9c-667">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-667">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-668">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-668">VM</span></span>
* <span data-ttu-id="5bc9c-669">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-669">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="5bc9c-670">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-670">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="5bc9c-671">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-671">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="5bc9c-672">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-672">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="5bc9c-673">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-673">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="5bc9c-674">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="5bc9c-674">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="5bc9c-675">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-675">September 21, 2018</span></span>

<span data-ttu-id="5bc9c-676">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="5bc9c-676">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-677">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-677">ACR</span></span>
* <span data-ttu-id="5bc9c-678">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-678">Added ACR Task commands</span></span>
* <span data-ttu-id="5bc9c-679">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-679">Added quick run command</span></span>
* <span data-ttu-id="5bc9c-680">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-680">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="5bc9c-681">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-681">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="5bc9c-682">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-682">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="5bc9c-683">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="5bc9c-683">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-684">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-684">ACS</span></span>
* <span data-ttu-id="5bc9c-685">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-685">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="5bc9c-686">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="5bc9c-686">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-687">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-687">AppService</span></span>

* <span data-ttu-id="5bc9c-688">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-688">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="5bc9c-689">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="5bc9c-689">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="5bc9c-690">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="5bc9c-690">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="5bc9c-691">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-691">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-692">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-692">Batch</span></span>
* <span data-ttu-id="5bc9c-693">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="5bc9c-693">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="5bc9c-694">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-694">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="5bc9c-695">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-695">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="5bc9c-696">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-696">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bc9c-697">Lote AI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-697">Batch AI</span></span> 
* <span data-ttu-id="5bc9c-698">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-698">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bc9c-699">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-699">Cognitive Services</span></span>
* <span data-ttu-id="5bc9c-700">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-700">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="5bc9c-701">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-701">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="5bc9c-702">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-702">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="5bc9c-703">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-703">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="5bc9c-704">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-704">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="5bc9c-705">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-705">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-706">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-706">Container</span></span>
* <span data-ttu-id="5bc9c-707">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="5bc9c-707">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="5bc9c-708">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-708">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="5bc9c-709">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-709">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="5bc9c-710">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-710">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="5bc9c-711">DataLake</span><span class="sxs-lookup"><span data-stu-id="5bc9c-711">Datalake</span></span>
* <span data-ttu-id="5bc9c-712">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-712">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="5bc9c-713">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-713">Interactive Shell</span></span>
* <span data-ttu-id="5bc9c-714">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-714">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="5bc9c-715">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-715">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-716">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-716">IoT</span></span>
* <span data-ttu-id="5bc9c-717">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-717">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="5bc9c-718">Key Vault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-718">Key Vault</span></span>
* <span data-ttu-id="5bc9c-719">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="5bc9c-719">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-720">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-720">Network</span></span>
* <span data-ttu-id="5bc9c-721">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="5bc9c-721">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="5bc9c-722">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-722">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="5bc9c-723">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="5bc9c-723">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="5bc9c-724">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="5bc9c-724">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="5bc9c-725">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-725">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="5bc9c-726">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-726">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="5bc9c-727">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-727">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="5bc9c-728">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-728">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="5bc9c-729">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-729">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="5bc9c-730">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-730">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="5bc9c-731">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-731">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="5bc9c-732">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-732">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="5bc9c-733">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-733">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="5bc9c-734">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-734">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="5bc9c-735">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-735">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="5bc9c-736">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="5bc9c-736">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="5bc9c-737">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-737">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="5bc9c-738">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-738">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-739">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-739">RDBMS</span></span>
* <span data-ttu-id="5bc9c-740">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-740">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="5bc9c-741">Reserva</span><span class="sxs-lookup"><span data-stu-id="5bc9c-741">Reservation</span></span>
* <span data-ttu-id="5bc9c-742">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-742">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="5bc9c-743">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="5bc9c-743">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="5bc9c-744">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-744">Manage App</span></span>
* <span data-ttu-id="5bc9c-745">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="5bc9c-745">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="5bc9c-746">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="5bc9c-746">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-747">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-747">Role</span></span>
* <span data-ttu-id="5bc9c-748">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="5bc9c-748">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="5bc9c-749">SignalR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-749">SignalR</span></span>
* <span data-ttu-id="5bc9c-750">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-750">First release</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-751">Storage</span></span>
* <span data-ttu-id="5bc9c-752">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="5bc9c-752">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="5bc9c-753">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="5bc9c-753">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-754">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-754">VM</span></span>
* <span data-ttu-id="5bc9c-755">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-755">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="5bc9c-756">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-756">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="5bc9c-757">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-757">August 28, 2018</span></span>

<span data-ttu-id="5bc9c-758">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="5bc9c-758">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-759">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-759">Core</span></span>

* <span data-ttu-id="5bc9c-760">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="5bc9c-760">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="5bc9c-761">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5bc9c-761">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-762">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-762">ACR</span></span>

* <span data-ttu-id="5bc9c-763">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-763">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="5bc9c-764">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-764">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-765">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-765">ACS</span></span>

* <span data-ttu-id="5bc9c-766">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-766">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="5bc9c-767">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="5bc9c-767">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-768">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-768">AppService</span></span>

* <span data-ttu-id="5bc9c-769">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="5bc9c-769">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="5bc9c-770">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-770">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="5bc9c-771">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-771">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="5bc9c-772">Backup</span><span class="sxs-lookup"><span data-stu-id="5bc9c-772">Backup</span></span>

* <span data-ttu-id="5bc9c-773">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-773">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="5bc9c-774">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-774">Bot Service</span></span>

* <span data-ttu-id="5bc9c-775">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-775">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bc9c-776">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-776">Cognitive Services</span></span>

* <span data-ttu-id="5bc9c-777">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="5bc9c-777">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-778">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-778">IoT</span></span>

* <span data-ttu-id="5bc9c-779">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-779">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-780">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-780">Monitor</span></span>

* <span data-ttu-id="5bc9c-781">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="5bc9c-781">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="5bc9c-782">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-782">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-783">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-783">Network</span></span>

* <span data-ttu-id="5bc9c-784">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-784">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-785">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-785">Resource</span></span>

* <span data-ttu-id="5bc9c-786">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-786">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-787">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-787">Storage</span></span>

* <span data-ttu-id="5bc9c-788">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-788">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-789">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-789">VM</span></span>

* <span data-ttu-id="5bc9c-790">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-790">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="5bc9c-791">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-791">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="5bc9c-792">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-792">Auguest 14, 2018</span></span>

<span data-ttu-id="5bc9c-793">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="5bc9c-793">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-794">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-794">Core</span></span>

* <span data-ttu-id="5bc9c-795">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-795">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="5bc9c-796">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="5bc9c-796">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="5bc9c-797">Telemetria</span><span class="sxs-lookup"><span data-stu-id="5bc9c-797">Telemetry</span></span>

* <span data-ttu-id="5bc9c-798">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="5bc9c-798">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-799">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-799">ACR</span></span>

* <span data-ttu-id="5bc9c-800">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-800">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="5bc9c-801">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-801">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-802">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-802">ACS</span></span>

* <span data-ttu-id="5bc9c-803">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-803">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="5bc9c-804">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-804">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="5bc9c-805">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-805">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="5bc9c-806">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-806">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="5bc9c-807">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="5bc9c-807">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="5bc9c-808">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-808">AppService</span></span>

* <span data-ttu-id="5bc9c-809">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-809">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="5bc9c-810">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="5bc9c-810">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="5bc9c-811">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-811">BatchAI</span></span>

* <span data-ttu-id="5bc9c-812">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-812">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="5bc9c-813">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-813">Container</span></span>

* <span data-ttu-id="5bc9c-814">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-814">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="5bc9c-815">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-815">IoT</span></span>

* <span data-ttu-id="5bc9c-816">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="5bc9c-816">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="5bc9c-817">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-817">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="5bc9c-818">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-818">Iot Central</span></span>

* <span data-ttu-id="5bc9c-819">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="5bc9c-819">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-820">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-820">KeyVault</span></span>


* <span data-ttu-id="5bc9c-821">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-821">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="5bc9c-822">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-822">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="5bc9c-823">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-823">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="5bc9c-824">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="5bc9c-824">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="5bc9c-825">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="5bc9c-825">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="5bc9c-826">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-826">Relay</span></span>

* <span data-ttu-id="5bc9c-827">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-827">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-828">Sql</span><span class="sxs-lookup"><span data-stu-id="5bc9c-828">Sql</span></span>

* <span data-ttu-id="5bc9c-829">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-829">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-830">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-830">Storage</span></span>

* <span data-ttu-id="5bc9c-831">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="5bc9c-831">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="5bc9c-832">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-832">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="5bc9c-833">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-833">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="5bc9c-834">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-834">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="5bc9c-835">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-835">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-836">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-836">VM</span></span>

* <span data-ttu-id="5bc9c-837">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-837">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="5bc9c-838">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-838">July 31, 2018</span></span>

<span data-ttu-id="5bc9c-839">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="5bc9c-839">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-840">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-840">ACR</span></span>

* <span data-ttu-id="5bc9c-841">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-841">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="5bc9c-842">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-842">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-843">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-843">ACS</span></span>

* <span data-ttu-id="5bc9c-844">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-844">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-845">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-845">Batch</span></span>

* <span data-ttu-id="5bc9c-846">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="5bc9c-846">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-847">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-847">Container</span></span>

* <span data-ttu-id="5bc9c-848">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-848">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-849">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-849">Network</span></span>

* <span data-ttu-id="5bc9c-850">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5bc9c-850">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="5bc9c-851">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-851">Resource</span></span>

* <span data-ttu-id="5bc9c-852">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-852">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="5bc9c-853">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-853">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-854">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-854">Role</span></span>

* <span data-ttu-id="5bc9c-855">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="5bc9c-855">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="5bc9c-856">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-856">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="5bc9c-857">Search</span><span class="sxs-lookup"><span data-stu-id="5bc9c-857">Search</span></span>

* <span data-ttu-id="5bc9c-858">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="5bc9c-858">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="5bc9c-859">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-859">Service Bus</span></span>

* <span data-ttu-id="5bc9c-860">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="5bc9c-860">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="5bc9c-861">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-861">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="5bc9c-862">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-862">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="5bc9c-863">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-864">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-864">Storage</span></span>

* <span data-ttu-id="5bc9c-865">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-865">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="5bc9c-866">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-866">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-867">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-867">VM</span></span>

* <span data-ttu-id="5bc9c-868">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-868">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="5bc9c-869">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-869">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="5bc9c-870">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-870">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="5bc9c-871">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-871">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="5bc9c-872">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-872">July 18, 2018</span></span>

<span data-ttu-id="5bc9c-873">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="5bc9c-873">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-874">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-874">Core</span></span>

* <span data-ttu-id="5bc9c-875">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-875">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="5bc9c-876">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="5bc9c-876">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="5bc9c-877">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-877">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-878">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-878">ACR</span></span>

* <span data-ttu-id="5bc9c-879">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="5bc9c-879">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="5bc9c-880">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-880">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="5bc9c-881">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-881">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="5bc9c-882">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-882">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-883">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-883">ACS</span></span>

* <span data-ttu-id="5bc9c-884">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="5bc9c-884">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-885">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-885">AppService</span></span>

* <span data-ttu-id="5bc9c-886">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="5bc9c-886">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-887">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-887">Batch</span></span>

* <span data-ttu-id="5bc9c-888">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5bc9c-888">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="5bc9c-889">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-889">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bc9c-890">Lote AI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-890">Batch AI</span></span>

* <span data-ttu-id="5bc9c-891">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-891">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-892">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-892">Container</span></span>

* <span data-ttu-id="5bc9c-893">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="5bc9c-893">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="5bc9c-894">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="5bc9c-894">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-895">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-895">Network</span></span>

* <span data-ttu-id="5bc9c-896">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-896">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="5bc9c-897">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-897">Added `network nic wait`</span></span>
* <span data-ttu-id="5bc9c-898">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-898">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="5bc9c-899">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-899">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="5bc9c-900">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-900">Resource</span></span>

* <span data-ttu-id="5bc9c-901">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-901">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="5bc9c-902">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-902">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="5bc9c-903">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-903">Added `deployment wait` command</span></span>
* <span data-ttu-id="5bc9c-904">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="5bc9c-904">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-905">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-905">SQL</span></span>

* <span data-ttu-id="5bc9c-906">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-906">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="5bc9c-907">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-907">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="5bc9c-908">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-908">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-909">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-909">Storage</span></span>

* <span data-ttu-id="5bc9c-910">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="5bc9c-910">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-911">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-911">VM</span></span>

* <span data-ttu-id="5bc9c-912">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-912">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="5bc9c-913">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-913">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="5bc9c-914">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-914">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5bc9c-915">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-915">July 3, 2018</span></span>

<span data-ttu-id="5bc9c-916">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="5bc9c-916">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="5bc9c-917">AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-917">AKS</span></span>

* <span data-ttu-id="5bc9c-918">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-918">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="5bc9c-919">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-919">July 3, 2018</span></span>

<span data-ttu-id="5bc9c-920">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="5bc9c-920">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-921">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-921">Core</span></span>

* <span data-ttu-id="5bc9c-922">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-922">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-923">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-923">ACR</span></span>

* <span data-ttu-id="5bc9c-924">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-924">Added polling build status</span></span>
* <span data-ttu-id="5bc9c-925">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-925">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="5bc9c-926">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-926">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-927">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-927">ACS</span></span>

* <span data-ttu-id="5bc9c-928">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-928">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="5bc9c-929">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="5bc9c-929">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="5bc9c-930">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-930">Updated options for `aks browse` command.</span></span> <span data-ttu-id="5bc9c-931">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-931">Added `--listen-port` support</span></span>
* <span data-ttu-id="5bc9c-932">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-932">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="5bc9c-933">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="5bc9c-933">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="5bc9c-934">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-934">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-935">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-935">AppService</span></span>

* <span data-ttu-id="5bc9c-936">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-936">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="5bc9c-937">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="5bc9c-937">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="5bc9c-938">Backup</span><span class="sxs-lookup"><span data-stu-id="5bc9c-938">Backup</span></span>

* <span data-ttu-id="5bc9c-939">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-939">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="5bc9c-940">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-940">BatchAI</span></span>

* <span data-ttu-id="5bc9c-941">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-941">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="5bc9c-942">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-942">Cloud</span></span>

* <span data-ttu-id="5bc9c-943">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-943">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-944">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-944">Container</span></span>

* <span data-ttu-id="5bc9c-945">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="5bc9c-945">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="5bc9c-946">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-946">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="5bc9c-947">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-947">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-948">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-948">Extension</span></span>

* <span data-ttu-id="5bc9c-949">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-949">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-950">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-950">Network</span></span>

* <span data-ttu-id="5bc9c-951">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-951">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-952">Rdbms</span><span class="sxs-lookup"><span data-stu-id="5bc9c-952">Rdbms</span></span>

* <span data-ttu-id="5bc9c-953">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-953">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-954">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-954">Resource</span></span>

* <span data-ttu-id="5bc9c-955">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-955">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-956">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-956">VM</span></span>

* <span data-ttu-id="5bc9c-957">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="5bc9c-957">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="5bc9c-958">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-958">June 25, 2018</span></span>

<span data-ttu-id="5bc9c-959">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="5bc9c-959">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="5bc9c-960">CLI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-960">CLI</span></span>

* <span data-ttu-id="5bc9c-961">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-961">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="5bc9c-962">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-962">June 19, 2018</span></span>

<span data-ttu-id="5bc9c-963">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="5bc9c-963">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-964">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-964">Core</span></span>

* <span data-ttu-id="5bc9c-965">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-965">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-966">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-966">ACR</span></span>

* <span data-ttu-id="5bc9c-967">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="5bc9c-967">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="5bc9c-968">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-968">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-969">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-969">ACS</span></span>

* <span data-ttu-id="5bc9c-970">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-970">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="5bc9c-971">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-971">Added `--update` support</span></span>
* <span data-ttu-id="5bc9c-972">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-972">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="5bc9c-973">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-973">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="5bc9c-974">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-974">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="5bc9c-975">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-975">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="5bc9c-976">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-976">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="5bc9c-977">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-977">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-978">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-978">AppService</span></span>

* <span data-ttu-id="5bc9c-979">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="5bc9c-979">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="5bc9c-980">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-980">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-981">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-981">Batch</span></span>

* <span data-ttu-id="5bc9c-982">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-982">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bc9c-983">Lote AI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-983">Batch AI</span></span>

* <span data-ttu-id="5bc9c-984">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-984">Added support for workspaces.</span></span> <span data-ttu-id="5bc9c-985">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-985">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="5bc9c-986">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-986">Added support for experiments.</span></span> <span data-ttu-id="5bc9c-987">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-987">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="5bc9c-988">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="5bc9c-988">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="5bc9c-989">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-989">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="5bc9c-990">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-990">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="5bc9c-991">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-991">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="5bc9c-992">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="5bc9c-992">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="5bc9c-993">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="5bc9c-993">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="5bc9c-994">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-994">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="5bc9c-995">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-995">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="5bc9c-996">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-996">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="5bc9c-997">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-997">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="5bc9c-998">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-998">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="5bc9c-999">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-999">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="5bc9c-1000">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1000">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="5bc9c-1001">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1001">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="5bc9c-1002">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1002">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="5bc9c-1003">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1003">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5bc9c-1004">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1004">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="5bc9c-1005">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1005">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="5bc9c-1006">Mapas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1006">Maps</span></span>

* <span data-ttu-id="5bc9c-1007">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1007">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1008">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1008">Network</span></span>

* <span data-ttu-id="5bc9c-1009">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1009">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="5bc9c-1010">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1010">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="5bc9c-1011">#6502</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1011">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="5bc9c-1012">Reservas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1012">Reservations</span></span>

* <span data-ttu-id="5bc9c-1013">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1013">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="5bc9c-1014">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1014">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="5bc9c-1015">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1015">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="5bc9c-1016">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1016">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="5bc9c-1017">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1017">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="5bc9c-1018">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1018">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1019">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1019">Role</span></span>

* <span data-ttu-id="5bc9c-1020">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1020">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1021">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1021">SQL</span></span>

* <span data-ttu-id="5bc9c-1022">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1022">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1023">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1023">Storage</span></span>

* <span data-ttu-id="5bc9c-1024">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1024">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1025">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1025">VM</span></span>

* <span data-ttu-id="5bc9c-1026">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1026">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="5bc9c-1027">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1027">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="5bc9c-1028">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1028">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5bc9c-1029">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1029">June 13, 2018</span></span>

<span data-ttu-id="5bc9c-1030">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1030">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1031">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1031">Core</span></span>

* <span data-ttu-id="5bc9c-1032">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1032">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="5bc9c-1033">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1033">June 13, 2018</span></span>

<span data-ttu-id="5bc9c-1034">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1034">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="5bc9c-1035">AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1035">AKS</span></span>

* <span data-ttu-id="5bc9c-1036">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1036">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="5bc9c-1037">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1037">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="5bc9c-1038">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1038">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="5bc9c-1039">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1039">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="5bc9c-1040">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1040">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1041">AppService</span></span>

* <span data-ttu-id="5bc9c-1042">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1042">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5bc9c-1043">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1043">June 5, 2018</span></span>

<span data-ttu-id="5bc9c-1044">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1044">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1045">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1045">Interactive</span></span>

* <span data-ttu-id="5bc9c-1046">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1046">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="5bc9c-1047">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1047">June 5, 2018</span></span>

<span data-ttu-id="5bc9c-1048">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1048">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1049">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1049">Core</span></span>

* <span data-ttu-id="5bc9c-1050">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1050">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="5bc9c-1051">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1051">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1052">ACR</span></span>

* <span data-ttu-id="5bc9c-1053">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1053">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="5bc9c-1054">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1054">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="5bc9c-1055">AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1055">AKS</span></span>

* <span data-ttu-id="5bc9c-1056">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1056">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1057">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1057">Batch</span></span>

* <span data-ttu-id="5bc9c-1058">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1058">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-1059">IOT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1059">IOT</span></span>

* <span data-ttu-id="5bc9c-1060">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1060">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1061">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1061">Network</span></span>

* <span data-ttu-id="5bc9c-1062">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1062">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="5bc9c-1063">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1063">Policy Insights</span></span>

* <span data-ttu-id="5bc9c-1064">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1064">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="5bc9c-1065">ARM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1065">ARM</span></span>

* <span data-ttu-id="5bc9c-1066">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1066">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1067">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1067">SQL</span></span>

* <span data-ttu-id="5bc9c-1068">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1068">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="5bc9c-1069">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1069">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="5bc9c-1070">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1070">Storage</span></span>

* <span data-ttu-id="5bc9c-1071">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1071">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1072">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1072">VM</span></span>

* <span data-ttu-id="5bc9c-1073">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1073">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="5bc9c-1074">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1074">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="5bc9c-1075">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1075">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="5bc9c-1076">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1076">May 22, 2018</span></span>

<span data-ttu-id="5bc9c-1077">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1077">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1078">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1078">Core</span></span>

* <span data-ttu-id="5bc9c-1079">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1079">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1080">ACS</span></span>

* <span data-ttu-id="5bc9c-1081">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1081">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="5bc9c-1082">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1082">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1083">AppService</span></span>

* <span data-ttu-id="5bc9c-1084">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1084">Improved generic update commands</span></span>
* <span data-ttu-id="5bc9c-1085">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1085">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1086">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1086">Container</span></span>

* <span data-ttu-id="5bc9c-1087">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1087">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="5bc9c-1088">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1088">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1089">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1089">Extension</span></span>

* <span data-ttu-id="5bc9c-1090">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1090">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1091">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1091">Interactive</span></span>

* <span data-ttu-id="5bc9c-1092">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1092">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="5bc9c-1093">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1093">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-1094">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1094">KeyVault</span></span>

* <span data-ttu-id="5bc9c-1095">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1095">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1096">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1096">Network</span></span>

* <span data-ttu-id="5bc9c-1097">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1097">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="5bc9c-1098">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1098">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1099">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1099">SQL</span></span>

* <span data-ttu-id="5bc9c-1100">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1100">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="5bc9c-1101">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1101">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="5bc9c-1102">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1102">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="5bc9c-1103">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1103">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="5bc9c-1104">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1104">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="5bc9c-1105">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1105">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="5bc9c-1106">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1106">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="5bc9c-1107">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1107">`edition`.</span></span> <span data-ttu-id="5bc9c-1108">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1108">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="5bc9c-1109">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1109">`elasticPoolName`.</span></span> <span data-ttu-id="5bc9c-1110">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1110">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="5bc9c-1111">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1111">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="5bc9c-1112">`edition`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1112">`edition`.</span></span> <span data-ttu-id="5bc9c-1113">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1113">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="5bc9c-1114">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1114">`dtu`.</span></span> <span data-ttu-id="5bc9c-1115">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1115">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="5bc9c-1116">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1116">`databaseDtuMin`.</span></span> <span data-ttu-id="5bc9c-1117">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1117">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="5bc9c-1118">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1118">`databaseDtuMax`.</span></span> <span data-ttu-id="5bc9c-1119">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1119">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="5bc9c-1120">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1120">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="5bc9c-1121">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1121">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1122">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1122">Storage</span></span>

* <span data-ttu-id="5bc9c-1123">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1123">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="5bc9c-1124">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1124">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1125">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1125">VM</span></span>

* <span data-ttu-id="5bc9c-1126">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1126">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="5bc9c-1127">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1127">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="5bc9c-1128">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1128">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="5bc9c-1129">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1129">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="5bc9c-1130">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1130">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="5bc9c-1131">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1131">May 7, 2018</span></span>

<span data-ttu-id="5bc9c-1132">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1132">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1133">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1133">Core</span></span>

* <span data-ttu-id="5bc9c-1134">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1134">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="5bc9c-1135">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1135">Added limited support for positional arguments</span></span>
* <span data-ttu-id="5bc9c-1136">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1136">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="5bc9c-1137">#5591</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1137">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="5bc9c-1138">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1138">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="5bc9c-1139">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1139">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="5bc9c-1140">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1140">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="5bc9c-1141">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1141">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="5bc9c-1142">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1142">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1143">ACR</span></span>

* <span data-ttu-id="5bc9c-1144">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1144">Added ACR Build commands</span></span>
* <span data-ttu-id="5bc9c-1145">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1145">Improved resource not found error messages</span></span>
* <span data-ttu-id="5bc9c-1146">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1146">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="5bc9c-1147">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1147">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="5bc9c-1148">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1148">Improved repository commands error messages</span></span>
* <span data-ttu-id="5bc9c-1149">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1149">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1150">ACS</span></span>

* <span data-ttu-id="5bc9c-1151">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1151">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="5bc9c-1152">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1152">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="5bc9c-1153">AMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1153">AMS</span></span>

* <span data-ttu-id="5bc9c-1154">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1154">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1155">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1155">Appservice</span></span>

* <span data-ttu-id="5bc9c-1156">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1156">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="5bc9c-1157">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1157">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="5bc9c-1158">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1158">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="5bc9c-1159">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1159">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="5bc9c-1160">Lote AI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1160">Batch AI</span></span>

* <span data-ttu-id="5bc9c-1161">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1161">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bc9c-1162">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1162">Cognitive Services</span></span>

* <span data-ttu-id="5bc9c-1163">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1163">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-1164">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1164">Consumption</span></span>

* <span data-ttu-id="5bc9c-1165">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1165">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1166">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1166">Container</span></span>

* <span data-ttu-id="5bc9c-1167">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1167">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="5bc9c-1168">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1168">Cosmos DB</span></span>

* <span data-ttu-id="5bc9c-1169">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1169">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="5bc9c-1170">DMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1170">DMS</span></span>

* <span data-ttu-id="5bc9c-1171">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1171">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1172">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1172">Extension</span></span>

* <span data-ttu-id="5bc9c-1173">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1173">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1174">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1174">Interactive</span></span>

* <span data-ttu-id="5bc9c-1175">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1175">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="5bc9c-1176">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1176">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="5bc9c-1177">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1177">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="5bc9c-1178">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1178">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="5bc9c-1179">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1179">Lab</span></span>

* <span data-ttu-id="5bc9c-1180">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1180">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1181">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1181">Network</span></span>

* <span data-ttu-id="5bc9c-1182">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1182">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="5bc9c-1183">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1183">Profile</span></span>

* <span data-ttu-id="5bc9c-1184">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1184">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="5bc9c-1185">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1185">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="5bc9c-1186">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1186">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="5bc9c-1187">Redis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1187">Redis</span></span>

* <span data-ttu-id="5bc9c-1188">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1188">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="5bc9c-1189">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1189">Deprecated `redis list-all`.</span></span> <span data-ttu-id="5bc9c-1190">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1190">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="5bc9c-1191">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1191">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="5bc9c-1192">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1192">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1193">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1193">Role</span></span>

* <span data-ttu-id="5bc9c-1194">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1194">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1195">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1195">Storage</span></span>

* <span data-ttu-id="5bc9c-1196">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1196">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="5bc9c-1197">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1197">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="5bc9c-1198">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1198">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="5bc9c-1199">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1199">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="5bc9c-1200">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1200">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1201">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1201">VM</span></span>

* <span data-ttu-id="5bc9c-1202">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1202">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="5bc9c-1203">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1203">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="5bc9c-1204">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1204">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="5bc9c-1205">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1205">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="5bc9c-1206">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1206">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="5bc9c-1207">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1207">Added write accelerator support</span></span>
* <span data-ttu-id="5bc9c-1208">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1208">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="5bc9c-1209">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1209">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="5bc9c-1210">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1210">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="5bc9c-1211">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1211">April 10, 2018</span></span>

<span data-ttu-id="5bc9c-1212">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1212">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1213">ACR</span></span>

* <span data-ttu-id="5bc9c-1214">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1214">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1215">ACS</span></span>

* <span data-ttu-id="5bc9c-1216">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1216">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1217">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1217">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="5bc9c-1219">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1219">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="5bc9c-1220">BatchAI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1220">BatchAI</span></span>

* <span data-ttu-id="5bc9c-1221">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1221">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="5bc9c-1222">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1222">Job level mounting</span></span>
  - <span data-ttu-id="5bc9c-1223">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1223">Environment variables with secret values</span></span>
  - <span data-ttu-id="5bc9c-1224">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1224">Performance counters settings</span></span>
  - <span data-ttu-id="5bc9c-1225">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1225">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="5bc9c-1226">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1226">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="5bc9c-1227">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1227">Usage and limits reporting</span></span>
  - <span data-ttu-id="5bc9c-1228">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1228">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="5bc9c-1229">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1229">Support for custom images</span></span>
  - <span data-ttu-id="5bc9c-1230">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1230">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="5bc9c-1231">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1231">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="5bc9c-1232">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1232">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="5bc9c-1233">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1233">National clouds are supported</span></span>
* <span data-ttu-id="5bc9c-1234">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1234">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="5bc9c-1235">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1235">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="5bc9c-1236">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1236">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="5bc9c-1237">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1237">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="5bc9c-1238">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1238">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="5bc9c-1239">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1239">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="5bc9c-1240">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1240">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="5bc9c-1241">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1241">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="5bc9c-1242">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1242">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="5bc9c-1243">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1243">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="5bc9c-1244">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1244">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="5bc9c-1245">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1245">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="5bc9c-1246">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1246">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="5bc9c-1247">Cobrança</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1247">Billing</span></span>

* <span data-ttu-id="5bc9c-1248">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1248">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-1249">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1249">Consumption</span></span>

* <span data-ttu-id="5bc9c-1250">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1250">Added `marketplace` commands</span></span>
* <span data-ttu-id="5bc9c-1251">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1251">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="5bc9c-1252">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1252">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="5bc9c-1253">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1253">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="5bc9c-1254">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1254">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="5bc9c-1255">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1255">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1256">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1256">Container</span></span>

* <span data-ttu-id="5bc9c-1257">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1257">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="5bc9c-1258">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1258">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1259">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1259">Extension</span></span>

* <span data-ttu-id="5bc9c-1260">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1260">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1261">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1261">Interactive</span></span>

* <span data-ttu-id="5bc9c-1262">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1262">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="5bc9c-1263">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1263">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="5bc9c-1264">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1264">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1265">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1265">Network</span></span>

* <span data-ttu-id="5bc9c-1266">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1266">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="5bc9c-1267">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1267">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="5bc9c-1268">#4910</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1268">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="5bc9c-1269">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1269">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="5bc9c-1270">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1270">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="5bc9c-1271">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1271">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1272">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1272">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1273">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1273">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1274">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1274">Profile</span></span>

* <span data-ttu-id="5bc9c-1275">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1275">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="5bc9c-1276">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1276">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-1277">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1277">RDBMS</span></span>

* <span data-ttu-id="5bc9c-1278">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1278">Added `georestore` command</span></span>
* <span data-ttu-id="5bc9c-1279">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1279">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1280">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1280">Resource</span></span>

* <span data-ttu-id="5bc9c-1281">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1281">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="5bc9c-1282">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1282">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1283">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1283">SQL</span></span>

* <span data-ttu-id="5bc9c-1284">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1284">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1285">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1285">Storage</span></span>

* <span data-ttu-id="5bc9c-1286">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1286">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1287">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1287">VM</span></span>

* <span data-ttu-id="5bc9c-1288">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1288">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="5bc9c-1289">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1289">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="5bc9c-1291">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1291">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="5bc9c-1292">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1292">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="5bc9c-1293">#5718</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1293">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="5bc9c-1294">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1294">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="5bc9c-1295">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1295">March 27, 2018</span></span>

<span data-ttu-id="5bc9c-1296">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1296">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1297">Core</span></span>

* <span data-ttu-id="5bc9c-1298">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1298">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1299">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1299">ACS</span></span>

* <span data-ttu-id="5bc9c-1300">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1300">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1301">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1301">Appservice</span></span>

* <span data-ttu-id="5bc9c-1302">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1302">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="5bc9c-1303">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1303">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5bc9c-1304">Backup</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1304">Backup</span></span>

* <span data-ttu-id="5bc9c-1305">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1305">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="5bc9c-1306">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1306">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="5bc9c-1307">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1307">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="5bc9c-1308">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1308">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1309">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1309">Container</span></span>

* <span data-ttu-id="5bc9c-1310">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1310">Added `container exec` command.</span></span> <span data-ttu-id="5bc9c-1311">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1311">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="5bc9c-1312">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1312">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1313">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1313">Extension</span></span>

* <span data-ttu-id="5bc9c-1314">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1314">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="5bc9c-1315">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1315">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="5bc9c-1316">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1316">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1317">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1317">Interactive</span></span>

* <span data-ttu-id="5bc9c-1318">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1318">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="5bc9c-1319">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1319">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="5bc9c-1320">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1320">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="5bc9c-1321">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1321">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="5bc9c-1322">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1322">Lab</span></span>

* <span data-ttu-id="5bc9c-1323">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1323">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1324">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1324">Monitor</span></span>

* <span data-ttu-id="5bc9c-1325">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1325">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="5bc9c-1326">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1326">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="5bc9c-1327">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1327">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1328">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1328">Network</span></span>

* <span data-ttu-id="5bc9c-1329">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1329">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1330">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1330">Profile</span></span>

* <span data-ttu-id="5bc9c-1331">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1331">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-1332">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1332">RDBMS</span></span>

* <span data-ttu-id="5bc9c-1333">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1333">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1334">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1334">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="5bc9c-1336">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1336">Role</span></span>

* <span data-ttu-id="5bc9c-1337">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1337">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="5bc9c-1338">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1338">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="5bc9c-1339">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1339">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="5bc9c-1340">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1340">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="5bc9c-1341">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1341">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1342">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1342">Storage</span></span>

* <span data-ttu-id="5bc9c-1343">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1343">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="5bc9c-1344">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1344">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1345">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1345">VM</span></span>

* <span data-ttu-id="5bc9c-1346">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1346">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="5bc9c-1347">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1347">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="5bc9c-1348">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1348">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="5bc9c-1349">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1349">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="5bc9c-1350">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1350">March 13, 2018</span></span>

<span data-ttu-id="5bc9c-1351">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1351">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1352">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1352">ACR</span></span>

* <span data-ttu-id="5bc9c-1353">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1353">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="5bc9c-1354">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1354">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="5bc9c-1355">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1355">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1356">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1356">ACS</span></span>

* <span data-ttu-id="5bc9c-1357">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1357">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="5bc9c-1358">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1358">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="5bc9c-1359">Supervisor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1359">Advisor</span></span>

* <span data-ttu-id="5bc9c-1360">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1360">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="5bc9c-1361">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1361">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="5bc9c-1362">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1362">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="5bc9c-1363">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1363">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="5bc9c-1364">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1364">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1365">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1365">Appservice</span></span>

* <span data-ttu-id="5bc9c-1366">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1366">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="5bc9c-1367">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1367">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="5bc9c-1368">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1368">Eventhubs</span></span>

* <span data-ttu-id="5bc9c-1369">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1369">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1370">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1370">Extension</span></span>

* <span data-ttu-id="5bc9c-1371">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1371">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1372">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1372">Interactive</span></span>

* <span data-ttu-id="5bc9c-1373">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1373">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="5bc9c-1374">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1374">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="5bc9c-1375">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1375">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="5bc9c-1376">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1376">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1377">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1377">Monitor</span></span>

* <span data-ttu-id="5bc9c-1378">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1378">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="5bc9c-1379">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1379">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="5bc9c-1380">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1380">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="5bc9c-1381">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1381">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1382">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1382">Network</span></span>

* <span data-ttu-id="5bc9c-1383">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1383">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="5bc9c-1384">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1384">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="5bc9c-1385">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1385">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="5bc9c-1386">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1386">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1387">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1387">Profile</span></span>

* <span data-ttu-id="5bc9c-1388">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1388">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="5bc9c-1389">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1389">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-1390">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1390">RDBMS</span></span>

* <span data-ttu-id="5bc9c-1391">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1391">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="5bc9c-1392">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1392">Service Bus</span></span>

* <span data-ttu-id="5bc9c-1393">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1393">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1394">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1394">Storage</span></span>

* <span data-ttu-id="5bc9c-1395">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1395">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="5bc9c-1396">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1396">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1397">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1397">VM</span></span>

* <span data-ttu-id="5bc9c-1398">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1398">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="5bc9c-1399">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1399">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="5bc9c-1400">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1400">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="5bc9c-1401">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1401">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="5bc9c-1402">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1402">February 27, 2018</span></span>

<span data-ttu-id="5bc9c-1403">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1403">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1404">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1404">Core</span></span>

* <span data-ttu-id="5bc9c-1405">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1405">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="5bc9c-1406">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1406">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="5bc9c-1407">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1407">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1408">ACS</span></span>

* <span data-ttu-id="5bc9c-1409">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1409">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="5bc9c-1410">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1410">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="5bc9c-1411">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1411">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="5bc9c-1412">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1412">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1413">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1413">Appservice</span></span>

* <span data-ttu-id="5bc9c-1414">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1414">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="5bc9c-1415">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1415">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="5bc9c-1416">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1416">Cognitive Services</span></span>

* <span data-ttu-id="5bc9c-1417">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1417">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-1418">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1418">Consumption</span></span>

* <span data-ttu-id="5bc9c-1419">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1419">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="5bc9c-1420">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1420">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1421">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1421">Container</span></span>

* <span data-ttu-id="5bc9c-1422">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1422">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1423">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1423">Network</span></span>

* <span data-ttu-id="5bc9c-1424">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1424">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1425">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1425">Resource</span></span>

* <span data-ttu-id="5bc9c-1426">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1426">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1427">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1427">Role</span></span>

* <span data-ttu-id="5bc9c-1428">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1428">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1429">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1429">SQL</span></span>

* <span data-ttu-id="5bc9c-1430">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1430">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1431">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1431">Storage</span></span>

* <span data-ttu-id="5bc9c-1432">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1432">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1433">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1433">VM</span></span>

* <span data-ttu-id="5bc9c-1434">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1434">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="5bc9c-1435">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1435">February 13, 2018</span></span>

<span data-ttu-id="5bc9c-1436">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1436">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1437">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1437">Core</span></span>

* <span data-ttu-id="5bc9c-1438">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1438">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1439">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1439">ACS</span></span>

* <span data-ttu-id="5bc9c-1440">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1440">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="5bc9c-1441">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1441">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="5bc9c-1442">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1442">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="5bc9c-1443">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1443">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="5bc9c-1444">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1444">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="5bc9c-1445">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1445">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="5bc9c-1446">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1446">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="5bc9c-1447">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1447">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1448">Appservice</span></span>

* <span data-ttu-id="5bc9c-1449">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1449">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="5bc9c-1450">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1450">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1451">CDN</span></span>

* <span data-ttu-id="5bc9c-1452">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1452">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1453">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1453">Container</span></span>

* <span data-ttu-id="5bc9c-1454">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1454">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="5bc9c-1455">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1455">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-1456">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1456">CosmosDB</span></span>

* <span data-ttu-id="5bc9c-1457">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1457">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1458">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1458">Extension</span></span>

* <span data-ttu-id="5bc9c-1459">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1459">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="5bc9c-1460">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1460">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="5bc9c-1461">Comentários</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1461">Feedback</span></span>

* <span data-ttu-id="5bc9c-1462">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1462">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1463">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1463">Interactive</span></span>

* <span data-ttu-id="5bc9c-1464">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1464">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="5bc9c-1465">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1465">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-1466">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1466">IoT</span></span>

* <span data-ttu-id="5bc9c-1467">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1467">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5bc9c-1468">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1468">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="5bc9c-1469">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1469">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1470">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1470">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1471">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1471">Monitor</span></span>

* <span data-ttu-id="5bc9c-1472">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1472">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1473">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1473">Network</span></span>

* <span data-ttu-id="5bc9c-1474">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1474">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="5bc9c-1475">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1475">Profile</span></span>

* <span data-ttu-id="5bc9c-1476">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1476">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1477">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1477">Resource</span></span>

* <span data-ttu-id="5bc9c-1478">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1478">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1479">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1479">Role</span></span>

* <span data-ttu-id="5bc9c-1480">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1480">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1481">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1481">SQL</span></span>

* <span data-ttu-id="5bc9c-1482">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1482">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="5bc9c-1483">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1483">Added `sql db rename`</span></span>
* <span data-ttu-id="5bc9c-1484">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1484">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1485">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1485">Storage</span></span>

* <span data-ttu-id="5bc9c-1486">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1486">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1487">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1487">VM</span></span>

* <span data-ttu-id="5bc9c-1488">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1488">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="5bc9c-1489">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1489">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="5bc9c-1490">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1490">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="5bc9c-1491">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1491">January 31, 2018</span></span>

<span data-ttu-id="5bc9c-1492">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1492">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1493">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1493">Core</span></span>

* <span data-ttu-id="5bc9c-1494">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1494">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="5bc9c-1495">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1495">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="5bc9c-1496">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1496">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="5bc9c-1497">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1497">Use `--verbose` to see</span></span>
* <span data-ttu-id="5bc9c-1498">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1498">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1499">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1499">ACS</span></span>

* <span data-ttu-id="5bc9c-1500">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1500">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="5bc9c-1501">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1501">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1502">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1502">Appservice</span></span>

* <span data-ttu-id="5bc9c-1503">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1503">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="5bc9c-1504">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1504">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-1505">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1505">CDN</span></span>

* <span data-ttu-id="5bc9c-1506">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1506">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-1507">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1507">CosmosDB</span></span>

* <span data-ttu-id="5bc9c-1508">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1508">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1509">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1509">Interactive</span></span>

* <span data-ttu-id="5bc9c-1510">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1510">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1511">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1511">Network</span></span>

* <span data-ttu-id="5bc9c-1512">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1512">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="5bc9c-1513">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1513">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="5bc9c-1514">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1514">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="5bc9c-1515">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1515">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="5bc9c-1516">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1516">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="5bc9c-1517">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1517">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="5bc9c-1518">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1518">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="5bc9c-1519">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1519">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="5bc9c-1520">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1520">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="5bc9c-1521">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1521">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1522">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1522">Profile</span></span>

* <span data-ttu-id="5bc9c-1523">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1523">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1524">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1524">Resource</span></span>

* <span data-ttu-id="5bc9c-1525">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1525">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1526">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1526">Storage</span></span>

* <span data-ttu-id="5bc9c-1527">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1527">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="5bc9c-1528">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1528">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="5bc9c-1529">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1529">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="5bc9c-1530">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1530">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="5bc9c-1531">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1531">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1532">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1532">VM</span></span>

* <span data-ttu-id="5bc9c-1533">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1533">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="5bc9c-1534">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1534">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="5bc9c-1535">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1535">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="5bc9c-1536">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1536">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="5bc9c-1537">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1537">January 17, 2018</span></span>

<span data-ttu-id="5bc9c-1538">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1538">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1539">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1539">ACR</span></span>

* <span data-ttu-id="5bc9c-1540">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1540">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5bc9c-1541">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1541">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1542">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1542">ACS</span></span>

* <span data-ttu-id="5bc9c-1543">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1543">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5bc9c-1544">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1544">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1545">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1545">Appservice</span></span>

* <span data-ttu-id="5bc9c-1546">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1546">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5bc9c-1547">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1547">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5bc9c-1548">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1548">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5bc9c-1549">Backup</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1549">Backup</span></span>

* <span data-ttu-id="5bc9c-1550">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1550">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5bc9c-1551">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1551">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5bc9c-1552">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1552">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5bc9c-1553">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1553">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5bc9c-1554">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1554">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1555">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1555">Batch</span></span>

* <span data-ttu-id="5bc9c-1556">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1556">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5bc9c-1557">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1557">Cloud</span></span>

* <span data-ttu-id="5bc9c-1558">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1558">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-1559">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1559">Consumption</span></span>

* <span data-ttu-id="5bc9c-1560">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1560">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bc9c-1561">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1561">Event Grid</span></span>

* <span data-ttu-id="5bc9c-1562">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1562">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5bc9c-1563">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1563">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5bc9c-1564">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1564">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5bc9c-1565">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5bc9c-1566">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1566">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5bc9c-1567">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1567">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5bc9c-1568">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1568">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5bc9c-1569">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1569">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-1570">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1570">Interactive</span></span>

* <span data-ttu-id="5bc9c-1571">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1571">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5bc9c-1572">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1572">Fixed errors on startup</span></span>
* <span data-ttu-id="5bc9c-1573">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1573">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-1574">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1574">IoT</span></span>

* <span data-ttu-id="5bc9c-1575">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1575">Added support for device provisioning service</span></span>
* <span data-ttu-id="5bc9c-1576">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1576">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5bc9c-1577">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1577">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1578">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1578">Monitor</span></span>

* <span data-ttu-id="5bc9c-1579">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1579">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5bc9c-1580">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1580">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5bc9c-1581">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1581">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1582">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1582">Network</span></span>

* <span data-ttu-id="5bc9c-1583">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1583">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5bc9c-1584">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1584">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1585">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1585">Profile</span></span>

* <span data-ttu-id="5bc9c-1586">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1586">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1587">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1587">Role</span></span>

* <span data-ttu-id="5bc9c-1588">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1588">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bc9c-1589">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1589">Service Fabric</span></span>

* <span data-ttu-id="5bc9c-1590">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1590">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5bc9c-1591">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1591">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1592">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1592">VM</span></span>

* <span data-ttu-id="5bc9c-1593">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1593">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5bc9c-1594">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1594">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5bc9c-1595">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1595">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5bc9c-1596">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1596">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5bc9c-1597">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1597">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5bc9c-1598">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1598">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bc9c-1599">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1599">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bc9c-1600">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1600">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5bc9c-1601">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1601">December 19, 2017</span></span>

<span data-ttu-id="5bc9c-1602">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1602">Version 2.0.23</span></span>

* <span data-ttu-id="5bc9c-1603">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1603">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1604">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1604">Container</span></span>

* <span data-ttu-id="5bc9c-1605">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1605">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1606">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1606">Network</span></span>

* <span data-ttu-id="5bc9c-1607">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1607">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1608">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1608">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1609">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1609">Storage</span></span>

* <span data-ttu-id="5bc9c-1610">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1610">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1611">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1611">VM</span></span>

* <span data-ttu-id="5bc9c-1612">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1612">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5bc9c-1613">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1613">December 5, 2017</span></span>

<span data-ttu-id="5bc9c-1614">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1614">Version 2.0.22</span></span>

* <span data-ttu-id="5bc9c-1615">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1615">Removed `az component` commands.</span></span> <span data-ttu-id="5bc9c-1616">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1616">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1617">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1617">Core</span></span>
* <span data-ttu-id="5bc9c-1618">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1618">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5bc9c-1619">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1619">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1620">ACS</span></span>

* <span data-ttu-id="5bc9c-1621">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1621">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5bc9c-1622">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1622">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5bc9c-1623">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1623">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5bc9c-1624">Supervisor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1624">Advisor</span></span>

* <span data-ttu-id="5bc9c-1625">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1625">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1626">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1626">Appservice</span></span>

* <span data-ttu-id="5bc9c-1627">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1627">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5bc9c-1628">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1628">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5bc9c-1629">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1629">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5bc9c-1630">Consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1630">Consumption</span></span>

* <span data-ttu-id="5bc9c-1631">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1631">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1632">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1632">Container</span></span>

* <span data-ttu-id="5bc9c-1633">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1633">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1634">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1634">Monitor</span></span>

* <span data-ttu-id="5bc9c-1635">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1635">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1636">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1636">Resource</span></span>

* <span data-ttu-id="5bc9c-1637">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1637">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-1638">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1638">Role</span></span>

* <span data-ttu-id="5bc9c-1639">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1639">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5bc9c-1640">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1640">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5bc9c-1641">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1641">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1642">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1642">SQL</span></span>

* <span data-ttu-id="5bc9c-1643">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1643">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5bc9c-1644">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1644">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1645">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1645">VM</span></span>

* <span data-ttu-id="5bc9c-1646">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1646">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5bc9c-1647">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1647">November 14, 2017</span></span>

<span data-ttu-id="5bc9c-1648">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1648">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1649">ACR</span></span>

* <span data-ttu-id="5bc9c-1650">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1650">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5bc9c-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1651">ACS</span></span>

* <span data-ttu-id="5bc9c-1652">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1652">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5bc9c-1653">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1653">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5bc9c-1654">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1654">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5bc9c-1655">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1655">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5bc9c-1656">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1656">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1657">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1657">Appservice</span></span>

* <span data-ttu-id="5bc9c-1658">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1658">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5bc9c-1659">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1659">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5bc9c-1660">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1660">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5bc9c-1661">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1661">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5bc9c-1662">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1662">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5bc9c-1663">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1663">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1664">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1664">Batch</span></span>

* <span data-ttu-id="5bc9c-1665">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1665">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5bc9c-1666">Batchai</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1666">Batchai</span></span>

* <span data-ttu-id="5bc9c-1667">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1667">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5bc9c-1668">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1668">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5bc9c-1669">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1669">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5bc9c-1670">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1670">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5bc9c-1671">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1671">Cloud</span></span>

* <span data-ttu-id="5bc9c-1672">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1672">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1673">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1673">Container</span></span>

* <span data-ttu-id="5bc9c-1674">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1674">Added support to open multiple ports</span></span>
* <span data-ttu-id="5bc9c-1675">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1675">Added container group restart policy</span></span>
* <span data-ttu-id="5bc9c-1676">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1676">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5bc9c-1677">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1677">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bc9c-1678">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1678">Data Lake Analytics</span></span>

* <span data-ttu-id="5bc9c-1679">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1679">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bc9c-1680">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1680">Data Lake Store</span></span>

* <span data-ttu-id="5bc9c-1681">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1681">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1682">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1682">Extension</span></span>

* <span data-ttu-id="5bc9c-1683">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1683">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5bc9c-1684">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1684">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-1685">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1685">IoT</span></span>

* <span data-ttu-id="5bc9c-1686">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1686">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1687">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1687">Monitor</span></span>

* <span data-ttu-id="5bc9c-1688">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1688">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1689">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1689">Network</span></span>

* <span data-ttu-id="5bc9c-1690">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1690">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5bc9c-1691">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1691">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5bc9c-1692">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1692">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5bc9c-1693">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1693">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5bc9c-1694">Reservas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1694">Reservations</span></span>

* <span data-ttu-id="5bc9c-1695">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1695">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1696">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1696">Resource</span></span>

* <span data-ttu-id="5bc9c-1697">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1697">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1698">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1698">SQL</span></span>

* <span data-ttu-id="5bc9c-1699">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1699">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1700">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1700">Storage</span></span>

* <span data-ttu-id="5bc9c-1701">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1701">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5bc9c-1702">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1702">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5bc9c-1703">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1703">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5bc9c-1704">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1704">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5bc9c-1705">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1705">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5bc9c-1706">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1706">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5bc9c-1707">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1707">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1708">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1708">VM</span></span>

* <span data-ttu-id="5bc9c-1709">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1709">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5bc9c-1710">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1710">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5bc9c-1711">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1711">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5bc9c-1712">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1712">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5bc9c-1713">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1713">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5bc9c-1714">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1714">October 24, 2017</span></span>

<span data-ttu-id="5bc9c-1715">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1715">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1716">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1716">Core</span></span>

* <span data-ttu-id="5bc9c-1717">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1717">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1718">ACR</span></span>

* <span data-ttu-id="5bc9c-1719">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1719">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5bc9c-1720">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1720">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5bc9c-1721">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1721">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1722">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1722">ACS</span></span>

* <span data-ttu-id="5bc9c-1723">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1723">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5bc9c-1724">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1724">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1725">Appservice</span></span>

* <span data-ttu-id="5bc9c-1726">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1726">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5bc9c-1727">Componente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1727">Component</span></span>

* <span data-ttu-id="5bc9c-1728">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1728">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-1729">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1729">Monitor</span></span>

* <span data-ttu-id="5bc9c-1730">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1730">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1731">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1731">Resource</span></span>

* <span data-ttu-id="5bc9c-1732">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1732">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5bc9c-1733">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1733">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1734">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1734">VM</span></span>

* <span data-ttu-id="5bc9c-1735">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1735">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5bc9c-1736">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1736">October 9, 2017</span></span>

<span data-ttu-id="5bc9c-1737">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1737">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1738">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1738">Core</span></span>

* <span data-ttu-id="5bc9c-1739">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1739">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1740">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1740">Appservice</span></span>

* <span data-ttu-id="5bc9c-1741">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1741">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1742">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1742">Batch</span></span>

* <span data-ttu-id="5bc9c-1743">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1743">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5bc9c-1744">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1744">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5bc9c-1745">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1745">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5bc9c-1746">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1746">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5bc9c-1747">Batchai</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1747">Batchai</span></span>

* <span data-ttu-id="5bc9c-1748">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1748">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-1749">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1749">Keyvault</span></span>

* <span data-ttu-id="5bc9c-1750">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1750">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5bc9c-1751">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1751">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5bc9c-1752">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1752">Network</span></span>

* <span data-ttu-id="5bc9c-1753">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1753">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5bc9c-1754">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1754">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1755">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1755">Resource</span></span>

* <span data-ttu-id="5bc9c-1756">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1756">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5bc9c-1757">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1757">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5bc9c-1758">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1758">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5bc9c-1759">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1759">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1760">Sql</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1760">Sql</span></span>

* <span data-ttu-id="5bc9c-1761">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1761">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5bc9c-1762">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1762">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5bc9c-1763">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1763">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1764">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1764">Storage</span></span>

* <span data-ttu-id="5bc9c-1765">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1765">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1766">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1766">Vm</span></span>

* <span data-ttu-id="5bc9c-1767">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1767">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5bc9c-1768">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1768">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5bc9c-1769">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1769">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5bc9c-1770">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1770">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5bc9c-1771">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1771">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5bc9c-1772">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1772">September 22, 2017</span></span>

<span data-ttu-id="5bc9c-1773">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1773">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1774">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1774">Resource</span></span>

* <span data-ttu-id="5bc9c-1775">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1775">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5bc9c-1776">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1776">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5bc9c-1777">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1777">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5bc9c-1778">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1778">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1779">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1779">Network</span></span>

* <span data-ttu-id="5bc9c-1780">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1780">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5bc9c-1781">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1781">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5bc9c-1782">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1782">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5bc9c-1783">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1783">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5bc9c-1784">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1784">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1785">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1785">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1786">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1786">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1787">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1787">Storage</span></span>

* <span data-ttu-id="5bc9c-1788">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1788">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5bc9c-1789">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1789">Eventgrid</span></span>

* <span data-ttu-id="5bc9c-1790">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1790">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1791">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1791">SQL</span></span>

* <span data-ttu-id="5bc9c-1792">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1792">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5bc9c-1793">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1793">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5bc9c-1794">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1794">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-1795">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1795">Keyvault</span></span>

* <span data-ttu-id="5bc9c-1796">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1796">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1797">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1797">VM</span></span>

* <span data-ttu-id="5bc9c-1798">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1798">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5bc9c-1799">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1799">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5bc9c-1800">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1800">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5bc9c-1801">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1801">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5bc9c-1802">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1802">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5bc9c-1803">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1803">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1804">ACS</span></span>

* <span data-ttu-id="5bc9c-1805">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1805">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1806">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1806">Appservice</span></span>

* <span data-ttu-id="5bc9c-1807">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1807">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5bc9c-1808">Backup</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1808">Backup</span></span>

* <span data-ttu-id="5bc9c-1809">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1809">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5bc9c-1810">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1810">September 11, 2017</span></span>

<span data-ttu-id="5bc9c-1811">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1811">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5bc9c-1812">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1812">Core</span></span>

* <span data-ttu-id="5bc9c-1813">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1813">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5bc9c-1814">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1814">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1815">Acs</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1815">Acs</span></span>

* <span data-ttu-id="5bc9c-1816">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1816">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5bc9c-1817">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1817">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1818">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1818">Appservice</span></span>

* <span data-ttu-id="5bc9c-1819">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1819">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-1820">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1820">CDN</span></span>

* <span data-ttu-id="5bc9c-1821">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1821">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="5bc9c-1822">Extensão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1822">Extension</span></span>

* <span data-ttu-id="5bc9c-1823">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1823">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-1824">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1824">Keyvault</span></span>

* <span data-ttu-id="5bc9c-1825">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1825">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1826">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1826">Network</span></span>

* <span data-ttu-id="5bc9c-1827">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1827">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5bc9c-1828">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1828">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5bc9c-1829">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1829">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5bc9c-1830">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1830">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5bc9c-1831">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1831">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-1832">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1832">Resource</span></span>

* <span data-ttu-id="5bc9c-1833">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1833">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5bc9c-1834">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1834">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5bc9c-1835">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1835">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5bc9c-1836">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1836">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1837">SQL</span></span>

* <span data-ttu-id="5bc9c-1838">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1838">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1839">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1839">VM</span></span>

* <span data-ttu-id="5bc9c-1840">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1840">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5bc9c-1841">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1841">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5bc9c-1842">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1842">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5bc9c-1843">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1843">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5bc9c-1844">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1844">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5bc9c-1845">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1845">August 31, 2017</span></span>

<span data-ttu-id="5bc9c-1846">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1846">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-1847">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1847">Keyvault</span></span>

* <span data-ttu-id="5bc9c-1848">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1848">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5bc9c-1849">Sf</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1849">Sf</span></span>

* <span data-ttu-id="5bc9c-1850">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1850">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1851">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1851">Storage</span></span>

* <span data-ttu-id="5bc9c-1852">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1852">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5bc9c-1853">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1853">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5bc9c-1854">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1854">August 28, 2017</span></span>

<span data-ttu-id="5bc9c-1855">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1855">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5bc9c-1856">CLI</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1856">CLI</span></span>

* <span data-ttu-id="5bc9c-1857">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1857">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1858">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1858">ACS</span></span>

* <span data-ttu-id="5bc9c-1859">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1859">Corrected preview regions</span></span>
* <span data-ttu-id="5bc9c-1860">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1860">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="5bc9c-1861">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1861">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1862">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1862">Appservice</span></span>

* <span data-ttu-id="5bc9c-1863">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1863">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5bc9c-1864">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1864">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5bc9c-1865">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1865">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5bc9c-1866">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1866">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5bc9c-1867">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1867">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-1868">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1868">IoT</span></span>

* <span data-ttu-id="5bc9c-1869">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1869">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1870">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1870">Network</span></span>

* <span data-ttu-id="5bc9c-1871">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1871">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5bc9c-1872">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1872">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1873">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1873">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5bc9c-1874">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1874">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5bc9c-1875">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1875">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1876">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1876">Profile</span></span>

* <span data-ttu-id="5bc9c-1877">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1877">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bc9c-1878">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1878">Service Fabric</span></span>

* <span data-ttu-id="5bc9c-1879">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1879">Preview release</span></span>
* <span data-ttu-id="5bc9c-1880">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1880">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5bc9c-1881">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1881">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5bc9c-1882">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1882">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1883">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1883">Storage</span></span>

* <span data-ttu-id="5bc9c-1884">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1884">Enabled setting blob tier</span></span>
* <span data-ttu-id="5bc9c-1885">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1885">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5bc9c-1886">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1886">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5bc9c-1887">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1887">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5bc9c-1888">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1888">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5bc9c-1889">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1889">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1890">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1890">VM</span></span>

* <span data-ttu-id="5bc9c-1891">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1891">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5bc9c-1892">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1892">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5bc9c-1893">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1893">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5bc9c-1894">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1894">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5bc9c-1895">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1895">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5bc9c-1896">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1896">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5bc9c-1897">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1897">August 15, 2017</span></span>

<span data-ttu-id="5bc9c-1898">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1898">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1899">ACS</span></span>

* <span data-ttu-id="5bc9c-1900">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1900">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1901">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1901">Appservice</span></span>

* <span data-ttu-id="5bc9c-1902">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1902">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bc9c-1903">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1903">Event Grid</span></span>

* <span data-ttu-id="5bc9c-1904">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1904">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5bc9c-1905">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1905">August 11, 2017</span></span>

<span data-ttu-id="5bc9c-1906">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1906">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1907">ACS</span></span>

* <span data-ttu-id="5bc9c-1908">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1908">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1909">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1909">Batch</span></span>

* <span data-ttu-id="5bc9c-1910">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1910">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5bc9c-1911">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1911">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5bc9c-1912">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1912">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5bc9c-1913">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="5bc9c-1913">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5bc9c-1914">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1914">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5bc9c-1915">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1915">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5bc9c-1916">Componente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1916">Component</span></span>

* <span data-ttu-id="5bc9c-1917">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1917">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5bc9c-1918">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1918">Container</span></span>

* <span data-ttu-id="5bc9c-1919">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1919">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5bc9c-1920">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1920">Data Lake Store</span></span>

* <span data-ttu-id="5bc9c-1921">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1921">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5bc9c-1922">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1922">Event Grid</span></span>

* <span data-ttu-id="5bc9c-1923">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1923">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-1924">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1924">Network</span></span>

* <span data-ttu-id="5bc9c-1925">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1925">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5bc9c-1926">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1926">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5bc9c-1927">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1927">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5bc9c-1928">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1928">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-1929">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1929">Profile</span></span>

* <span data-ttu-id="5bc9c-1930">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1930">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-1931">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1931">Storage</span></span>

* <span data-ttu-id="5bc9c-1932">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1932">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-1933">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1933">VM</span></span>

* <span data-ttu-id="5bc9c-1934">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1934">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5bc9c-1935">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1935">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5bc9c-1936">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1936">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5bc9c-1937">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1937">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5bc9c-1938">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1938">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5bc9c-1939">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1939">July 28, 2017</span></span>

<span data-ttu-id="5bc9c-1940">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1940">Version 2.0.12</span></span>

* <span data-ttu-id="5bc9c-1941">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1941">Added container commands</span></span>
* <span data-ttu-id="5bc9c-1942">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1942">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="5bc9c-1943">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1943">Core</span></span>

* <span data-ttu-id="5bc9c-1944">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1944">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5bc9c-1945">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1945">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5bc9c-1946">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1946">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5bc9c-1947">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1947">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5bc9c-1948">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1948">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5bc9c-1949">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1949">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5bc9c-1950">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1950">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5bc9c-1951">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1951">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5bc9c-1952">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1952">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5bc9c-1953">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1953">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5bc9c-1954">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1954">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5bc9c-1955">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1955">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5bc9c-1956">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1956">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5bc9c-1957">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1957">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5bc9c-1958">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1958">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5bc9c-1959">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1959">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5bc9c-1960">ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1960">ACR</span></span>

* <span data-ttu-id="5bc9c-1961">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1961">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5bc9c-1962">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1962">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5bc9c-1963">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1963">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5bc9c-1964">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1964">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5bc9c-1965">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1965">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5bc9c-1966">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1966">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1967">ACS</span></span>

* <span data-ttu-id="5bc9c-1968">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1968">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-1969">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1969">Appservice</span></span>

* <span data-ttu-id="5bc9c-1970">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1970">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5bc9c-1971">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1971">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5bc9c-1972">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1972">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5bc9c-1973">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1973">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5bc9c-1974">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1974">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5bc9c-1975">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1975">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5bc9c-1976">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1976">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5bc9c-1977">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1977">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5bc9c-1978">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1978">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5bc9c-1979">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1979">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5bc9c-1980">Lote</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1980">Batch</span></span>

* <span data-ttu-id="5bc9c-1981">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1981">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5bc9c-1982">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1982">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5bc9c-1983">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1983">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5bc9c-1984">CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1984">CDN</span></span>

* <span data-ttu-id="5bc9c-1985">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1985">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="5bc9c-1986">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1986">Cloud</span></span>

* <span data-ttu-id="5bc9c-1987">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1987">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5bc9c-1988">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1988">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5bc9c-1989">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1989">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5bc9c-1990">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1990">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5bc9c-1991">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1991">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-1992">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1992">CosmosDB</span></span>

* <span data-ttu-id="5bc9c-1993">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1993">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5bc9c-1994">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1994">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bc9c-1995">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1995">Data Lake Analytics</span></span>

* <span data-ttu-id="5bc9c-1996">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1996">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5bc9c-1997">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1997">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5bc9c-1998">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1998">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bc9c-1999">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-1999">Data Lake Store</span></span>

* <span data-ttu-id="5bc9c-2000">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2000">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5bc9c-2001">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2001">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5bc9c-2002">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2002">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5bc9c-2003">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2003">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5bc9c-2004">Interativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2004">Interactive</span></span>

* <span data-ttu-id="5bc9c-2005">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2005">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5bc9c-2006">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2006">Increased test coverage</span></span>
* <span data-ttu-id="5bc9c-2007">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2007">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5bc9c-2008">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2008">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5bc9c-2009">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2009">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5bc9c-2010">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2010">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5bc9c-2011">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2011">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5bc9c-2012">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2012">Added `--progress` flag</span></span>
* <span data-ttu-id="5bc9c-2013">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2013">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5bc9c-2014">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2014">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5bc9c-2015">IoT</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2015">IoT</span></span>

* <span data-ttu-id="5bc9c-2016">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2016">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5bc9c-2017">(#3934)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2017">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5bc9c-2018">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2018">Key vault</span></span>

* <span data-ttu-id="5bc9c-2019">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2019">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5bc9c-2020">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2020">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5bc9c-2021">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2021">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5bc9c-2022">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2022">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5bc9c-2023">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2023">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5bc9c-2024">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2024">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5bc9c-2025">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2025">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5bc9c-2026">(#3307)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2026">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5bc9c-2027">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2027">Lab</span></span>

* <span data-ttu-id="5bc9c-2028">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2028">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5bc9c-2029">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2029">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-2030">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2030">Monitor</span></span>

* <span data-ttu-id="5bc9c-2031">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2031">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5bc9c-2032">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2032">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5bc9c-2033">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2033">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5bc9c-2034">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2034">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5bc9c-2035">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2035">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5bc9c-2036">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2036">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5bc9c-2037">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2037">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5bc9c-2038">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2038">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5bc9c-2039">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2039">`location` no longer required</span></span>
  * <span data-ttu-id="5bc9c-2040">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2040">Add name and ID support for target</span></span>
  * <span data-ttu-id="5bc9c-2041">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2041">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5bc9c-2042">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2042">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5bc9c-2043">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2043">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5bc9c-2044">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2044">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5bc9c-2045">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2045">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5bc9c-2046">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2046">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-2047">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2047">Network</span></span>

* <span data-ttu-id="5bc9c-2048">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2048">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5bc9c-2049">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2049">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5bc9c-2050">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2050">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5bc9c-2051">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2051">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5bc9c-2052">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2052">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5bc9c-2053">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2053">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5bc9c-2054">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2054">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5bc9c-2055">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2055">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5bc9c-2056">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2056">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5bc9c-2057">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2057">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5bc9c-2058">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2058">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5bc9c-2059">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2059">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5bc9c-2060">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2060">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5bc9c-2061">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2061">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5bc9c-2062">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2062">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5bc9c-2063">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2063">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5bc9c-2064">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2064">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5bc9c-2065">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2065">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5bc9c-2066">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2066">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5bc9c-2067">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2067">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5bc9c-2068">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2068">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5bc9c-2069">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2069">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5bc9c-2070">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2070">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5bc9c-2071">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2071">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5bc9c-2072">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2072">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5bc9c-2073">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2073">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5bc9c-2074">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2074">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-2075">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2075">Profile</span></span>

* <span data-ttu-id="5bc9c-2076">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2076">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5bc9c-2077">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2077">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5bc9c-2078">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2078">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5bc9c-2079">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2079">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5bc9c-2080">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2080">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5bc9c-2081">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2081">RDBMS</span></span>

* <span data-ttu-id="5bc9c-2082">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2082">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5bc9c-2083">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2083">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5bc9c-2084">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2084">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5bc9c-2085">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2085">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-2086">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2086">Resource</span></span>

* <span data-ttu-id="5bc9c-2087">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2087">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5bc9c-2088">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2088">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5bc9c-2089">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2089">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5bc9c-2090">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2090">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5bc9c-2091">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2091">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5bc9c-2092">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2092">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5bc9c-2093">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2093">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5bc9c-2094">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2094">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-2095">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2095">Role</span></span>

* <span data-ttu-id="5bc9c-2096">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2096">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5bc9c-2097">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2097">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5bc9c-2098">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2098">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5bc9c-2099">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2099">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5bc9c-2100">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2100">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5bc9c-2101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2101">Service Fabric</span></span>
* <span data-ttu-id="5bc9c-2102">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2102">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5bc9c-2103">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2103">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5bc9c-2104">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2104">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-2105">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2105">SQL</span></span>

* <span data-ttu-id="5bc9c-2106">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2106">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5bc9c-2107">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2107">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5bc9c-2108">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2108">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-2109">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2109">Storage</span></span>

* <span data-ttu-id="5bc9c-2110">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2110">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5bc9c-2111">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2111">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5bc9c-2112">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2112">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5bc9c-2113">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2113">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5bc9c-2114">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2114">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5bc9c-2115">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2115">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-2116">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2116">VM</span></span>

* <span data-ttu-id="5bc9c-2117">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2117">Support configuring nsg</span></span>
* <span data-ttu-id="5bc9c-2118">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2118">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5bc9c-2119">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2119">Support managed service identities</span></span>
* <span data-ttu-id="5bc9c-2120">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2120">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="5bc9c-2121">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2121">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5bc9c-2122">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2122">May 10, 2017</span></span>

<span data-ttu-id="5bc9c-2123">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2123">Version 2.0.6</span></span>

* <span data-ttu-id="5bc9c-2124">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2124">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5bc9c-2125">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2125">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5bc9c-2126">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2126">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="5bc9c-2127">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2127">Include Cognitive Services module</span></span>
* <span data-ttu-id="5bc9c-2128">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2128">Include Service Fabric module</span></span>
* <span data-ttu-id="5bc9c-2129">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2129">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="5bc9c-2130">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2130">Add support for CDN commands</span></span>
* <span data-ttu-id="5bc9c-2131">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2131">Remove Container module</span></span>
* <span data-ttu-id="5bc9c-2132">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2132">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5bc9c-2133">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2133">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="5bc9c-2134">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2134">Core</span></span>

* <span data-ttu-id="5bc9c-2135">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2135">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5bc9c-2136">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2136">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5bc9c-2137">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2137">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5bc9c-2138">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2138">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5bc9c-2139">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2139">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5bc9c-2140">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2140">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5bc9c-2141">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2141">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5bc9c-2142">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2142">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5bc9c-2143">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2143">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5bc9c-2144">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2144">core: Improved performance</span></span>
* <span data-ttu-id="5bc9c-2145">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2145">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5bc9c-2146">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2146">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2147">ACS</span></span>

* <span data-ttu-id="5bc9c-2148">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2148">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5bc9c-2149">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2149">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5bc9c-2150">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2150">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5bc9c-2151">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2151">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-2152">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2152">AppService</span></span>

* <span data-ttu-id="5bc9c-2153">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2153">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5bc9c-2154">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2154">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5bc9c-2155">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2155">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5bc9c-2156">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2156">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5bc9c-2157">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2157">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5bc9c-2158">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2158">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5bc9c-2159">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2159">support slot swap with preview</span></span>
* <span data-ttu-id="5bc9c-2160">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2160">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5bc9c-2161">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2161">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5bc9c-2162">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2162">CosmosDB</span></span>

* <span data-ttu-id="5bc9c-2163">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2163">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="5bc9c-2164">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2164">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5bc9c-2165">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2165">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5bc9c-2166">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2166">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5bc9c-2167">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2167">Data Lake Analytics</span></span>

* <span data-ttu-id="5bc9c-2168">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2168">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="5bc9c-2169">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2169">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5bc9c-2170">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2170">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5bc9c-2171">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2171">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5bc9c-2172">Tabela</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2172">Table</span></span>
  * <span data-ttu-id="5bc9c-2173">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2173">Table valued function</span></span>
  * <span data-ttu-id="5bc9c-2174">Visualizar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2174">View</span></span>
  * <span data-ttu-id="5bc9c-2175">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2175">Table Statistics.</span></span> <span data-ttu-id="5bc9c-2176">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2176">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5bc9c-2177">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2177">Data Lake Store</span></span>

* <span data-ttu-id="5bc9c-2178">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2178">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="5bc9c-2179">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2179">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5bc9c-2180">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2180">missed help for access show.</span></span> <span data-ttu-id="5bc9c-2181">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2181">adding it.</span></span> <span data-ttu-id="5bc9c-2182">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5bc9c-2183">Localizar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2183">Find</span></span>

* <span data-ttu-id="5bc9c-2184">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2184">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bc9c-2185">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2185">KeyVault</span></span>

* <span data-ttu-id="5bc9c-2186">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2186">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5bc9c-2187">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2187">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="5bc9c-2188">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2188">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5bc9c-2189">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2189">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="5bc9c-2190">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2190">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5bc9c-2191">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2191">Lab</span></span>

* <span data-ttu-id="5bc9c-2192">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2192">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="5bc9c-2193">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2193">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="5bc9c-2194">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2194">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="5bc9c-2195">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2195">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="5bc9c-2196">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2196">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="5bc9c-2197">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2197">Monitor</span></span>

* <span data-ttu-id="5bc9c-2198">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2198">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5bc9c-2199">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2199">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5bc9c-2200">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2200">Network</span></span>

* <span data-ttu-id="5bc9c-2201">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2201">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="5bc9c-2202">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2202">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="5bc9c-2203">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2203">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="5bc9c-2204">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2204">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="5bc9c-2205">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2205">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="5bc9c-2206">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2206">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="5bc9c-2207">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2207">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="5bc9c-2208">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2208">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="5bc9c-2209">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2209">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="5bc9c-2210">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2210">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5bc9c-2211">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2211">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="5bc9c-2212">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2212">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5bc9c-2213">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2213">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="5bc9c-2214">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2214">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="5bc9c-2215">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2215">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="5bc9c-2216">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2216">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="5bc9c-2217">Perfil</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2217">Profile</span></span>

* <span data-ttu-id="5bc9c-2218">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2218">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5bc9c-2219">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2219">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5bc9c-2220">Redis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2220">Redis</span></span>

* <span data-ttu-id="5bc9c-2221">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2221">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5bc9c-2222">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2222">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="5bc9c-2223">Recurso</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2223">Resource</span></span>

* <span data-ttu-id="5bc9c-2224">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2224">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5bc9c-2225">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2225">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5bc9c-2226">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2226">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5bc9c-2227">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2227">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5bc9c-2228">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5bc9c-2229">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2229">Add docs for az lock update.</span></span> <span data-ttu-id="5bc9c-2230">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5bc9c-2231">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2231">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5bc9c-2232">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5bc9c-2233">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2233">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5bc9c-2234">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5bc9c-2235">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2235">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5bc9c-2236">Função</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2236">Role</span></span>

* <span data-ttu-id="5bc9c-2237">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2237">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5bc9c-2238">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2238">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5bc9c-2239">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2239">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5bc9c-2240">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2240">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5bc9c-2241">SQL</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2241">SQL</span></span>

* <span data-ttu-id="5bc9c-2242">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2242">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="5bc9c-2243">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2243">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5bc9c-2244">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2244">Storage</span></span>

* <span data-ttu-id="5bc9c-2245">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2245">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="5bc9c-2246">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2246">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5bc9c-2247">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2247">Add support for large block blob upload</span></span>
* <span data-ttu-id="5bc9c-2248">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2248">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-2249">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2249">VM</span></span>

* <span data-ttu-id="5bc9c-2250">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2250">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5bc9c-2251">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2251">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5bc9c-2252">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2252">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5bc9c-2253">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2253">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5bc9c-2254">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2254">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5bc9c-2255">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2255">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5bc9c-2256">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2256">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5bc9c-2257">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2257">April 3, 2017</span></span>

<span data-ttu-id="5bc9c-2258">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2258">Version 2.0.2</span></span>

<span data-ttu-id="5bc9c-2259">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2259">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="5bc9c-2260">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2260">Core</span></span>

* <span data-ttu-id="5bc9c-2261">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2261">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="5bc9c-2262">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2262">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5bc9c-2263">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2263">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5bc9c-2264">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2264">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5bc9c-2265">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2265">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5bc9c-2266">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2266">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5bc9c-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5bc9c-2268">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2268">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5bc9c-2269">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2269">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5bc9c-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2270">ACS</span></span>

* <span data-ttu-id="5bc9c-2271">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2271">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5bc9c-2272">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2272">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5bc9c-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5bc9c-2274">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2274">Add support for windows clusters.</span></span> <span data-ttu-id="5bc9c-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5bc9c-2276">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2276">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5bc9c-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5bc9c-2278">AppService</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2278">AppService</span></span>

* <span data-ttu-id="5bc9c-2279">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2279">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5bc9c-2280">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2280">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5bc9c-2281">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2281">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5bc9c-2282">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2282">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5bc9c-2283">DataLake</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2283">DataLake</span></span>

* <span data-ttu-id="5bc9c-2284">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2284">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="5bc9c-2285">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2285">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5bc9c-2286">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2286">DocuemntDB</span></span>

* <span data-ttu-id="5bc9c-2287">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2287">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5bc9c-2288">VM</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2288">VM</span></span>

* <span data-ttu-id="5bc9c-2289">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2289">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5bc9c-2290">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2290">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5bc9c-2291">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2291">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5bc9c-2292">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2292">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5bc9c-2293">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2293">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5bc9c-2294">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2294">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="5bc9c-2295">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2295">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5bc9c-2296">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2296">February 27, 2017</span></span>

<span data-ttu-id="5bc9c-2297">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2297">Version 2.0.0</span></span>

<span data-ttu-id="5bc9c-2298">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2298">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="5bc9c-2299">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2299">Container Service (acs)</span></span>
- <span data-ttu-id="5bc9c-2300">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2300">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5bc9c-2301">Rede</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2301">Networking</span></span>
- <span data-ttu-id="5bc9c-2302">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2302">Storage</span></span>

<span data-ttu-id="5bc9c-2303">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2303">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="5bc9c-2304">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2304">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="5bc9c-2305">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2305">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="5bc9c-2306">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2306">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="5bc9c-2307">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2307">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="5bc9c-2308">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2308">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5bc9c-2309">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2309">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5bc9c-2310">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2310">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="5bc9c-2311">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="5bc9c-2311">Provide feedback from the command line with the `az feedback` command</span></span>

