---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/09/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: df665565130322504c4794462098980b1064a6c7
ms.sourcegitcommit: c6dff58438d256647d4aa29a53eef4bf93a0cd24
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "59479990"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="a948f-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-103">Azure CLI release notes</span></span>
## <a name="april-9-2019"></a><span data-ttu-id="a948f-104">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-104">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="a948f-105">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-105">Core</span></span>
* <span data-ttu-id="a948f-106">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="a948f-106">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-107">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-107">ACR</span></span>
* <span data-ttu-id="a948f-108">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="a948f-108">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="a948f-109">AMS</span><span class="sxs-lookup"><span data-stu-id="a948f-109">AMS</span></span>
* [<span data-ttu-id="a948f-110">PRETERIDO</span><span class="sxs-lookup"><span data-stu-id="a948f-110">DEPRECATED</span></span>]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [<span data-ttu-id="a948f-111">ALTERAÇÃO DA FALHA</span><span class="sxs-lookup"><span data-stu-id="a948f-111">BREAKING CHANGE</span></span>]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="a948f-112">Adição de suporte para novos parâmetros de criptografia em</span><span class="sxs-lookup"><span data-stu-id="a948f-112">Added new encryption parameters support in</span></span> `ams streaming-policy create`
* <span data-ttu-id="a948f-113">Adição de novo parâmetro `--filters` a</span><span class="sxs-lookup"><span data-stu-id="a948f-113">Added new paramter `--filters` to</span></span> `ams streaming-locator create`

### <a name="appservice"></a><span data-ttu-id="a948f-114">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-114">AppService</span></span>
* <span data-ttu-id="a948f-115">Adicionado suporte `--logs` a</span><span class="sxs-lookup"><span data-stu-id="a948f-115">Added `--logs` support to</span></span> `webapp up`
* <span data-ttu-id="a948f-116">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="a948f-116">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="a948f-117">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="a948f-117">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="a948f-118">[ALTERAÇÃO DA FALHA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a948f-118">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="a948f-119">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="a948f-119">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="a948f-120">Adição da capacidade de trocar um plano abaixo de um aplicativo de funções usando</span><span class="sxs-lookup"><span data-stu-id="a948f-120">Added ability to switch a plan underneath a function app using</span></span> `functionapp update --plan`
* <span data-ttu-id="a948f-121">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="a948f-121">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="a948f-122">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-122">CDN</span></span>
* <span data-ttu-id="a948f-123">Adição de suporte para `Microsoft_Standard` e</span><span class="sxs-lookup"><span data-stu-id="a948f-123">Added support for `Microsoft_Standard` and</span></span> `Standard_ChinaCdn`

### <a name="feedback"></a><span data-ttu-id="a948f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="a948f-124">Feedback</span></span>
* <span data-ttu-id="a948f-125">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="a948f-125">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="a948f-126">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="a948f-126">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="a948f-127">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="a948f-127">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-128">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-128">Monitor</span></span>
* <span data-ttu-id="a948f-129">Correção de um problema em que “count” não era um valor permitido com</span><span class="sxs-lookup"><span data-stu-id="a948f-129">Fixed issue where "count" was not a permitted value with</span></span> `metrics alert [create|update]` 

### <a name="network"></a><span data-ttu-id="a948f-130">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-130">Network</span></span>
* <span data-ttu-id="a948f-131">Correção do formato de tabela que não estava sendo exibido com</span><span class="sxs-lookup"><span data-stu-id="a948f-131">Fixed table format not displaying with</span></span> `vnet-gateway list-bgp-peer-status`
* <span data-ttu-id="a948f-132">Adição dos comandos `list-request-headers` e `list-response-headers` ao</span><span class="sxs-lookup"><span data-stu-id="a948f-132">Added `list-request-headers` and `list-response-headers` commands to</span></span> `application-gateway rewrite-rule`
* <span data-ttu-id="a948f-133">Adição do comando `list-server-variables` ao</span><span class="sxs-lookup"><span data-stu-id="a948f-133">Added `list-server-variables` command to</span></span> `application-gateway rewrite-rule condition`
* <span data-ttu-id="a948f-134">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido</span><span class="sxs-lookup"><span data-stu-id="a948f-134">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception</span></span> `express-route port update`

### <a name="privatedns"></a><span data-ttu-id="a948f-135">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="a948f-135">PrivateDNS</span></span>
* <span data-ttu-id="a948f-136">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="a948f-136">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-137">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-137">Resource</span></span>
* <span data-ttu-id="a948f-138">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="a948f-138">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="a948f-139">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-139">Role</span></span>
* <span data-ttu-id="a948f-140">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="a948f-140">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="a948f-141">[ALTERAÇÃO DA FALHA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="a948f-141">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-142">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-142">SQL</span></span>
* <span data-ttu-id="a948f-143">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="a948f-143">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-144">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-144">Storage</span></span>
* <span data-ttu-id="a948f-145">[ALTERAÇÃO DA FALHA] Remoção do resultado de</span><span class="sxs-lookup"><span data-stu-id="a948f-145">[BREAKING CHANGE] Removed result of</span></span> `storage blob delete`
* <span data-ttu-id="a948f-146">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="a948f-146">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="a948f-147">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="a948f-147">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="a948f-148">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="a948f-148">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="a948f-149">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-149">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="a948f-150">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-150">Core</span></span>
* <span data-ttu-id="a948f-151">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="a948f-151">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="a948f-152">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="a948f-152">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="a948f-153">Nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-153">Cloud</span></span>
* <span data-ttu-id="a948f-154">Correção do erro de “assinatura não encontrada” em</span><span class="sxs-lookup"><span data-stu-id="a948f-154">Fixed a 'subscription not found' error in</span></span> `cloud set`

### <a name="acr"></a><span data-ttu-id="a948f-155">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-155">ACR</span></span>
* <span data-ttu-id="a948f-156">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="a948f-156">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="a948f-157">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a948f-157">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="a948f-158">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="a948f-158">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="a948f-159">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="a948f-159">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-160">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-160">AppService</span></span>
* <span data-ttu-id="a948f-161">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="a948f-161">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="a948f-162">Correção do bug em que os slots não funcionavam para</span><span class="sxs-lookup"><span data-stu-id="a948f-162">Fixed bug where slots didn't work for</span></span> `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a><span data-ttu-id="a948f-163">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="a948f-163">BOT Service</span></span>
* <span data-ttu-id="a948f-164">Adição de `bot prepare-deploy` para se preparar para a implantação de bots via</span><span class="sxs-lookup"><span data-stu-id="a948f-164">Added `bot prepare-deploy` to prepare for deploying bots via</span></span> `webapp`
* <span data-ttu-id="a948f-165">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="a948f-165">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="a948f-166">[ALTERAÇÃO DA FALHA] `--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="a948f-166">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="a948f-167">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="a948f-167">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="a948f-168">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-168">CDN</span></span>
* <span data-ttu-id="a948f-169">Adição do suporte para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-169">Added support for `--no-wait` to</span></span> `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* [ALTERAÇÃO DA FALHA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="a948f-171">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="a948f-171">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a948f-172">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-172">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-173">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="a948f-173">Cosmosdb</span></span>
* <span data-ttu-id="a948f-174">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="a948f-174">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="a948f-175">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a948f-175">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-176">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-176">Interactive</span></span>
* <span data-ttu-id="a948f-177">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="a948f-177">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-178">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-178">Monitor</span></span>
* <span data-ttu-id="a948f-179">Alteração para permitir o valor de dimensão `*` para</span><span class="sxs-lookup"><span data-stu-id="a948f-179">Changed to allow dimension value `*` for</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="a948f-180">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-180">Network</span></span>
* <span data-ttu-id="a948f-181">Adição do grupo de comandos `rewrite-rule` a</span><span class="sxs-lookup"><span data-stu-id="a948f-181">Added `rewrite-rule` command group to</span></span> `application-gateway`

### <a name="profile"></a><span data-ttu-id="a948f-182">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-182">Profile</span></span>
* <span data-ttu-id="a948f-183">Adição de suporte de conta no nível do locatário para a identidade de serviço gerenciado a</span><span class="sxs-lookup"><span data-stu-id="a948f-183">Added tenant level account support for managed service identity to</span></span> `login`

### <a name="postgres"></a><span data-ttu-id="a948f-184">Postgres</span><span class="sxs-lookup"><span data-stu-id="a948f-184">Postgres</span></span> 
* <span data-ttu-id="a948f-185">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="a948f-185">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="a948f-186">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="a948f-186">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-187">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-187">Resource</span></span>
* <span data-ttu-id="a948f-188">Melhoria da saída da tabela para</span><span class="sxs-lookup"><span data-stu-id="a948f-188">Improved table output for</span></span> `deployment [create|list|show]`
* <span data-ttu-id="a948f-189">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="a948f-189">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="a948f-190">Grafo</span><span class="sxs-lookup"><span data-stu-id="a948f-190">Graph</span></span>
* <span data-ttu-id="a948f-191">Adição do suporte para `--end-date` a</span><span class="sxs-lookup"><span data-stu-id="a948f-191">Added support for `--end-date` to</span></span> `ad [app|sp] credential reset`
* <span data-ttu-id="a948f-192">Adição de suporte para adicionar permissões com</span><span class="sxs-lookup"><span data-stu-id="a948f-192">Added support to add permissions with</span></span> `ad app permission add`
* <span data-ttu-id="a948f-193">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="a948f-193">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="a948f-194">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-194">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="a948f-195">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="a948f-195">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-196">storage</span><span class="sxs-lookup"><span data-stu-id="a948f-196">storage</span></span>
* <span data-ttu-id="a948f-197">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="a948f-197">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="a948f-198">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="a948f-198">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="a948f-199">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="a948f-199">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="a948f-200">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="a948f-200">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-201">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-201">VM</span></span>
* <span data-ttu-id="a948f-202">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="a948f-202">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="a948f-203">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-203">March 12, 2019</span></span>

<span data-ttu-id="a948f-204">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="a948f-204">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="a948f-205">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-205">Core</span></span>

* <span data-ttu-id="a948f-206">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="a948f-206">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-207">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-207">ACR</span></span>

* <span data-ttu-id="a948f-208">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="a948f-208">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-209">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-209">ACS</span></span>

* <span data-ttu-id="a948f-210">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="a948f-210">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="a948f-211">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-211">AppService</span></span>

* <span data-ttu-id="a948f-212">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="a948f-212">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="a948f-213">Removida a instrução de impressão errônea de</span><span class="sxs-lookup"><span data-stu-id="a948f-213">Removed erroneous print statement for</span></span> `webapp auth update`
* <span data-ttu-id="a948f-214">Corrigido `functionapp` para definir a imagem correta do tempo de execução nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="a948f-214">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="a948f-215">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="a948f-215">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="a948f-216">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="a948f-216">Botservice</span></span>

* <span data-ttu-id="a948f-217">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="a948f-217">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a948f-218">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="a948f-218">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="a948f-219">Removidas as aspas simples da saída de comando `bot publish` no final de</span><span class="sxs-lookup"><span data-stu-id="a948f-219">Removed single quotes from `bot publish` command output at end of</span></span> `bot create`
* <span data-ttu-id="a948f-220">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="a948f-220">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="a948f-221">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-221">Container</span></span>

* <span data-ttu-id="a948f-222">Adicionado argumento `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-222">Added `--no-wait` argument to</span></span> `container [start|restart]`

### <a name="eventhub"></a><span data-ttu-id="a948f-223">EventHub</span><span class="sxs-lookup"><span data-stu-id="a948f-223">EventHub</span></span>

* <span data-ttu-id="a948f-224">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="a948f-224">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="a948f-225">Localizar</span><span class="sxs-lookup"><span data-stu-id="a948f-225">Find</span></span>

* <span data-ttu-id="a948f-226">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="a948f-226">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a948f-227">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a948f-227">HDInsight</span></span>

* <span data-ttu-id="a948f-228">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="a948f-228">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="a948f-229">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-229">Network</span></span>

* <span data-ttu-id="a948f-230">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="a948f-230">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a948f-231">Rdbms</span></span>

* <span data-ttu-id="a948f-232">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="a948f-232">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="a948f-233">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-233">Role</span></span>

* <span data-ttu-id="a948f-234">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="a948f-234">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="a948f-235">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="a948f-235">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a948f-236">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a948f-236">Service Fabric</span></span>

* <span data-ttu-id="a948f-237">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="a948f-237">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="a948f-238">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-238">February 26, 2019</span></span>

<span data-ttu-id="a948f-239">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="a948f-239">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="a948f-240">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-240">Core</span></span>

* <span data-ttu-id="a948f-241">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="a948f-241">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-242">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-242">ACR</span></span>

* <span data-ttu-id="a948f-243">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="a948f-243">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="a948f-244">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-244">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-245">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-245">ACS</span></span>

* <span data-ttu-id="a948f-246">Adição da opção `--listen-address` a</span><span class="sxs-lookup"><span data-stu-id="a948f-246">Added `--listen-address` option to</span></span> `aks port-forward`

### <a name="appservice"></a><span data-ttu-id="a948f-247">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-247">AppService</span></span>

* <span data-ttu-id="a948f-248">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="a948f-248">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-249">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-249">Batch</span></span>
* <span data-ttu-id="a948f-250">[ALTERAÇÃO DA FALHA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="a948f-250">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="a948f-251">[ALTERAÇÃO DA FALHA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="a948f-251">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="a948f-252">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-252">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="a948f-253">[ALTERAÇÃO DA FALHA] `--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="a948f-253">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="a948f-254">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="a948f-254">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="a948f-255">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-255">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-256">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-256">CosmosDB</span></span>

* <span data-ttu-id="a948f-257">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a948f-257">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="a948f-258">Kusto</span><span class="sxs-lookup"><span data-stu-id="a948f-258">Kusto</span></span>

* <span data-ttu-id="a948f-259">[ALTERAÇÃO DA FALHA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="a948f-259">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="a948f-260">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-260">Network</span></span>

* <span data-ttu-id="a948f-261">Adicionado argumento `--express-route-gateway-bypass` a</span><span class="sxs-lookup"><span data-stu-id="a948f-261">Added `--express-route-gateway-bypass` argument to</span></span> `vpn-connection [create|update]`
* <span data-ttu-id="a948f-262">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="a948f-262">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="a948f-263">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-263">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="a948f-264">Adicionado argumento `--legacy-mode` a</span><span class="sxs-lookup"><span data-stu-id="a948f-264">Added argument `--legacy-mode` to</span></span> `express-route peering [create|update]` 
* <span data-ttu-id="a948f-265">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a</span><span class="sxs-lookup"><span data-stu-id="a948f-265">Added arguments `--allow-classic-operations` and `--express-route-port` to</span></span> `express-route [create|update]`
* <span data-ttu-id="a948f-266">Adicionado argumento `--gateway-default-site` a</span><span class="sxs-lookup"><span data-stu-id="a948f-266">Added `--gateway-default-site` argument to</span></span> `vnet-gateway [create|update]`
* <span data-ttu-id="a948f-267">Adicionados comandos `ipsec-policy` a</span><span class="sxs-lookup"><span data-stu-id="a948f-267">Added `ipsec-policy` commands to</span></span> `vnet-gateway`

### <a name="resource"></a><span data-ttu-id="a948f-268">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-268">Resource</span></span>

* <span data-ttu-id="a948f-269">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-269">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="a948f-270">Adicionado suporte para arquivo de parâmetros de URI a</span><span class="sxs-lookup"><span data-stu-id="a948f-270">Added support for URI-based parameters file to</span></span> `policy assignment create`
* <span data-ttu-id="a948f-271">Adicionado suporte para parâmetros de URI e definições a</span><span class="sxs-lookup"><span data-stu-id="a948f-271">Added support for URI-based parameters and definitions to</span></span> `policy set-definition update`
* <span data-ttu-id="a948f-272">Corrigido o tratamento de parâmetros e regras para</span><span class="sxs-lookup"><span data-stu-id="a948f-272">Fixed handling of parameters and rules for</span></span> `policy definition update`
* <span data-ttu-id="a948f-273">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-273">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="a948f-274">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-274">Role</span></span>

* <span data-ttu-id="a948f-275">Adicionado suporte para as funções do aplicativo a</span><span class="sxs-lookup"><span data-stu-id="a948f-275">Added support for app roles to</span></span> `ad app [create|update]`

### <a name="vm"></a><span data-ttu-id="a948f-276">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-276">VM</span></span>

* <span data-ttu-id="a948f-277">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="a948f-277">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="a948f-278">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-278">February 12, 2019</span></span>

<span data-ttu-id="a948f-279">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="a948f-279">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="a948f-280">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-280">Core</span></span>

* `az --version` <span data-ttu-id="a948f-281">agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="a948f-281">now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="a948f-282">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="a948f-282">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-283">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-283">ACR</span></span>
* <span data-ttu-id="a948f-284">[ALTERAÇÃO DA FALHA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="a948f-284">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="a948f-285">[ALTERAÇÃO DA FALHA] As opções `--tag` e `--manifest` foram removidas de</span><span class="sxs-lookup"><span data-stu-id="a948f-285">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from</span></span> `acr repository delete`

### <a name="acs"></a><span data-ttu-id="a948f-286">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-286">ACS</span></span>
* <span data-ttu-id="a948f-287">Suporte adicionado para nomes que não diferenciam maiúsculas de minúsculas a</span><span class="sxs-lookup"><span data-stu-id="a948f-287">Added support for case-insensitive names to</span></span> `aks [enable-addons|disable-addons]`
* <span data-ttu-id="a948f-288">Suporte adicionado para a operação de atualização do Azure Active Directory usando</span><span class="sxs-lookup"><span data-stu-id="a948f-288">Added support for Azure Active Directory updating operation using</span></span> `aks update-credentials --reset-aad`
* <span data-ttu-id="a948f-289">Adicionado um esclarecimento informando que `--output` é ignorado para</span><span class="sxs-lookup"><span data-stu-id="a948f-289">Added clarification that `--output` is ignored for</span></span> `aks get-credentials`

### <a name="ams"></a><span data-ttu-id="a948f-290">AMS</span><span class="sxs-lookup"><span data-stu-id="a948f-290">AMS</span></span>
* <span data-ttu-id="a948f-291">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="a948f-291">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="a948f-292">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="a948f-292">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-293">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-293">Appservice</span></span>
* <span data-ttu-id="a948f-294">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-294">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="a948f-295">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="a948f-295">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="a948f-296">A ajuda foi aprimorada para</span><span class="sxs-lookup"><span data-stu-id="a948f-296">Improved help for</span></span> `appservice-plan-update`
* <span data-ttu-id="a948f-297">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="a948f-297">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="a948f-298">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="a948f-298">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="a948f-299">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="a948f-299">Botservice</span></span>
* <span data-ttu-id="a948f-300">A experiência do usuário foi aprimorada para</span><span class="sxs-lookup"><span data-stu-id="a948f-300">Improved UX for</span></span> `bot publish`
* <span data-ttu-id="a948f-301">Adicionados avisos de tempos limite ao executar `npm install` durante</span><span class="sxs-lookup"><span data-stu-id="a948f-301">Added warning for timeouts when running `npm install` during</span></span> `az bot publish`
* <span data-ttu-id="a948f-302">O caractere inválido `.` de `--name` foi removido em</span><span class="sxs-lookup"><span data-stu-id="a948f-302">Removed invalid char `.` from `--name`  in</span></span> `az bot create`
* <span data-ttu-id="a948f-303">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="a948f-303">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="a948f-304">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de</span><span class="sxs-lookup"><span data-stu-id="a948f-304">[DEPRECATED] Deprecated `--proj-name` argument in favor of</span></span> `--proj-file-path`
* <span data-ttu-id="a948f-305">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="a948f-305">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="a948f-306">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-306">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="a948f-307">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="a948f-307">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="a948f-308">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="a948f-308">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="a948f-309">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="a948f-309">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="a948f-310">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a948f-310">Key Vault</span></span>
* <span data-ttu-id="a948f-311">Corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar</span><span class="sxs-lookup"><span data-stu-id="a948f-311">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using</span></span> `--id`

### <a name="monitor"></a><span data-ttu-id="a948f-312">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-312">Monitor</span></span>
* <span data-ttu-id="a948f-313">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional</span><span class="sxs-lookup"><span data-stu-id="a948f-313">Changed `monitor metrics alert [create|update]` to allow dimension value</span></span> `*`

### <a name="network"></a><span data-ttu-id="a948f-314">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-314">Network</span></span>
* <span data-ttu-id="a948f-315">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="a948f-315">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="a948f-316">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-316">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="a948f-317">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="a948f-317">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="a948f-318">`--idle-timeout` e `--floating-ip` foram adicionados a</span><span class="sxs-lookup"><span data-stu-id="a948f-318">Added `--idle-timeout` and `--floating-ip` to</span></span> `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a><span data-ttu-id="a948f-319">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="a948f-319">Policy Insights</span></span>
* <span data-ttu-id="a948f-320">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="a948f-320">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-321">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-321">RDBMS</span></span>
* <span data-ttu-id="a948f-322">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="a948f-322">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="a948f-323">Redis</span><span class="sxs-lookup"><span data-stu-id="a948f-323">Redis</span></span>
* <span data-ttu-id="a948f-324">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="a948f-324">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="a948f-325">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="a948f-325">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="a948f-326">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="a948f-326">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="a948f-327">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="a948f-327">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="a948f-328">[ALTERAÇÃO DA FALHA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="a948f-328">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="a948f-329">[ALTERAÇÃO DA FALHA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="a948f-329">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="a948f-330">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="a948f-330">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="a948f-331">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-331">Role</span></span>
* <span data-ttu-id="a948f-332">[ALTERAÇÃO DA FALHA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="a948f-332">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="a948f-333">SQL VM</span><span class="sxs-lookup"><span data-stu-id="a948f-333">SQL VM</span></span>
* <span data-ttu-id="a948f-334">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="a948f-334">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-335">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-335">VM</span></span>
* <span data-ttu-id="a948f-336">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de</span><span class="sxs-lookup"><span data-stu-id="a948f-336">Changed `vm list-skus` to allow use of `--all` in place of</span></span> `--all true`
* <span data-ttu-id="a948f-337">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-337">Added</span></span> `vmss run-command [invoke | list | show]`
* <span data-ttu-id="a948f-338">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="a948f-338">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="a948f-339">[ALTERAÇÃO DA FALHA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="a948f-339">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="a948f-340">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-340">January 31, 2019</span></span>

<span data-ttu-id="a948f-341">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="a948f-341">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="a948f-342">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-342">Core</span></span>

* <span data-ttu-id="a948f-343">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="a948f-343">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="a948f-344">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-344">January 28, 2019</span></span>

<span data-ttu-id="a948f-345">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="a948f-345">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-346">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-346">ACR</span></span>
* <span data-ttu-id="a948f-347">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="a948f-347">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-348">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-348">ACS</span></span>
* <span data-ttu-id="a948f-349">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="a948f-349">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a948f-350">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-350">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="a948f-351">Suporte adicionado para operações de atualização da entidade de serviço com</span><span class="sxs-lookup"><span data-stu-id="a948f-351">Added support for service principal updates operation with</span></span> `aks update-credentials -reset-service-principal`

### <a name="ams"></a><span data-ttu-id="a948f-352">AMS</span><span class="sxs-lookup"><span data-stu-id="a948f-352">AMS</span></span>
* <span data-ttu-id="a948f-353">[ALTERAÇÃO DA FALHA] `ams asset get-streaming-locators` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-353">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to</span></span> `ams asset list-streaming-locators`
* <span data-ttu-id="a948f-354">[ALTERAÇÃO DA FALHA] `ams streaming-locator get-content-keys` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-354">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to</span></span> `ams streaming-locator list-content-keys`

### <a name="appservice"></a><span data-ttu-id="a948f-355">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-355">Appservice</span></span>
* <span data-ttu-id="a948f-356">Suporte adicionado para o App Insights no</span><span class="sxs-lookup"><span data-stu-id="a948f-356">Added support for app insights on</span></span> `functionapp create`
* <span data-ttu-id="a948f-357">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="a948f-357">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="a948f-358">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="a948f-358">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="a948f-359">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-359">Container</span></span>
* <span data-ttu-id="a948f-360">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="a948f-360">Added `container start` command</span></span>
* <span data-ttu-id="a948f-361">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-361">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a948f-362">EventGrid</span><span class="sxs-lookup"><span data-stu-id="a948f-362">EventGrid</span></span>
* <span data-ttu-id="a948f-363">Parâmetro `--deadletter-endpoint` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-363">Added `--deadletter-endpoint` parameter to</span></span> `event-subscription [create|update]`
* <span data-ttu-id="a948f-364">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="a948f-364">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="a948f-365">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-365">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="a948f-366">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="a948f-366">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="a948f-367">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-367">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a948f-368">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a948f-368">HDInsight</span></span>
* <span data-ttu-id="a948f-369">[ALTERAÇÃO DA FALHA] Os parâmetros `--virtual-network` e `--subnet-name` foram removidos de</span><span class="sxs-lookup"><span data-stu-id="a948f-369">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from</span></span> `hdinsight [application] create`
* <span data-ttu-id="a948f-370">[ALTERAÇÃO DA FALHA] `hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="a948f-370">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="a948f-371">Parâmetros `--vnet-name` e `--subnet-name` adicionados a</span><span class="sxs-lookup"><span data-stu-id="a948f-371">Added `--vnet-name` and `--subnet-name` parameters to</span></span> `hdinsight create`
* <span data-ttu-id="a948f-372">Suporte adicionado para a criptografia de disco e Enterprise Security Package a</span><span class="sxs-lookup"><span data-stu-id="a948f-372">Added support for Enterprise Security Package and disk encryption to</span></span> `hdinsight create` 
* <span data-ttu-id="a948f-373">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="a948f-373">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="a948f-374">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="a948f-374">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-375">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-375">IoT</span></span>
* <span data-ttu-id="a948f-376">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="a948f-376">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="a948f-377">Kusto</span><span class="sxs-lookup"><span data-stu-id="a948f-377">Kusto</span></span>
* <span data-ttu-id="a948f-378">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-378">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-379">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-379">Monitor</span></span>
* <span data-ttu-id="a948f-380">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-380">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="a948f-381">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-381">Profile</span></span>
* <span data-ttu-id="a948f-382">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de</span><span class="sxs-lookup"><span data-stu-id="a948f-382">Enable tenant level account for managed service identity for</span></span> `login`

### <a name="network"></a><span data-ttu-id="a948f-383">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-383">Network</span></span>
* <span data-ttu-id="a948f-384">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="a948f-384">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="a948f-385">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="a948f-385">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-386">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-386">Resource</span></span>
* <span data-ttu-id="a948f-387">Suporte adicionado para o arquivo de parâmetros de URI à</span><span class="sxs-lookup"><span data-stu-id="a948f-387">Added support for URI parameters file to</span></span> `group deployment create`
* <span data-ttu-id="a948f-388">Suporte adicionado para a identidade gerenciada à</span><span class="sxs-lookup"><span data-stu-id="a948f-388">Added support for managed identity to</span></span> `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a><span data-ttu-id="a948f-389">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-389">SQL Virtual Machine</span></span>
* <span data-ttu-id="a948f-390">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-390">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-391">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-391">Storage</span></span>
* <span data-ttu-id="a948f-392">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="a948f-392">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="a948f-393">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="a948f-393">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-394">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-394">VM</span></span>
* <span data-ttu-id="a948f-395">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="a948f-395">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="a948f-396">O sinalizador `--force` foi adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-396">Added `--force` flag to</span></span> `vm encryption enable`

## <a name="january-15-2019"></a><span data-ttu-id="a948f-397">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="a948f-397">January 15, 2019</span></span>

<span data-ttu-id="a948f-398">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="a948f-398">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-399">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-399">ACR</span></span>
* <span data-ttu-id="a948f-400">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="a948f-400">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="a948f-401">Alteração para permitir operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="a948f-401">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="a948f-402">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="a948f-402">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="a948f-403">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-403">ACS</span></span>
* <span data-ttu-id="a948f-404">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="a948f-404">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-405">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-405">Appservice</span></span>
* <span data-ttu-id="a948f-406">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="a948f-406">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="a948f-407">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="a948f-407">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="a948f-408">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="a948f-408">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="a948f-409">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="a948f-409">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="a948f-410">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="a948f-410">Botservice</span></span>
* <span data-ttu-id="a948f-411">Atualizações de status de implantação foram adicionadas a</span><span class="sxs-lookup"><span data-stu-id="a948f-411">Added deployment status updates to</span></span> `bot create`

### <a name="configure"></a><span data-ttu-id="a948f-412">Configurar</span><span class="sxs-lookup"><span data-stu-id="a948f-412">Configure</span></span>
* <span data-ttu-id="a948f-413">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="a948f-413">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-414">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-414">CosmosDB</span></span>
* <span data-ttu-id="a948f-415">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="a948f-415">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a948f-416">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a948f-416">HDInsight</span></span>
* <span data-ttu-id="a948f-417">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="a948f-417">Added commands for managing applications</span></span>
* <span data-ttu-id="a948f-418">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="a948f-418">Added commands for managing script actions</span></span>
* <span data-ttu-id="a948f-419">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="a948f-419">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="a948f-420">Suporte adicionado para listar a utilização regional a</span><span class="sxs-lookup"><span data-stu-id="a948f-420">Added support to list regional usage to</span></span> `hdinsight list-usage`
* <span data-ttu-id="a948f-421">[ALTERAÇÃO DA FALHA] Removido o tipo de cluster padrão de</span><span class="sxs-lookup"><span data-stu-id="a948f-421">[BREAKING CHANGE] Removed default cluster type from</span></span> `hdinsight create`

### <a name="network"></a><span data-ttu-id="a948f-422">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-422">Network</span></span>
* <span data-ttu-id="a948f-423">Adicionados argumentos `--custom-headers` e `--status-code-ranges` a</span><span class="sxs-lookup"><span data-stu-id="a948f-423">Added `--custom-headers` and `--status-code-ranges` arguments to</span></span> `traffic-manager profile [create|update]`
* <span data-ttu-id="a948f-424">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="a948f-424">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="a948f-425">Adicionados argumentos `--custom-headers` e `--subnets` a</span><span class="sxs-lookup"><span data-stu-id="a948f-425">Added `--custom-headers` and `--subnets` arguments to</span></span> `traffic-manager endpoint [create|update]`  
* <span data-ttu-id="a948f-426">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="a948f-426">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="a948f-427">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-427">Role</span></span>
* <span data-ttu-id="a948f-428">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="a948f-428">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="a948f-429">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="a948f-429">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="a948f-430">Segurança</span><span class="sxs-lookup"><span data-stu-id="a948f-430">Security</span></span>
* <span data-ttu-id="a948f-431">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-431">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-432">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-432">Storage</span></span>
* <span data-ttu-id="a948f-433">[ALTERAÇÃO DA FALHA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="a948f-433">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="a948f-434">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="a948f-434">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="a948f-435">Parâmetro `--marker` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-435">Added `--marker` parameter to</span></span> `storage [blob|file|container|share] list`
* <span data-ttu-id="a948f-436">Um marcador de log foi adicionado para a próxima página ao STDERR de</span><span class="sxs-lookup"><span data-stu-id="a948f-436">Added log marker for next page to STDERR for</span></span> `storage [blob|file|container|share] list` 
* <span data-ttu-id="a948f-437">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="a948f-437">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-438">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-438">VM</span></span>
* <span data-ttu-id="a948f-439">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="a948f-439">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="a948f-440">Suporte adicionado para referência cruzada de imagem de locatário a</span><span class="sxs-lookup"><span data-stu-id="a948f-440">Added support for cross tenant image referencing to</span></span> `[vm|vmss] create`
* <span data-ttu-id="a948f-441">O bug de configuração padrão foi corrigido em</span><span class="sxs-lookup"><span data-stu-id="a948f-441">Fixed bug with default configuration in</span></span> `vm diagnostics get-default-config --windows-os`
* <span data-ttu-id="a948f-442">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="a948f-442">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="a948f-443">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-443">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="a948f-444">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="a948f-444">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="a948f-445">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-445">December 20, 2018</span></span>

<span data-ttu-id="a948f-446">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="a948f-446">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="a948f-447">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-447">Appservice</span></span>
* <span data-ttu-id="a948f-448">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="a948f-448">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="a948f-449">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="a948f-449">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="a948f-450">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-450">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a948f-451">IoT Central</span><span class="sxs-lookup"><span data-stu-id="a948f-451">IoTCentral</span></span>
* <span data-ttu-id="a948f-452">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="a948f-452">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="a948f-453">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-453">Role</span></span>
* <span data-ttu-id="a948f-454">[ALTERAÇÃO DA FALHA] `ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-454">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-455">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-455">SQL</span></span>
* <span data-ttu-id="a948f-456">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="a948f-456">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-457">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-457">VM</span></span>
* <span data-ttu-id="a948f-458">Parâmetro `---os-type` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-458">Added `---os-type` parameter to</span></span> `disk create`

## <a name="december-18-2018"></a><span data-ttu-id="a948f-459">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-459">December 18, 2018</span></span>

<span data-ttu-id="a948f-460">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="a948f-460">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="a948f-461">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-461">ACR</span></span>
* <span data-ttu-id="a948f-462">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="a948f-462">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="a948f-463">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="a948f-463">Condensed the table layout for task list</span></span>
* <span data-ttu-id="a948f-464">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="a948f-464">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-465">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-465">ACS</span></span>
* <span data-ttu-id="a948f-466">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="a948f-466">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="a948f-467">Removido “(VERSÃO PRÉVIA)” de argumentos do AAD para</span><span class="sxs-lookup"><span data-stu-id="a948f-467">Removed "(PREVIEW)" from AAD arguments to</span></span> `aks create`
* <span data-ttu-id="a948f-468">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="a948f-468">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="a948f-469">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="a948f-469">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="a948f-470">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-470">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="a948f-471">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="a948f-471">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-472">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-472">Appservice</span></span>
* <span data-ttu-id="a948f-473">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="a948f-473">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="a948f-474">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="a948f-474">Botservice</span></span>
* <span data-ttu-id="a948f-475">Suporte adicionado para análise do arquivo `.bot` ao chamar</span><span class="sxs-lookup"><span data-stu-id="a948f-475">Added support for `.bot` file parsing when calling</span></span> `bot show`
* <span data-ttu-id="a948f-476">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="a948f-476">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="a948f-477">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="a948f-477">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="a948f-478">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="a948f-478">Reduced Kudu network calls</span></span>
* <span data-ttu-id="a948f-479">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="a948f-479">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="a948f-480">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-480">Consumption</span></span>
* <span data-ttu-id="a948f-481">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="a948f-481">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-482">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-482">CosmosDB</span></span>
* <span data-ttu-id="a948f-483">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="a948f-483">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="a948f-484">Mapas</span><span class="sxs-lookup"><span data-stu-id="a948f-484">Maps</span></span>
* <span data-ttu-id="a948f-485">Adicionado suporte para o SKU S1 a</span><span class="sxs-lookup"><span data-stu-id="a948f-485">Added support for the S1 SKU to</span></span> `maps account [create|update]`

### <a name="network"></a><span data-ttu-id="a948f-486">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-486">Network</span></span>
* <span data-ttu-id="a948f-487">Adicionado suporte para `--format` e `--log-version` a</span><span class="sxs-lookup"><span data-stu-id="a948f-487">Added support for `--format` and `--log-version` to</span></span> `watcher flow-log configure`
* <span data-ttu-id="a948f-488">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="a948f-488">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-489">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-489">Resource</span></span>
* <span data-ttu-id="a948f-490">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do</span><span class="sxs-lookup"><span data-stu-id="a948f-490">Fixed handling of scope parameter for management groups in</span></span> `policy assignment [create|list|delete|show|update]` 
* <span data-ttu-id="a948f-491">Adicionado novo comando</span><span class="sxs-lookup"><span data-stu-id="a948f-491">Added new command</span></span> `resource wait`

### <a name="storage"></a><span data-ttu-id="a948f-492">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-492">Storage</span></span>
*  <span data-ttu-id="a948f-493">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no</span><span class="sxs-lookup"><span data-stu-id="a948f-493">Added ability to update log schema version for storage services in</span></span> `storage logging update`

### <a name="vm"></a><span data-ttu-id="a948f-494">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-494">VM</span></span>
* <span data-ttu-id="a948f-495">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="a948f-495">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="a948f-496">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-496">December 4, 2018</span></span>

<span data-ttu-id="a948f-497">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="a948f-497">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="a948f-498">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-498">Core</span></span>
* <span data-ttu-id="a948f-499">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="a948f-499">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="a948f-500">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-500">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-501">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-501">Appservice</span></span>
* <span data-ttu-id="a948f-502">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-502">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="a948f-503">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="a948f-503">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="a948f-504">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-504">Network</span></span>
* <span data-ttu-id="a948f-505">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="a948f-505">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="a948f-506">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-506">Role</span></span>
* <span data-ttu-id="a948f-507">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="a948f-507">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="a948f-508">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-508">VM</span></span>
* <span data-ttu-id="a948f-509">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="a948f-509">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="a948f-510">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="a948f-510">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="a948f-511">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="a948f-511">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="a948f-512">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-512">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="a948f-513">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-513">November 20, 2018</span></span>

<span data-ttu-id="a948f-514">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="a948f-514">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="a948f-515">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-515">Core</span></span>
* <span data-ttu-id="a948f-516">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="a948f-516">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-517">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-517">ACR</span></span>
* <span data-ttu-id="a948f-518">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="a948f-518">Added context token to task step</span></span>
* <span data-ttu-id="a948f-519">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="a948f-519">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="a948f-520">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="a948f-520">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-521">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-521">Appservice</span></span>
* <span data-ttu-id="a948f-522">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="a948f-522">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="a948f-523">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="a948f-523">Updated the default `node_version`.</span></span> <span data-ttu-id="a948f-524">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="a948f-524">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="a948f-525">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-525">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="a948f-526">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="a948f-526">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="a948f-527">Iot Central</span><span class="sxs-lookup"><span data-stu-id="a948f-527">IotCentral</span></span>
* <span data-ttu-id="a948f-528">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="a948f-528">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-529">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a948f-529">KeyVault</span></span>
* <span data-ttu-id="a948f-530">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="a948f-530">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="a948f-531">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-531">Network</span></span>
* <span data-ttu-id="a948f-532">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="a948f-532">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="a948f-533">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="a948f-533">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="a948f-534">`--zones` adicionado para suporte da zona de disponibilidade a</span><span class="sxs-lookup"><span data-stu-id="a948f-534">Added `--zones` for availability zone support to</span></span> `application-gateway create` 
* <span data-ttu-id="a948f-535">Os argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` foram adicionados a</span><span class="sxs-lookup"><span data-stu-id="a948f-535">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to</span></span> `application-gateway waf-config set`

### <a name="rdbms"></a><span data-ttu-id="a948f-536">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a948f-536">Rdbms</span></span>
* <span data-ttu-id="a948f-537">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-537">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="a948f-538">Rbac</span><span class="sxs-lookup"><span data-stu-id="a948f-538">Rbac</span></span>
* <span data-ttu-id="a948f-539">Problema corrigido ao tentar atualizar credenciais inalteradas em</span><span class="sxs-lookup"><span data-stu-id="a948f-539">Fixed an issue with attempting to update immutable credentials in</span></span> `ad app update`
* <span data-ttu-id="a948f-540">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para</span><span class="sxs-lookup"><span data-stu-id="a948f-540">Added output warnings to communicate breaking changes in the near future for</span></span> `ad [app|sp] list` 

### <a name="storage"></a><span data-ttu-id="a948f-541">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-541">Storage</span></span>
* <span data-ttu-id="a948f-542">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-542">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="a948f-543">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="a948f-543">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="a948f-544">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="a948f-544">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="a948f-545">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-545">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-546">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-546">VM</span></span>
* <span data-ttu-id="a948f-547">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="a948f-547">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="a948f-548">Parâmetros do nome da versão de `sig image-version` alterados para</span><span class="sxs-lookup"><span data-stu-id="a948f-548">Changed version name parameters to `sig image-version` to be</span></span> `--image-version -e`
* <span data-ttu-id="a948f-549">Argumento `sig image-version` preterido `--image-version-name`, substituído por</span><span class="sxs-lookup"><span data-stu-id="a948f-549">Deprecated `sig image-version` argument `--image-version-name`, replaced by</span></span> `--image-version`
* <span data-ttu-id="a948f-550">Suporte adicionado para usar o disco local do SO a</span><span class="sxs-lookup"><span data-stu-id="a948f-550">Added support to use local OS disk to</span></span> `[vm|vmss] create --ephemeral-os-disk`
* <span data-ttu-id="a948f-551">Adição do suporte para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-551">Added support for `--no-wait` to</span></span> `snapshot create/update`
* <span data-ttu-id="a948f-552">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="a948f-552">Added `snapshot wait` command</span></span>
* <span data-ttu-id="a948f-553">Suporte adicionado para usar o nome da instância com</span><span class="sxs-lookup"><span data-stu-id="a948f-553">Added support for using instance name with</span></span> `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a><span data-ttu-id="a948f-554">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-554">November 6, 2018</span></span>

<span data-ttu-id="a948f-555">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="a948f-555">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="a948f-556">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-556">Core</span></span>
* <span data-ttu-id="a948f-557">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="a948f-557">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-558">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-558">ACR</span></span>
* <span data-ttu-id="a948f-559">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="a948f-559">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="a948f-560">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="a948f-560">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-561">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-561">ACS</span></span>
* <span data-ttu-id="a948f-562">[ALTERAÇÃO DA FALHA] `enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-562">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="a948f-563">Supervisor</span><span class="sxs-lookup"><span data-stu-id="a948f-563">Advisor</span></span>
* <span data-ttu-id="a948f-564">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="a948f-564">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="a948f-565">AMS</span><span class="sxs-lookup"><span data-stu-id="a948f-565">AMS</span></span>
* <span data-ttu-id="a948f-566">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="a948f-566">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="a948f-567">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="a948f-567">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="a948f-568">Adicionado suporte aos parâmetros de criptografia a</span><span class="sxs-lookup"><span data-stu-id="a948f-568">Added encryption parameters support to</span></span> `ams streaming-policy create`
* <span data-ttu-id="a948f-569">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="a948f-569">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="a948f-570">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="a948f-570">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="a948f-571">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="a948f-571">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="a948f-572">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="a948f-572">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="a948f-573">[ALTERAÇÃO DA FALHA] O comando `ams streaming locator` foi substituído por</span><span class="sxs-lookup"><span data-stu-id="a948f-573">[BREAKING CHANGE] Replaced `ams streaming locator` command with</span></span> `ams streaming-locator`
* <span data-ttu-id="a948f-574">[ALTERAÇÃO DA FALHA] O argumento `--content-keys` foi atualizado de</span><span class="sxs-lookup"><span data-stu-id="a948f-574">[BREAKING CHANGE] Updated `--content-keys` argument of</span></span> `ams streaming locator`
* <span data-ttu-id="a948f-575">[ALTERAÇÃO DA FALHA] `--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="a948f-575">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="a948f-576">[ALTERAÇÃO DA FALHA] O comando `ams streaming policy` foi substituído por</span><span class="sxs-lookup"><span data-stu-id="a948f-576">[BREAKING CHANGE] Replaced `ams streaming policy` command with</span></span> `ams streaming-policy`
* <span data-ttu-id="a948f-577">[ALTERAÇÃO DA FALHA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="a948f-577">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="a948f-578">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="a948f-578">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="a948f-579">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="a948f-579">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="a948f-580">[ALTERAÇÃO DA FALHA] `--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="a948f-580">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="a948f-581">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="a948f-581">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="a948f-582">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="a948f-582">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-583">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-583">AppService</span></span>
* <span data-ttu-id="a948f-584">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="a948f-584">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="a948f-585">Configurar</span><span class="sxs-lookup"><span data-stu-id="a948f-585">Configure</span></span>
* <span data-ttu-id="a948f-586">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="a948f-586">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="a948f-587">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-587">Container</span></span>
* <span data-ttu-id="a948f-588">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="a948f-588">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="a948f-589">EventHub</span><span class="sxs-lookup"><span data-stu-id="a948f-589">EventHub</span></span>
* <span data-ttu-id="a948f-590">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no</span><span class="sxs-lookup"><span data-stu-id="a948f-590">Added `--enable-kafka` flag to support Kafka in</span></span> `eventhub namespace [create|update]`

### <a name="interactive"></a><span data-ttu-id="a948f-591">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-591">Interactive</span></span>
* <span data-ttu-id="a948f-592">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="a948f-592">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-593">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-593">Monitor</span></span>
* <span data-ttu-id="a948f-594">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) a `--condition` em</span><span class="sxs-lookup"><span data-stu-id="a948f-594">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="a948f-595">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-595">Network</span></span>
* <span data-ttu-id="a948f-596">Os nomes de comandos `network interface-endpoint` foram preteridos em favor de</span><span class="sxs-lookup"><span data-stu-id="a948f-596">Deprecated `network interface-endpoint` command names in favor of</span></span> `network private-endpoint`
* <span data-ttu-id="a948f-597">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="a948f-597">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="a948f-598">Corrigido problema em que `--ip-tags` não funcionava corretamente com</span><span class="sxs-lookup"><span data-stu-id="a948f-598">Fixed issue where `--ip-tags` did not work correctly with</span></span> `public-ip create` 

### <a name="profile"></a><span data-ttu-id="a948f-599">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-599">Profile</span></span>
* <span data-ttu-id="a948f-600">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="a948f-600">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-601">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-601">RDBMS</span></span>
* <span data-ttu-id="a948f-602">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="a948f-602">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-603">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-603">Resource</span></span>
* <span data-ttu-id="a948f-604">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="a948f-604">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="a948f-605">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-605">Role</span></span>
* <span data-ttu-id="a948f-606">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="a948f-606">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="a948f-607">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-607">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="a948f-608">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="a948f-608">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-609">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-609">Storage</span></span>
* <span data-ttu-id="a948f-610">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="a948f-610">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-611">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-611">VM</span></span>
* <span data-ttu-id="a948f-612">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-612">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="a948f-613">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="a948f-613">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="a948f-614">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="a948f-614">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="a948f-615">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="a948f-615">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="a948f-616">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="a948f-616">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="a948f-617">Validação de argumento aprimorada para</span><span class="sxs-lookup"><span data-stu-id="a948f-617">Improved argument validation for</span></span> `vm create --image`

## <a name="october-23-2018"></a><span data-ttu-id="a948f-618">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-618">October 23, 2018</span></span>

<span data-ttu-id="a948f-619">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="a948f-619">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="a948f-620">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-620">Core</span></span>
* <span data-ttu-id="a948f-621">Corrigido o problema com `--ids` em que `--subscription` teria precedência sobre a assinatura em</span><span class="sxs-lookup"><span data-stu-id="a948f-621">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in</span></span> `--ids`
* <span data-ttu-id="a948f-622">Adicionados avisos explícitos quando os parâmetros seriam ignorados pelo uso de</span><span class="sxs-lookup"><span data-stu-id="a948f-622">Added explicit warnings when parameters would be ignored by use of</span></span> `--ids`

### <a name="acr"></a><span data-ttu-id="a948f-623">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-623">ACR</span></span>
* <span data-ttu-id="a948f-624">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="a948f-624">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="a948f-625">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-625">CDN</span></span>
* <span data-ttu-id="a948f-626">[ALTERAÇÃO DA FALHA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="a948f-626">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="a948f-627">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-627">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="a948f-628">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-628">Container</span></span>
* <span data-ttu-id="a948f-629">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="a948f-629">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="a948f-630">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="a948f-630">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="a948f-631">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="a948f-631">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="a948f-632">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="a948f-632">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="a948f-633">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="a948f-633">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="a948f-634">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="a948f-634">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="a948f-635">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="a948f-635">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-636">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-636">CosmosDB</span></span>
* <span data-ttu-id="a948f-637">Adicionado suporte `--enable-multiple-write-locations` a</span><span class="sxs-lookup"><span data-stu-id="a948f-637">Added `--enable-multiple-write-locations` support to</span></span> `cosmosdb create`

### <a name="interactive"></a><span data-ttu-id="a948f-638">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-638">Interactive</span></span>
* <span data-ttu-id="a948f-639">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="a948f-639">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="a948f-640">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-640">IoT Central</span></span>
* <span data-ttu-id="a948f-641">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="a948f-641">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="a948f-642">[ALTERAÇÃO DA FALHA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="a948f-642">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-643">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-643">Monitor</span></span>
* <span data-ttu-id="a948f-644">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="a948f-644">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="a948f-645">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-645">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="a948f-646">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="a948f-646">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a948f-647">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="a948f-647">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="a948f-648">Adicionado `--namespace` como alias para a opção preterida</span><span class="sxs-lookup"><span data-stu-id="a948f-648">Added `--namespace` as alias for deprecated option</span></span> `--resource-provider`
  * <span data-ttu-id="a948f-649">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-649">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="a948f-650">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="a948f-650">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="a948f-651">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="a948f-651">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="a948f-652">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="a948f-652">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="a948f-653">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para</span><span class="sxs-lookup"><span data-stu-id="a948f-653">Improved validation for `--event-hub` and `--event-hub-rule` arguments to</span></span> `monitor diagnostic-settings create`

### <a name="network"></a><span data-ttu-id="a948f-654">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-654">Network</span></span>
* <span data-ttu-id="a948f-655">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="a948f-655">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="a948f-656">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="a948f-656">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="a948f-657">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a948f-657">ServiceBus</span></span>
* <span data-ttu-id="a948f-658">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-658">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-659">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-659">SQL</span></span>
* <span data-ttu-id="a948f-660">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="a948f-660">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-661">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-661">Storage</span></span>
* <span data-ttu-id="a948f-662">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="a948f-662">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="a948f-663">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="a948f-663">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-664">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-664">VM</span></span>
* <span data-ttu-id="a948f-665">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no</span><span class="sxs-lookup"><span data-stu-id="a948f-665">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in</span></span> `[vm|vmss] create`
* <span data-ttu-id="a948f-666">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para</span><span class="sxs-lookup"><span data-stu-id="a948f-666">Updated supported size list supporting networking accelerator for</span></span> `vm create`
* <span data-ttu-id="a948f-667">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para</span><span class="sxs-lookup"><span data-stu-id="a948f-667">Added strong typed arguments for ultrassd iops and mbps configs for</span></span> `disk create`

## <a name="october-16-2018"></a><span data-ttu-id="a948f-668">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-668">October 16, 2018</span></span>

<span data-ttu-id="a948f-669">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="a948f-669">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-670">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-670">VM</span></span>
* <span data-ttu-id="a948f-671">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="a948f-671">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="a948f-672">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-672">October 9, 2018</span></span>

<span data-ttu-id="a948f-673">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="a948f-673">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="a948f-674">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-674">Core</span></span>
* <span data-ttu-id="a948f-675">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="a948f-675">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-676">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-676">ACR</span></span>
* <span data-ttu-id="a948f-677">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="a948f-677">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-678">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-678">ACS</span></span>
* <span data-ttu-id="a948f-679">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="a948f-679">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="a948f-680">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="a948f-680">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="a948f-681">`aks create` alterado para não precisar mais de</span><span class="sxs-lookup"><span data-stu-id="a948f-681">Changed `aks create` to no longer require</span></span> `--aad-tenant-id`
* <span data-ttu-id="a948f-682">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="a948f-682">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="a948f-683">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-683">Container</span></span>
* <span data-ttu-id="a948f-684">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="a948f-684">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="a948f-685">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-685">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="a948f-686">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="a948f-686">Event Hub</span></span>
* <span data-ttu-id="a948f-687">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="a948f-687">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="a948f-688">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="a948f-688">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="a948f-689">Extensões</span><span class="sxs-lookup"><span data-stu-id="a948f-689">Extensions</span></span>
* <span data-ttu-id="a948f-690">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="a948f-690">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="a948f-691">HDInsight</span><span class="sxs-lookup"><span data-stu-id="a948f-691">HDInsight</span></span>
* <span data-ttu-id="a948f-692">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-692">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-693">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-693">IoT</span></span>
* <span data-ttu-id="a948f-694">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-694">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-695">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a948f-695">KeyVault</span></span>
* <span data-ttu-id="a948f-696">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="a948f-696">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="a948f-697">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-697">Network</span></span>
* <span data-ttu-id="a948f-698">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="a948f-698">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="a948f-699">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="a948f-699">See #6052</span></span>
* <span data-ttu-id="a948f-700">Preterido `--remote-vnet-id` para</span><span class="sxs-lookup"><span data-stu-id="a948f-700">Deprecated `--remote-vnet-id` for</span></span> `network vnet peering create`
* <span data-ttu-id="a948f-701">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="a948f-701">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="a948f-702">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com</span><span class="sxs-lookup"><span data-stu-id="a948f-702">Added support for multiple subnet prefixes to `network vnet create` with</span></span> `--subnet-prefixes`
* <span data-ttu-id="a948f-703">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com</span><span class="sxs-lookup"><span data-stu-id="a948f-703">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with</span></span> `--address-prefixes`
* <span data-ttu-id="a948f-704">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="a948f-704">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="a948f-705">Argumento de conveniência `--service-endpoint-policy` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-705">Added `--service-endpoint-policy` convenience argument to</span></span> `network vnet subnet update`

### <a name="role"></a><span data-ttu-id="a948f-706">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-706">Role</span></span>
* <span data-ttu-id="a948f-707">Suporte adicionado para listar os proprietários de aplicativo do Azure Active Directory a</span><span class="sxs-lookup"><span data-stu-id="a948f-707">Added support for listing Azure AD app owners to</span></span> `ad app owner`
* <span data-ttu-id="a948f-708">Suporte adicionado para listar os proprietários da entidade de serviço do Azure Active Directory a</span><span class="sxs-lookup"><span data-stu-id="a948f-708">Added support for listing Azure AD service principal owners to</span></span> `ad sp owner`
* <span data-ttu-id="a948f-709">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="a948f-709">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="a948f-710">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="a948f-710">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="a948f-711">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-711">Service Bus</span></span>
* <span data-ttu-id="a948f-712">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="a948f-712">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-713">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-713">VM</span></span>
* <span data-ttu-id="a948f-714">Corrigido o campo `accessSas` vazio em</span><span class="sxs-lookup"><span data-stu-id="a948f-714">Fixed empty `accessSas` field in</span></span> `disk grant-access`
* <span data-ttu-id="a948f-715">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="a948f-715">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="a948f-716">Corrigidos os comandos de atualização para</span><span class="sxs-lookup"><span data-stu-id="a948f-716">Fixed update commands for</span></span> `sig`
* <span data-ttu-id="a948f-717">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em</span><span class="sxs-lookup"><span data-stu-id="a948f-717">Added `--no-wait` support for managing image versions in</span></span> `sig`
* <span data-ttu-id="a948f-718">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="a948f-718">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="a948f-719">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="a948f-719">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="a948f-720">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-720">September 21, 2018</span></span>

<span data-ttu-id="a948f-721">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="a948f-721">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-722">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-722">ACR</span></span>
* <span data-ttu-id="a948f-723">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-723">Added ACR Task commands</span></span>
* <span data-ttu-id="a948f-724">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="a948f-724">Added quick run command</span></span>
* <span data-ttu-id="a948f-725">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-725">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="a948f-726">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-726">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="a948f-727">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="a948f-727">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="a948f-728">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="a948f-728">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-729">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-729">ACS</span></span>
* <span data-ttu-id="a948f-730">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-730">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="a948f-731">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="a948f-731">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-732">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-732">AppService</span></span>

* <span data-ttu-id="a948f-733">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="a948f-733">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="a948f-734">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="a948f-734">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="a948f-735">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="a948f-735">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="a948f-736">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="a948f-736">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-737">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-737">Batch</span></span>
* <span data-ttu-id="a948f-738">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="a948f-738">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="a948f-739">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="a948f-739">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="a948f-740">`--max-tasks-per-node-option` foi adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-740">Added `--max-tasks-per-node-option` to</span></span> `batch pool create`
* <span data-ttu-id="a948f-741">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="a948f-741">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a948f-742">Lote AI</span><span class="sxs-lookup"><span data-stu-id="a948f-742">Batch AI</span></span> 
* <span data-ttu-id="a948f-743">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="a948f-743">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a948f-744">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-744">Cognitive Services</span></span>
* <span data-ttu-id="a948f-745">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="a948f-745">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="a948f-746">Adicionado comando</span><span class="sxs-lookup"><span data-stu-id="a948f-746">Added command</span></span> `cognitiveservices account list-usage`
* <span data-ttu-id="a948f-747">Adicionado comando</span><span class="sxs-lookup"><span data-stu-id="a948f-747">Added command</span></span> `cognitiveservices account list-kinds`
* <span data-ttu-id="a948f-748">Adicionado comando</span><span class="sxs-lookup"><span data-stu-id="a948f-748">Added command</span></span> `cognitiveservices account list`
* <span data-ttu-id="a948f-749">Preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-749">Deprecated</span></span> `cognitiveservices list`
* <span data-ttu-id="a948f-750">Alterado `--name` para que seja opcional para</span><span class="sxs-lookup"><span data-stu-id="a948f-750">Changed `--name` to be optional for</span></span> `cognitiveservices account list-skus`

### <a name="container"></a><span data-ttu-id="a948f-751">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-751">Container</span></span>
* <span data-ttu-id="a948f-752">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="a948f-752">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="a948f-753">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="a948f-753">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="a948f-754">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="a948f-754">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="a948f-755">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="a948f-755">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="a948f-756">DataLake</span><span class="sxs-lookup"><span data-stu-id="a948f-756">Datalake</span></span>
* <span data-ttu-id="a948f-757">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="a948f-757">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="a948f-758">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-758">Interactive Shell</span></span>
* <span data-ttu-id="a948f-759">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-759">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="a948f-760">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-760">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-761">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-761">IoT</span></span>
* <span data-ttu-id="a948f-762">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-762">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="a948f-763">Key Vault</span><span class="sxs-lookup"><span data-stu-id="a948f-763">Key Vault</span></span>
* <span data-ttu-id="a948f-764">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="a948f-764">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="a948f-765">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-765">Network</span></span>
* <span data-ttu-id="a948f-766">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="a948f-766">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="a948f-767">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-767">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="a948f-768">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="a948f-768">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="a948f-769">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="a948f-769">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="a948f-770">Adicionado `--enable-tcp-reset` a</span><span class="sxs-lookup"><span data-stu-id="a948f-770">Add `--enable-tcp-reset` to</span></span> `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* <span data-ttu-id="a948f-771">Adicionado `--disable-outbound-snat` a</span><span class="sxs-lookup"><span data-stu-id="a948f-771">Add `--disable-outbound-snat` to</span></span> `network lb rule create/update`
* <span data-ttu-id="a948f-772">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="a948f-772">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="a948f-773">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="a948f-773">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="a948f-774">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="a948f-774">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* `network express-route create/update`<span data-ttu-id="a948f-775">: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="a948f-775">: Add `--allow-global-reach` flag</span></span>
* `network vnet subnet create/update`<span data-ttu-id="a948f-776">: Adicionado suporte para</span><span class="sxs-lookup"><span data-stu-id="a948f-776">: Add support for</span></span> `--delegation`
* <span data-ttu-id="a948f-777">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="a948f-777">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="a948f-778">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="a948f-778">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="a948f-779">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="a948f-779">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* `dns record-set * create/update`<span data-ttu-id="a948f-780">: Adicionado suporte para</span><span class="sxs-lookup"><span data-stu-id="a948f-780">: Add support for</span></span> `--target-resource`
* <span data-ttu-id="a948f-781">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="a948f-781">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="a948f-782">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="a948f-782">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="a948f-783">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="a948f-783">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-784">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-784">RDBMS</span></span>
* <span data-ttu-id="a948f-785">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="a948f-785">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="a948f-786">Reserva</span><span class="sxs-lookup"><span data-stu-id="a948f-786">Reservation</span></span>
* <span data-ttu-id="a948f-787">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="a948f-787">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="a948f-788">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="a948f-788">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="a948f-789">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-789">Manage App</span></span>
* <span data-ttu-id="a948f-790">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="a948f-790">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="a948f-791">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="a948f-791">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="a948f-792">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-792">Role</span></span>
* <span data-ttu-id="a948f-793">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="a948f-793">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="a948f-794">SignalR</span><span class="sxs-lookup"><span data-stu-id="a948f-794">SignalR</span></span>
* <span data-ttu-id="a948f-795">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="a948f-795">First release</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-796">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-796">Storage</span></span>
* <span data-ttu-id="a948f-797">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="a948f-797">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="a948f-798">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="a948f-798">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-799">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-799">VM</span></span>
* <span data-ttu-id="a948f-800">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="a948f-800">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="a948f-801">Adicionado suporte para galeria de imagem compartilhada por meio de</span><span class="sxs-lookup"><span data-stu-id="a948f-801">Added support for shared image gallery through</span></span> `az sig`

## <a name="august-28-2018"></a><span data-ttu-id="a948f-802">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-802">August 28, 2018</span></span>

<span data-ttu-id="a948f-803">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="a948f-803">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="a948f-804">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-804">Core</span></span>

* <span data-ttu-id="a948f-805">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="a948f-805">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="a948f-806">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a948f-806">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-807">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-807">ACR</span></span>

* <span data-ttu-id="a948f-808">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="a948f-808">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="a948f-809">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="a948f-809">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-810">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-810">ACS</span></span>

* <span data-ttu-id="a948f-811">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="a948f-811">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="a948f-812">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="a948f-812">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-813">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-813">AppService</span></span>

* <span data-ttu-id="a948f-814">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="a948f-814">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="a948f-815">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-815">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="a948f-816">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-816">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="a948f-817">Backup</span><span class="sxs-lookup"><span data-stu-id="a948f-817">Backup</span></span>

* <span data-ttu-id="a948f-818">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-818">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="a948f-819">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="a948f-819">Bot Service</span></span>

* <span data-ttu-id="a948f-820">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-820">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a948f-821">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-821">Cognitive Services</span></span>

* <span data-ttu-id="a948f-822">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="a948f-822">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-823">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-823">IoT</span></span>

* <span data-ttu-id="a948f-824">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="a948f-824">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-825">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-825">Monitor</span></span>

* <span data-ttu-id="a948f-826">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="a948f-826">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="a948f-827">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-827">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a948f-828">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-828">Network</span></span>

* <span data-ttu-id="a948f-829">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-829">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-830">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-830">Resource</span></span>

* <span data-ttu-id="a948f-831">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-831">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-832">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-832">Storage</span></span>

* <span data-ttu-id="a948f-833">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-833">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-834">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-834">VM</span></span>

* <span data-ttu-id="a948f-835">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-835">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="a948f-836">Preterido `--storage-caching` para</span><span class="sxs-lookup"><span data-stu-id="a948f-836">Deprecated `--storage-caching` for</span></span> `vm create`

## <a name="auguest-14-2018"></a><span data-ttu-id="a948f-837">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-837">Auguest 14, 2018</span></span>

<span data-ttu-id="a948f-838">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="a948f-838">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="a948f-839">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-839">Core</span></span>

* <span data-ttu-id="a948f-840">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="a948f-840">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="a948f-841">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="a948f-841">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="a948f-842">Telemetria</span><span class="sxs-lookup"><span data-stu-id="a948f-842">Telemetry</span></span>

* <span data-ttu-id="a948f-843">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="a948f-843">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-844">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-844">ACR</span></span>

* <span data-ttu-id="a948f-845">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="a948f-845">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="a948f-846">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="a948f-846">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-847">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-847">ACS</span></span>

* <span data-ttu-id="a948f-848">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-848">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="a948f-849">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="a948f-849">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="a948f-850">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="a948f-850">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="a948f-851">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="a948f-851">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="a948f-852">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="a948f-852">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="a948f-853">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-853">AppService</span></span>

* <span data-ttu-id="a948f-854">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="a948f-854">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="a948f-855">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="a948f-855">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="a948f-856">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a948f-856">BatchAI</span></span>

* <span data-ttu-id="a948f-857">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="a948f-857">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="a948f-858">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-858">Container</span></span>

* <span data-ttu-id="a948f-859">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-859">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="a948f-860">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-860">IoT</span></span>

* <span data-ttu-id="a948f-861">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="a948f-861">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="a948f-862">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="a948f-862">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="a948f-863">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-863">Iot Central</span></span>

* <span data-ttu-id="a948f-864">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="a948f-864">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-865">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a948f-865">KeyVault</span></span>


* <span data-ttu-id="a948f-866">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="a948f-866">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="a948f-867">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="a948f-867">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="a948f-868">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="a948f-868">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="a948f-869">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="a948f-869">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="a948f-870">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="a948f-870">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="a948f-871">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="a948f-871">Relay</span></span>

* <span data-ttu-id="a948f-872">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-872">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-873">Sql</span><span class="sxs-lookup"><span data-stu-id="a948f-873">Sql</span></span>

* <span data-ttu-id="a948f-874">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="a948f-874">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-875">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-875">Storage</span></span>

* <span data-ttu-id="a948f-876">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="a948f-876">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="a948f-877">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="a948f-877">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="a948f-878">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="a948f-878">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="a948f-879">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="a948f-879">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="a948f-880">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-880">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-881">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-881">VM</span></span>

* <span data-ttu-id="a948f-882">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="a948f-882">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="a948f-883">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-883">July 31, 2018</span></span>

<span data-ttu-id="a948f-884">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="a948f-884">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-885">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-885">ACR</span></span>

* <span data-ttu-id="a948f-886">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="a948f-886">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="a948f-887">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="a948f-887">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-888">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-888">ACS</span></span>

* <span data-ttu-id="a948f-889">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="a948f-889">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-890">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-890">Batch</span></span>

* <span data-ttu-id="a948f-891">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="a948f-891">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="a948f-892">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-892">Container</span></span>

* <span data-ttu-id="a948f-893">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-893">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="a948f-894">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-894">Network</span></span>

* <span data-ttu-id="a948f-895">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a948f-895">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="a948f-896">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-896">Resource</span></span>

* <span data-ttu-id="a948f-897">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="a948f-897">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="a948f-898">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="a948f-898">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="a948f-899">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-899">Role</span></span>

* <span data-ttu-id="a948f-900">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="a948f-900">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="a948f-901">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-901">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="a948f-902">Search</span><span class="sxs-lookup"><span data-stu-id="a948f-902">Search</span></span>

* <span data-ttu-id="a948f-903">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="a948f-903">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="a948f-904">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-904">Service Bus</span></span>

* <span data-ttu-id="a948f-905">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="a948f-905">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="a948f-906">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-906">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  `--enable-batched-operations` <span data-ttu-id="a948f-907">e `--enable-dead-lettering-on-message-expiration` em</span><span class="sxs-lookup"><span data-stu-id="a948f-907">and `--enable-dead-lettering-on-message-expiration` in</span></span> `queue`
  *  `--dead-letter-on-filter-exceptions` <span data-ttu-id="a948f-908">mergulhar</span><span class="sxs-lookup"><span data-stu-id="a948f-908">in</span></span> `subscriptions`

### <a name="storage"></a><span data-ttu-id="a948f-909">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-909">Storage</span></span>

* <span data-ttu-id="a948f-910">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="a948f-910">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="a948f-911">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-911">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-912">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-912">VM</span></span>

* <span data-ttu-id="a948f-913">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-913">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="a948f-914">Adicionado suporte para</span><span class="sxs-lookup"><span data-stu-id="a948f-914">Added support for</span></span> `StandardSSD_LRS`
* <span data-ttu-id="a948f-915">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="a948f-915">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="a948f-916">[ALTERAÇÃO DA FALHA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="a948f-916">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="a948f-917">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-917">July 18, 2018</span></span>

<span data-ttu-id="a948f-918">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="a948f-918">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="a948f-919">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-919">Core</span></span>

* <span data-ttu-id="a948f-920">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="a948f-920">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="a948f-921">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="a948f-921">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="a948f-922">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="a948f-922">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-923">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-923">ACR</span></span>

* <span data-ttu-id="a948f-924">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="a948f-924">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="a948f-925">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="a948f-925">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="a948f-926">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="a948f-926">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="a948f-927">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-927">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-928">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-928">ACS</span></span>

* <span data-ttu-id="a948f-929">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="a948f-929">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-930">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-930">AppService</span></span>

* <span data-ttu-id="a948f-931">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="a948f-931">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-932">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-932">Batch</span></span>

* <span data-ttu-id="a948f-933">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a948f-933">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="a948f-934">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-934">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a948f-935">Lote AI</span><span class="sxs-lookup"><span data-stu-id="a948f-935">Batch AI</span></span>

* <span data-ttu-id="a948f-936">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="a948f-936">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="a948f-937">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-937">Container</span></span>

* <span data-ttu-id="a948f-938">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="a948f-938">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="a948f-939">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="a948f-939">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="a948f-940">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-940">Network</span></span>

* <span data-ttu-id="a948f-941">Adicionado suporte `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-941">Added `--no-wait` support to</span></span> `network nic [create|update|delete]` 
* <span data-ttu-id="a948f-942">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-942">Added</span></span> `network nic wait`
* <span data-ttu-id="a948f-943">Preterido argumento `--ids` para</span><span class="sxs-lookup"><span data-stu-id="a948f-943">Deprecated `--ids` argument for</span></span> `network vnet [subnet|peering] list`
* <span data-ttu-id="a948f-944">Adicionado sinalizador `--include-default` para incluir regras de segurança padrão na saída do</span><span class="sxs-lookup"><span data-stu-id="a948f-944">Added `--include-default` flag to include default security rules in the output of</span></span> `network nsg rule list`  

### <a name="resource"></a><span data-ttu-id="a948f-945">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-945">Resource</span></span>

* <span data-ttu-id="a948f-946">Adicionado suporte `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-946">Added `--no-wait` support to</span></span> `group deployment delete`
* <span data-ttu-id="a948f-947">Adicionado suporte `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-947">Added `--no-wait` support to</span></span> `deployment delete`
* <span data-ttu-id="a948f-948">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="a948f-948">Added `deployment wait` command</span></span>
* <span data-ttu-id="a948f-949">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="a948f-949">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-950">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-950">SQL</span></span>

* <span data-ttu-id="a948f-951">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="a948f-951">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="a948f-952">Permitir a configuração do padrão do SQL Server, executando</span><span class="sxs-lookup"><span data-stu-id="a948f-952">Allow configuring default sql server by executing</span></span> `az configure --defaults sql-server=<name>`
* <span data-ttu-id="a948f-953">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="a948f-953">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-954">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-954">Storage</span></span>

* <span data-ttu-id="a948f-955">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="a948f-955">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-956">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-956">VM</span></span>

* <span data-ttu-id="a948f-957">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-957">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="a948f-958">Adicionado suporte `--no-wait` a `vm extension [set|delete]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-958">Added `--no-wait` support to `vm extension [set|delete]` and</span></span> `vmss extension [set|delete]`
* <span data-ttu-id="a948f-959">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-959">Added</span></span> `vm extension wait`

## <a name="july-3-2018"></a><span data-ttu-id="a948f-960">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-960">July 3, 2018</span></span>

<span data-ttu-id="a948f-961">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="a948f-961">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="a948f-962">AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-962">AKS</span></span>

* <span data-ttu-id="a948f-963">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-963">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="a948f-964">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-964">July 3, 2018</span></span>

<span data-ttu-id="a948f-965">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="a948f-965">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="a948f-966">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-966">Core</span></span>

* <span data-ttu-id="a948f-967">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-967">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-968">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-968">ACR</span></span>

* <span data-ttu-id="a948f-969">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="a948f-969">Added polling build status</span></span>
* <span data-ttu-id="a948f-970">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-970">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="a948f-971">Parâmetros `--top` e `--orderby` adicionados para</span><span class="sxs-lookup"><span data-stu-id="a948f-971">Added `--top` and `--orderby` parameters for</span></span> `show-manifests`

### <a name="acs"></a><span data-ttu-id="a948f-972">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-972">ACS</span></span>

* <span data-ttu-id="a948f-973">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-973">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="a948f-974">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="a948f-974">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="a948f-975">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="a948f-975">Updated options for `aks browse` command.</span></span> <span data-ttu-id="a948f-976">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="a948f-976">Added `--listen-port` support</span></span>
* <span data-ttu-id="a948f-977">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="a948f-977">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="a948f-978">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="a948f-978">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="a948f-979">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="a948f-979">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-980">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-980">AppService</span></span>

* <span data-ttu-id="a948f-981">Suporte adicionado para desabilitar a identidade via</span><span class="sxs-lookup"><span data-stu-id="a948f-981">Added support for disabling identity via</span></span> `webapp identity remove`
* <span data-ttu-id="a948f-982">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="a948f-982">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="a948f-983">Backup</span><span class="sxs-lookup"><span data-stu-id="a948f-983">Backup</span></span>

* <span data-ttu-id="a948f-984">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="a948f-984">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="a948f-985">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a948f-985">BatchAI</span></span>

* <span data-ttu-id="a948f-986">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="a948f-986">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="a948f-987">Nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-987">Cloud</span></span>

* <span data-ttu-id="a948f-988">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-988">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="a948f-989">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-989">Container</span></span>

* <span data-ttu-id="a948f-990">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="a948f-990">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="a948f-991">Adicionados parâmetros do Log Analytics `--log-analytics-workspace` e</span><span class="sxs-lookup"><span data-stu-id="a948f-991">Added Log Analytics parameters `--log-analytics-workspace` and</span></span> `--log-analytics-workspace-key`
* <span data-ttu-id="a948f-992">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="a948f-992">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-993">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-993">Extension</span></span>

* <span data-ttu-id="a948f-994">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="a948f-994">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="a948f-995">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-995">Network</span></span>

* <span data-ttu-id="a948f-996">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="a948f-996">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-997">Rdbms</span><span class="sxs-lookup"><span data-stu-id="a948f-997">Rdbms</span></span>

* <span data-ttu-id="a948f-998">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a948f-998">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-999">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-999">Resource</span></span>

* <span data-ttu-id="a948f-1000">Novo grupo de operação adicionado</span><span class="sxs-lookup"><span data-stu-id="a948f-1000">Added new operation group</span></span> `deployment`

### <a name="vm"></a><span data-ttu-id="a948f-1001">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1001">VM</span></span>

* <span data-ttu-id="a948f-1002">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="a948f-1002">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="a948f-1003">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1003">June 25, 2018</span></span>

<span data-ttu-id="a948f-1004">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="a948f-1004">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="a948f-1005">CLI</span><span class="sxs-lookup"><span data-stu-id="a948f-1005">CLI</span></span>

* <span data-ttu-id="a948f-1006">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1006">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="a948f-1007">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1007">June 19, 2018</span></span>

<span data-ttu-id="a948f-1008">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="a948f-1008">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1009">Core</span></span>

* <span data-ttu-id="a948f-1010">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1010">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1011">ACR</span></span>

* <span data-ttu-id="a948f-1012">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="a948f-1012">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="a948f-1013">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="a948f-1013">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1014">ACS</span></span>

* <span data-ttu-id="a948f-1015">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="a948f-1015">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="a948f-1016">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="a948f-1016">Added `--update` support</span></span>
* <span data-ttu-id="a948f-1017">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em</span><span class="sxs-lookup"><span data-stu-id="a948f-1017">Changed `aks get-credentials --admin` to not eplace the user context in</span></span> `$HOME/.kube/config`
* <span data-ttu-id="a948f-1018">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="a948f-1018">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="a948f-1019">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="a948f-1019">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="a948f-1020">`--connector-name` tornou-se opcional para `aks install-connector`, `aks upgrade-connector` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1020">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and</span></span> `aks remove-connector`
* <span data-ttu-id="a948f-1021">Novas regiões de Instância de Contêiner do Azure foram adicionadas para</span><span class="sxs-lookup"><span data-stu-id="a948f-1021">Added new Azure Container Instance regions for</span></span> `aks install-connector`
* <span data-ttu-id="a948f-1022">O local normalizado no nome de versão do helm e no nome do nó foi adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1022">Added the normalized location into the helm release name and node name to</span></span> `aks install-connector`

### <a name="appservice"></a><span data-ttu-id="a948f-1023">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1023">AppService</span></span>

* <span data-ttu-id="a948f-1024">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="a948f-1024">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="a948f-1025">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="a948f-1025">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-1026">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1026">Batch</span></span>

* <span data-ttu-id="a948f-1027">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="a948f-1027">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a948f-1028">Lote AI</span><span class="sxs-lookup"><span data-stu-id="a948f-1028">Batch AI</span></span>

* <span data-ttu-id="a948f-1029">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="a948f-1029">Added support for workspaces.</span></span> <span data-ttu-id="a948f-1030">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="a948f-1030">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="a948f-1031">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="a948f-1031">Added support for experiments.</span></span> <span data-ttu-id="a948f-1032">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="a948f-1032">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="a948f-1033">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="a948f-1033">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="a948f-1034">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1034">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="a948f-1035">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="a948f-1035">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="a948f-1036">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="a948f-1036">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="a948f-1037">[ALTERAÇÃO CRÍTICA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="a948f-1037">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="a948f-1038">[ALTERAÇÃO CRÍTICA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="a948f-1038">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="a948f-1039">[ALTERAÇÃO CRÍTICA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1039">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="a948f-1040">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="a948f-1040">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="a948f-1041">[ALTERAÇÃO CRÍTICA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1041">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="a948f-1042">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="a948f-1042">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="a948f-1043">[ALTERAÇÃO CRÍTICA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="a948f-1043">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="a948f-1044">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="a948f-1044">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="a948f-1045">[ALTERAÇÃO CRÍTICA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1045">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="a948f-1046">[ALTERAÇÃO CRÍTICA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="a948f-1046">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="a948f-1047">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="a948f-1047">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="a948f-1048">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a948f-1048">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a948f-1049">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="a948f-1049">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="a948f-1050">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="a948f-1050">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="a948f-1051">Mapas</span><span class="sxs-lookup"><span data-stu-id="a948f-1051">Maps</span></span>

* <span data-ttu-id="a948f-1052">[ALTERAÇÃO CRÍTICA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="a948f-1052">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1053">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1053">Network</span></span>

* <span data-ttu-id="a948f-1054">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="a948f-1054">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="a948f-1055">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a948f-1055">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="a948f-1056">#6502</span><span class="sxs-lookup"><span data-stu-id="a948f-1056">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="a948f-1057">Reservas</span><span class="sxs-lookup"><span data-stu-id="a948f-1057">Reservations</span></span>

* <span data-ttu-id="a948f-1058">[ALTERAÇÃO DA FALHA] Adicionado parâmetro `ReservedResourceType` necessário a</span><span class="sxs-lookup"><span data-stu-id="a948f-1058">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to</span></span> `reservations catalog show`
* <span data-ttu-id="a948f-1059">Parâmetro `Location` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1059">Added parameter `Location`to</span></span> `reservations catalog show`
* <span data-ttu-id="a948f-1060">[ALTERAÇÃO DA FALHA] Removido `kind` de</span><span class="sxs-lookup"><span data-stu-id="a948f-1060">[BREAKING CHANGE] Removed `kind` from</span></span> `ReservationProperties`
* <span data-ttu-id="a948f-1061">[ALTERAÇÃO DA FALHA] `capabilities` foi renomeado para `sku_properties` em</span><span class="sxs-lookup"><span data-stu-id="a948f-1061">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in</span></span> `Catalog`
* <span data-ttu-id="a948f-1062">[ALTERAÇÃO DA FALHA] As propriedades `size` e `tier` foram removidas de</span><span class="sxs-lookup"><span data-stu-id="a948f-1062">[BREAKING CHANGE] Removed `size` and `tier` properties from</span></span> `Catalog`
* <span data-ttu-id="a948f-1063">Parâmetro `InstanceFlexibility` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1063">Added parameter `InstanceFlexibility` to</span></span> `reservations reservation update`

### <a name="role"></a><span data-ttu-id="a948f-1064">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1064">Role</span></span>

* <span data-ttu-id="a948f-1065">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="a948f-1065">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1066">SQL</span></span>

* <span data-ttu-id="a948f-1067">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-1067">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1068">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1068">Storage</span></span>

* <span data-ttu-id="a948f-1069">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="a948f-1069">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1070">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1070">VM</span></span>

* <span data-ttu-id="a948f-1071">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em</span><span class="sxs-lookup"><span data-stu-id="a948f-1071">Improved refine vm size check for accelerated networking support in</span></span> `vm create`
* <span data-ttu-id="a948f-1072">Adicionado aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para</span><span class="sxs-lookup"><span data-stu-id="a948f-1072">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to</span></span> `Standard_DS1_v2`
* <span data-ttu-id="a948f-1073">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="a948f-1073">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a948f-1074">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1074">June 13, 2018</span></span>

<span data-ttu-id="a948f-1075">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="a948f-1075">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1076">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1076">Core</span></span>

* <span data-ttu-id="a948f-1077">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="a948f-1077">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="a948f-1078">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1078">June 13, 2018</span></span>

<span data-ttu-id="a948f-1079">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="a948f-1079">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="a948f-1080">AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-1080">AKS</span></span>

* <span data-ttu-id="a948f-1081">Adicionadas opções de rede avançada a</span><span class="sxs-lookup"><span data-stu-id="a948f-1081">Added advanced networking options to</span></span> `aks create`
* <span data-ttu-id="a948f-1082">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="a948f-1082">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="a948f-1083">Adicionado argumento `--no-ssh-key` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1083">Added `--no-ssh-key` argument to</span></span> `aks create`
* <span data-ttu-id="a948f-1084">Adicionado argumento `--enable-rbac` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1084">Added `--enable-rbac` argument to</span></span> `aks create`
* <span data-ttu-id="a948f-1085">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory a</span><span class="sxs-lookup"><span data-stu-id="a948f-1085">[PREVIEW] Added support for Azure Active Directory authentication to</span></span> `aks create`

### <a name="appservice"></a><span data-ttu-id="a948f-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1086">AppService</span></span>

* <span data-ttu-id="a948f-1087">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="a948f-1087">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a948f-1088">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1088">June 5, 2018</span></span>

<span data-ttu-id="a948f-1089">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="a948f-1089">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1090">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1090">Interactive</span></span>

* <span data-ttu-id="a948f-1091">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1091">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="a948f-1092">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1092">June 5, 2018</span></span>

<span data-ttu-id="a948f-1093">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="a948f-1093">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1094">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1094">Core</span></span>

* <span data-ttu-id="a948f-1095">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="a948f-1095">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="a948f-1096">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="a948f-1096">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1097">ACR</span></span>

* <span data-ttu-id="a948f-1098">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="a948f-1098">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="a948f-1099">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="a948f-1099">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="a948f-1100">AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-1100">AKS</span></span>

* <span data-ttu-id="a948f-1101">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="a948f-1101">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-1102">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1102">Batch</span></span>

* <span data-ttu-id="a948f-1103">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="a948f-1103">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-1104">IOT</span><span class="sxs-lookup"><span data-stu-id="a948f-1104">IOT</span></span>

* <span data-ttu-id="a948f-1105">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="a948f-1105">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1106">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1106">Network</span></span>

* <span data-ttu-id="a948f-1107">Melhoria de</span><span class="sxs-lookup"><span data-stu-id="a948f-1107">Improved</span></span> `network vnet peering`

### <a name="policy-insights"></a><span data-ttu-id="a948f-1108">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="a948f-1108">Policy Insights</span></span>

* <span data-ttu-id="a948f-1109">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1109">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="a948f-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="a948f-1110">ARM</span></span>

* <span data-ttu-id="a948f-1111">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="a948f-1111">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1112">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1112">SQL</span></span>

* <span data-ttu-id="a948f-1113">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="a948f-1113">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="a948f-1114">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="a948f-1114">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="a948f-1115">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1115">Storage</span></span>

* <span data-ttu-id="a948f-1116">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="a948f-1116">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1117">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1117">VM</span></span>

* <span data-ttu-id="a948f-1118">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="a948f-1118">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="a948f-1119">Adição da opção `--accelerated-networking` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1119">Added `--accelerated-networking` option to</span></span> `vm create`
* <span data-ttu-id="a948f-1120">`--tags` foi adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1120">Added `--tags` to</span></span> `identity create`

## <a name="may-22-2018"></a><span data-ttu-id="a948f-1121">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1121">May 22, 2018</span></span>

<span data-ttu-id="a948f-1122">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="a948f-1122">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1123">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1123">Core</span></span>

* <span data-ttu-id="a948f-1124">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1124">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1125">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1125">ACS</span></span>

* <span data-ttu-id="a948f-1126">Adicionados novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1126">Added new Dev-Spaces commands `aks use-dev-spaces` and</span></span> `aks remove-dev-spaces`
* <span data-ttu-id="a948f-1127">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="a948f-1127">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1128">AppService</span></span>

* <span data-ttu-id="a948f-1129">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="a948f-1129">Improved generic update commands</span></span>
* <span data-ttu-id="a948f-1130">Suporte assíncrono adicionado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1130">Added async support for</span></span> `webapp deployment source config-zip`

### <a name="container"></a><span data-ttu-id="a948f-1131">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1131">Container</span></span>

* <span data-ttu-id="a948f-1132">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="a948f-1132">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="a948f-1133">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1133">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1134">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1134">Extension</span></span>

* <span data-ttu-id="a948f-1135">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="a948f-1135">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1136">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1136">Interactive</span></span>

* <span data-ttu-id="a948f-1137">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="a948f-1137">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="a948f-1138">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="a948f-1138">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-1139">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a948f-1139">KeyVault</span></span>

* <span data-ttu-id="a948f-1140">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="a948f-1140">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1141">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1141">Network</span></span>

* <span data-ttu-id="a948f-1142">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="a948f-1142">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="a948f-1143">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="a948f-1143">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1144">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1144">SQL</span></span>

* <span data-ttu-id="a948f-1145">[ALTERAÇÃO DA FALHA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="a948f-1145">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="a948f-1146">A propriedade `serviceLevelObjective` foi renomeada para</span><span class="sxs-lookup"><span data-stu-id="a948f-1146">Renamed `serviceLevelObjective` property to</span></span> `currentServiceObjectiveName`
    * <span data-ttu-id="a948f-1147">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="a948f-1147">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="a948f-1148">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a948f-1148">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="a948f-1149">[ALTERAÇÃO DA FALHA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="a948f-1149">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * `requestedServiceObjectiveName`<span data-ttu-id="a948f-1150">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1150">.</span></span>  <span data-ttu-id="a948f-1151">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="a948f-1151">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * `edition`<span data-ttu-id="a948f-1152">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1152">.</span></span> <span data-ttu-id="a948f-1153">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="a948f-1153">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * `elasticPoolName`<span data-ttu-id="a948f-1154">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1154">.</span></span> <span data-ttu-id="a948f-1155">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="a948f-1155">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="a948f-1156">[ALTERAÇÃO DA FALHA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="a948f-1156">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * `edition`<span data-ttu-id="a948f-1157">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1157">.</span></span> <span data-ttu-id="a948f-1158">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="a948f-1158">To update, use the `--edition` parameter</span></span>
    * `dtu`<span data-ttu-id="a948f-1159">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1159">.</span></span> <span data-ttu-id="a948f-1160">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="a948f-1160">To update, use the `--capacity` parameter</span></span>
    *  `databaseDtuMin`<span data-ttu-id="a948f-1161">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1161">.</span></span> <span data-ttu-id="a948f-1162">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="a948f-1162">To update, use the `--db-min-capacity` parameter</span></span>
    *  `databaseDtuMax`<span data-ttu-id="a948f-1163">.</span><span class="sxs-lookup"><span data-stu-id="a948f-1163">.</span></span> <span data-ttu-id="a948f-1164">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="a948f-1164">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="a948f-1165">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1165">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="a948f-1166">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1166">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1167">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1167">Storage</span></span>

* <span data-ttu-id="a948f-1168">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="a948f-1168">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="a948f-1169">Corrigido problema com</span><span class="sxs-lookup"><span data-stu-id="a948f-1169">Fixed problem with</span></span> `storage entity query`

### <a name="vm"></a><span data-ttu-id="a948f-1170">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1170">VM</span></span>

* <span data-ttu-id="a948f-1171">[ALTERAÇÃO DA FALHA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1171">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="a948f-1172">O mesmo suporte pode ser acessado por meio de `vm update` ou</span><span class="sxs-lookup"><span data-stu-id="a948f-1172">The same support can be accessed through `vm update` or</span></span> `vm disk attach`
* <span data-ttu-id="a948f-1173">Corrigida correspondência de imagem de extensão em</span><span class="sxs-lookup"><span data-stu-id="a948f-1173">Fixed extension image matching in</span></span> `[vm|vmss] extension`
* <span data-ttu-id="a948f-1174">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="a948f-1174">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="a948f-1175">`--license-type` foi adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1175">Added `--license-type` to</span></span> `[vm|vmss] update`

## <a name="may-7-2018"></a><span data-ttu-id="a948f-1176">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1176">May 7, 2018</span></span>

<span data-ttu-id="a948f-1177">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="a948f-1177">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1178">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1178">Core</span></span>

* <span data-ttu-id="a948f-1179">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="a948f-1179">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="a948f-1180">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="a948f-1180">Added limited support for positional arguments</span></span>
* <span data-ttu-id="a948f-1181">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1181">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="a948f-1182">#5591</span><span class="sxs-lookup"><span data-stu-id="a948f-1182">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="a948f-1183">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1183">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="a948f-1184">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="a948f-1184">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="a948f-1185">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1185">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="a948f-1186">Erro aprimorado durante a digitação dos usuários</span><span class="sxs-lookup"><span data-stu-id="a948f-1186">Improved error when users type</span></span> `az ''`
* <span data-ttu-id="a948f-1187">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="a948f-1187">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1188">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1188">ACR</span></span>

* <span data-ttu-id="a948f-1189">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1189">Added ACR Build commands</span></span>
* <span data-ttu-id="a948f-1190">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="a948f-1190">Improved resource not found error messages</span></span>
* <span data-ttu-id="a948f-1191">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="a948f-1191">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="a948f-1192">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="a948f-1192">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="a948f-1193">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="a948f-1193">Improved repository commands error messages</span></span>
* <span data-ttu-id="a948f-1194">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="a948f-1194">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1195">ACS</span></span>

* <span data-ttu-id="a948f-1196">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-1196">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="a948f-1197">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="a948f-1197">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="a948f-1198">AMS</span><span class="sxs-lookup"><span data-stu-id="a948f-1198">AMS</span></span>

* <span data-ttu-id="a948f-1199">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-1199">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1200">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1200">Appservice</span></span>

* <span data-ttu-id="a948f-1201">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="a948f-1201">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="a948f-1202">Removido `--runtime-version` de</span><span class="sxs-lookup"><span data-stu-id="a948f-1202">Removed `--runtime-version` from</span></span> `webapp auth update`
* <span data-ttu-id="a948f-1203">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="a948f-1203">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="a948f-1204">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="a948f-1204">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="a948f-1205">Lote AI</span><span class="sxs-lookup"><span data-stu-id="a948f-1205">Batch AI</span></span>

* <span data-ttu-id="a948f-1206">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="a948f-1206">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a948f-1207">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1207">Cognitive Services</span></span>

* <span data-ttu-id="a948f-1208">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="a948f-1208">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="a948f-1209">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1209">Consumption</span></span>

* <span data-ttu-id="a948f-1210">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1210">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1211">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1211">Container</span></span>

* <span data-ttu-id="a948f-1212">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-1212">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="a948f-1213">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a948f-1213">Cosmos DB</span></span>

* <span data-ttu-id="a948f-1214">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="a948f-1214">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="a948f-1215">DMS</span><span class="sxs-lookup"><span data-stu-id="a948f-1215">DMS</span></span>

* <span data-ttu-id="a948f-1216">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-1216">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1217">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1217">Extension</span></span>

* <span data-ttu-id="a948f-1218">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="a948f-1218">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1219">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1219">Interactive</span></span>

* <span data-ttu-id="a948f-1220">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="a948f-1220">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="a948f-1221">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="a948f-1221">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="a948f-1222">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="a948f-1222">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="a948f-1223">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1223">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="a948f-1224">Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-1224">Lab</span></span>

* <span data-ttu-id="a948f-1225">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="a948f-1225">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1226">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1226">Network</span></span>

* <span data-ttu-id="a948f-1227">[ALTERAÇÃO DA FALHA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="a948f-1227">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="a948f-1228">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1228">Profile</span></span>

* <span data-ttu-id="a948f-1229">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="a948f-1229">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="a948f-1230">[ALTERAÇÃO DA FALHA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="a948f-1230">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="a948f-1231">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="a948f-1231">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="a948f-1232">Redis</span><span class="sxs-lookup"><span data-stu-id="a948f-1232">Redis</span></span>

* <span data-ttu-id="a948f-1233">`redis patch-schedule patch-schedule show` preterido em favor de</span><span class="sxs-lookup"><span data-stu-id="a948f-1233">Deprecated `redis patch-schedule patch-schedule show` in favor of</span></span> `redis patch-schedule show`
* <span data-ttu-id="a948f-1234">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="a948f-1234">Deprecated `redis list-all`.</span></span> <span data-ttu-id="a948f-1235">Esta funcionalidade foi dobrada em</span><span class="sxs-lookup"><span data-stu-id="a948f-1235">This functionality has been folded into</span></span> `redis list`
* <span data-ttu-id="a948f-1236">`redis import-method` preterido em favor de</span><span class="sxs-lookup"><span data-stu-id="a948f-1236">Deprecated `redis import-method` in favor of</span></span> `redis import`
* <span data-ttu-id="a948f-1237">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1237">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="a948f-1238">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1238">Role</span></span>

* <span data-ttu-id="a948f-1239">[ALTERAÇÃO DA FALHA] Remoção de preterido</span><span class="sxs-lookup"><span data-stu-id="a948f-1239">[BREAKING CHANGE] Removed deprecated</span></span> `ad sp reset-credentials`

### <a name="storage"></a><span data-ttu-id="a948f-1240">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1240">Storage</span></span>

* <span data-ttu-id="a948f-1241">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="a948f-1241">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="a948f-1242">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="a948f-1242">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="a948f-1243">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="a948f-1243">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="a948f-1244">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="a948f-1244">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="a948f-1245">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="a948f-1245">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1246">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1246">VM</span></span>

* <span data-ttu-id="a948f-1247">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="a948f-1247">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="a948f-1248">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="a948f-1248">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="a948f-1249">[ALTERAÇÃO DA FALHA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="a948f-1249">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="a948f-1250">Suporte adicionado para a política de remoção em</span><span class="sxs-lookup"><span data-stu-id="a948f-1250">Added support for eviction policy to</span></span> `vmss`
* <span data-ttu-id="a948f-1251">[ALTERAÇÃO DA FALHA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="a948f-1251">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="a948f-1252">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="a948f-1252">Added write accelerator support</span></span>
* <span data-ttu-id="a948f-1253">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-1253">Added</span></span> `vmss perform-maintenance`
* <span data-ttu-id="a948f-1254">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="a948f-1254">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="a948f-1255">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="a948f-1255">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="a948f-1256">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1256">April 10, 2018</span></span>

<span data-ttu-id="a948f-1257">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="a948f-1257">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1258">ACR</span></span>

* <span data-ttu-id="a948f-1259">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="a948f-1259">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1260">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1260">ACS</span></span>

* <span data-ttu-id="a948f-1261">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="a948f-1261">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1262">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1262">Appservice</span></span>

* [<span data-ttu-id="a948f-1263">ALTERAÇÃO DA FALHA</span><span class="sxs-lookup"><span data-stu-id="a948f-1263">BREAKING CHANGE</span></span>]: Removed `assign-identity`
* <span data-ttu-id="a948f-1264">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1264">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="a948f-1265">BatchAI</span><span class="sxs-lookup"><span data-stu-id="a948f-1265">BatchAI</span></span>

* <span data-ttu-id="a948f-1266">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="a948f-1266">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="a948f-1267">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="a948f-1267">Job level mounting</span></span>
  - <span data-ttu-id="a948f-1268">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="a948f-1268">Environment variables with secret values</span></span>
  - <span data-ttu-id="a948f-1269">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="a948f-1269">Performance counters settings</span></span>
  - <span data-ttu-id="a948f-1270">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="a948f-1270">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="a948f-1271">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="a948f-1271">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="a948f-1272">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="a948f-1272">Usage and limits reporting</span></span>
  - <span data-ttu-id="a948f-1273">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="a948f-1273">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="a948f-1274">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="a948f-1274">Support for custom images</span></span>
  - <span data-ttu-id="a948f-1275">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="a948f-1275">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="a948f-1276">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="a948f-1276">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="a948f-1277">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="a948f-1277">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="a948f-1278">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="a948f-1278">National clouds are supported</span></span>
* <span data-ttu-id="a948f-1279">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="a948f-1279">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="a948f-1280">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="a948f-1280">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="a948f-1281">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1281">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="a948f-1282">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="a948f-1282">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="a948f-1283">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="a948f-1283">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="a948f-1284">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="a948f-1284">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="a948f-1285">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="a948f-1285">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="a948f-1286">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="a948f-1286">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="a948f-1287">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="a948f-1287">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="a948f-1288">Adição da opção `--generate-ssh-keys` a `cluster create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1288">Added `--generate-ssh-keys` option to `cluster create` and</span></span> `file-server create`
* <span data-ttu-id="a948f-1289">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1289">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="a948f-1290">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="a948f-1290">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="a948f-1291">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1291">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="a948f-1292">Cobrança</span><span class="sxs-lookup"><span data-stu-id="a948f-1292">Billing</span></span>

* <span data-ttu-id="a948f-1293">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="a948f-1293">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="a948f-1294">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1294">Consumption</span></span>

* <span data-ttu-id="a948f-1295">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="a948f-1295">Added `marketplace` commands</span></span>
* <span data-ttu-id="a948f-1296">[ALTERAÇÃO DA FALHA] `reservations summaries` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1296">[BREAKING CHANGE] Renamed `reservations summaries` to</span></span> `reservation summary`
* <span data-ttu-id="a948f-1297">[ALTERAÇÃO DA FALHA] `reservations details` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1297">[BREAKING CHANGE] Renamed `reservations details` to</span></span> `reservation detail`
* <span data-ttu-id="a948f-1298">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="a948f-1298">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="a948f-1299">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="a948f-1299">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="a948f-1300">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="a948f-1300">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1301">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1301">Container</span></span>

* <span data-ttu-id="a948f-1302">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1302">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and</span></span> `--gitrepo-mount-path`
* <span data-ttu-id="a948f-1303">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="a948f-1303">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1304">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1304">Extension</span></span>

* <span data-ttu-id="a948f-1305">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="a948f-1305">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1306">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1306">Interactive</span></span>

* <span data-ttu-id="a948f-1307">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="a948f-1307">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="a948f-1308">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1308">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="a948f-1309">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="a948f-1309">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1310">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1310">Network</span></span>

* <span data-ttu-id="a948f-1311">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="a948f-1311">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="a948f-1312">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1312">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="a948f-1313">#4910</span><span class="sxs-lookup"><span data-stu-id="a948f-1313">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="a948f-1314">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="a948f-1314">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="a948f-1315">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="a948f-1315">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="a948f-1316">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em</span><span class="sxs-lookup"><span data-stu-id="a948f-1316">Fixed issue with `--disable-bgp-route-propagation` flag in</span></span> `network route-table [create|update]`
* <span data-ttu-id="a948f-1317">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para</span><span class="sxs-lookup"><span data-stu-id="a948f-1317">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for</span></span> `network lb [create|update]`
* <span data-ttu-id="a948f-1318">Adição de suporte para registros TXT com sequências de escape RFC 1035 a `network dns zone [import|export]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1318">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and</span></span> `network dns record-set txt add-record`

### <a name="profile"></a><span data-ttu-id="a948f-1319">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1319">Profile</span></span>

* <span data-ttu-id="a948f-1320">Adição de suporte para contas clássicas do Azure em</span><span class="sxs-lookup"><span data-stu-id="a948f-1320">Added support for Azure Classic accounts in</span></span> `account list`
* <span data-ttu-id="a948f-1321">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="a948f-1321">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-1322">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-1322">RDBMS</span></span>

* <span data-ttu-id="a948f-1323">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="a948f-1323">Added `georestore` command</span></span>
* <span data-ttu-id="a948f-1324">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1324">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1325">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1325">Resource</span></span>

* <span data-ttu-id="a948f-1326">Adição do suporte para `--metadata` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1326">Added support for `--metadata` to</span></span> `policy definition create`
* <span data-ttu-id="a948f-1327">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1327">Added support for `--metadata`, `--set`, `--add`, `--remove` to</span></span> `policy definition update`

### <a name="sql"></a><span data-ttu-id="a948f-1328">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1328">SQL</span></span>

* <span data-ttu-id="a948f-1329">Adição de `sql elastic-pool op list` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1329">Added `sql elastic-pool op list` and</span></span> `sql elastic-pool op cancel`

### <a name="storage"></a><span data-ttu-id="a948f-1330">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1330">Storage</span></span>

* <span data-ttu-id="a948f-1331">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="a948f-1331">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1332">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1332">VM</span></span>

* <span data-ttu-id="a948f-1333">Adição de suporte para configurar a contagem de domínios de falha da plataforma a</span><span class="sxs-lookup"><span data-stu-id="a948f-1333">Added support to configure platform fault domain count to</span></span> `vmss create`
* <span data-ttu-id="a948f-1334">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1334">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [<span data-ttu-id="a948f-1335">ALTERAÇÃO DA FALHA</span><span class="sxs-lookup"><span data-stu-id="a948f-1335">BREAKING CHANGE</span></span>]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="a948f-1336">Adição de suporte para a SKU de IP público a</span><span class="sxs-lookup"><span data-stu-id="a948f-1336">Added support for Public-IP SKU to</span></span> `vm create`
* <span data-ttu-id="a948f-1337">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="a948f-1337">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="a948f-1338">#5718</span><span class="sxs-lookup"><span data-stu-id="a948f-1338">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="a948f-1339">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="a948f-1339">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="a948f-1340">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1340">March 27, 2018</span></span>

<span data-ttu-id="a948f-1341">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="a948f-1341">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1342">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1342">Core</span></span>

* <span data-ttu-id="a948f-1343">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="a948f-1343">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1344">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1344">ACS</span></span>

* <span data-ttu-id="a948f-1345">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a948f-1345">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1346">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1346">Appservice</span></span>

* <span data-ttu-id="a948f-1347">Adição de suporte somente para HTTPS a</span><span class="sxs-lookup"><span data-stu-id="a948f-1347">Added HTTPS-only support to</span></span> `webapp update`
* <span data-ttu-id="a948f-1348">Adição de suporte para os slots a `az webapp identity [assign|show]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1348">Added support for slots to `az webapp identity [assign|show]` and</span></span> `az functionapp identity [assign|show]`

### <a name="backup"></a><span data-ttu-id="a948f-1349">Backup</span><span class="sxs-lookup"><span data-stu-id="a948f-1349">Backup</span></span>

* <span data-ttu-id="a948f-1350">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1350">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="a948f-1351">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-1351">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="a948f-1352">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="a948f-1352">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="a948f-1353">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="a948f-1353">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1354">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1354">Container</span></span>

* <span data-ttu-id="a948f-1355">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="a948f-1355">Added `container exec` command.</span></span> <span data-ttu-id="a948f-1356">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="a948f-1356">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="a948f-1357">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1357">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1358">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1358">Extension</span></span>

* <span data-ttu-id="a948f-1359">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-1359">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="a948f-1360">`extension list-available` alterado para mostrar dados de extensão total com</span><span class="sxs-lookup"><span data-stu-id="a948f-1360">Changed `extension list-available` to show full extension data with</span></span> `--show-details`
* <span data-ttu-id="a948f-1361">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-1361">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1362">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1362">Interactive</span></span>

* <span data-ttu-id="a948f-1363">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1363">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="a948f-1364">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="a948f-1364">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="a948f-1365">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1365">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="a948f-1366">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="a948f-1366">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="a948f-1367">Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-1367">Lab</span></span>

* <span data-ttu-id="a948f-1368">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="a948f-1368">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1369">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1369">Monitor</span></span>

* <span data-ttu-id="a948f-1370">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a948f-1370">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="a948f-1371">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="a948f-1371">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="a948f-1372">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="a948f-1372">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1373">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1373">Network</span></span>

* <span data-ttu-id="a948f-1374">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="a948f-1374">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="a948f-1375">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1375">Profile</span></span>

* <span data-ttu-id="a948f-1376">Adição de avisos para `--identity-port` e `--msi-port` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1376">Added warning for `--identity-port` and `--msi-port` to</span></span> `login`

### <a name="rdbms"></a><span data-ttu-id="a948f-1377">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-1377">RDBMS</span></span>

* <span data-ttu-id="a948f-1378">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a948f-1378">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1379">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1379">Resource</span></span>

* [<span data-ttu-id="a948f-1380">ALTERAÇÃO DA FALHA</span><span class="sxs-lookup"><span data-stu-id="a948f-1380">BREAKING CHANGE</span></span>]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="a948f-1381">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1381">Role</span></span>

* <span data-ttu-id="a948f-1382">Adição de suporte para configurações de acesso necessário e clientes nativos a</span><span class="sxs-lookup"><span data-stu-id="a948f-1382">Added support for required access configurations and native clients to</span></span> `az ad app create`
* <span data-ttu-id="a948f-1383">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="a948f-1383">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="a948f-1384">Adição de comandos de gerenciamento de credencial</span><span class="sxs-lookup"><span data-stu-id="a948f-1384">Added credential management commands</span></span> `ad sp credential [reset|list|delete]`
* <span data-ttu-id="a948f-1385">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="a948f-1385">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="a948f-1386">Adição de suporte para as permissões `dataActions` e `notDataActions` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1386">Added support for `dataActions` and `notDataActions` permissions to</span></span> `role definition`

### <a name="storage"></a><span data-ttu-id="a948f-1387">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1387">Storage</span></span>

* <span data-ttu-id="a948f-1388">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="a948f-1388">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="a948f-1389">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="a948f-1389">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1390">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1390">VM</span></span>

* <span data-ttu-id="a948f-1391">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="a948f-1391">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="a948f-1392">Adição de suporte com flexibilidade de zona a</span><span class="sxs-lookup"><span data-stu-id="a948f-1392">Added zone resilient support to</span></span> `vm [snapshot|image]`
* <span data-ttu-id="a948f-1393">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="a948f-1393">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="a948f-1394">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="a948f-1394">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="a948f-1395">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1395">March 13, 2018</span></span>

<span data-ttu-id="a948f-1396">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="a948f-1396">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1397">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1397">ACR</span></span>

* <span data-ttu-id="a948f-1398">Suporte adicionado para o parâmetro `--image` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1398">Added support for `--image` parameter to</span></span> `repository delete`
* <span data-ttu-id="a948f-1399">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="a948f-1399">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="a948f-1400">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="a948f-1400">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1401">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1401">ACS</span></span>

* <span data-ttu-id="a948f-1402">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="a948f-1402">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="a948f-1403">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="a948f-1403">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="a948f-1404">Supervisor</span><span class="sxs-lookup"><span data-stu-id="a948f-1404">Advisor</span></span>

* <span data-ttu-id="a948f-1405">[ALTERAÇÃO DA FALHA] `advisor configuration get` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1405">[BREAKING CHANGE] Renamed `advisor configuration get` to</span></span> `advisor configuration list`
* <span data-ttu-id="a948f-1406">[ALTERAÇÃO DA FALHA] `advisor configuration set` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1406">[BREAKING CHANGE] Renamed `advisor configuration set` to</span></span> `advisor configuration update`
* <span data-ttu-id="a948f-1407">[ALTERAÇÃO DA FALHA] Removido</span><span class="sxs-lookup"><span data-stu-id="a948f-1407">[BREAKING CHANGE] Removed</span></span> `advisor recommendation generate`
* <span data-ttu-id="a948f-1408">Parâmetro `--refresh` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1408">Added `--refresh` parameter to</span></span> `advisor recommendation list`
* <span data-ttu-id="a948f-1409">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="a948f-1409">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1410">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1410">Appservice</span></span>

* <span data-ttu-id="a948f-1411">Preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-1411">Deprecated</span></span> `[webapp|functionapp] assign-identity`
* <span data-ttu-id="a948f-1412">Adicionados comandos de identidade gerenciada `webapp identity [assign|show]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1412">Added managed identity commands `webapp identity [assign|show]` and</span></span> `functionapp identity [assign|show]`

### <a name="eventhubs"></a><span data-ttu-id="a948f-1413">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-1413">Eventhubs</span></span>

* <span data-ttu-id="a948f-1414">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1414">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1415">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1415">Extension</span></span>

* <span data-ttu-id="a948f-1416">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="a948f-1416">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1417">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1417">Interactive</span></span>

* <span data-ttu-id="a948f-1418">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1418">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="a948f-1419">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="a948f-1419">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="a948f-1420">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="a948f-1420">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="a948f-1421">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="a948f-1421">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1422">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1422">Monitor</span></span>

* <span data-ttu-id="a948f-1423">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-1423">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="a948f-1424">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="a948f-1424">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="a948f-1425">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="a948f-1425">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="a948f-1426">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="a948f-1426">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1427">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1427">Network</span></span>

* <span data-ttu-id="a948f-1428">[ALTERAÇÃO DA FALHA] Parâmetro `--tags` removido de</span><span class="sxs-lookup"><span data-stu-id="a948f-1428">[BREAKING CHANGE] Removed `--tags` parameter from</span></span>  `route-filter rule create`
* <span data-ttu-id="a948f-1429">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="a948f-1429">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="a948f-1430">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1430">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="a948f-1431">Parâmetros `--vnet` e `--subnet` adicionados a</span><span class="sxs-lookup"><span data-stu-id="a948f-1431">Added `--vnet` and `--subnet` parameters to</span></span> `network watcher show-topology`

### <a name="profile"></a><span data-ttu-id="a948f-1432">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1432">Profile</span></span>

* <span data-ttu-id="a948f-1433">Parâmetro `--msi` preterido de</span><span class="sxs-lookup"><span data-stu-id="a948f-1433">Deprecated `--msi` parameter for</span></span> `az login`
* <span data-ttu-id="a948f-1434">Parâmetro `--identity` adicionado de `az login` para substituir</span><span class="sxs-lookup"><span data-stu-id="a948f-1434">Added `--identity` parameter for `az login` to replace</span></span> `--msi`

### <a name="rdbms"></a><span data-ttu-id="a948f-1435">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-1435">RDBMS</span></span>

* <span data-ttu-id="a948f-1436">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="a948f-1436">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="a948f-1437">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-1437">Service Bus</span></span>

* <span data-ttu-id="a948f-1438">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1438">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1439">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1439">Storage</span></span>

* <span data-ttu-id="a948f-1440">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-1440">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="a948f-1441">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="a948f-1441">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1442">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1442">VM</span></span>

* <span data-ttu-id="a948f-1443">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="a948f-1443">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="a948f-1444">Preteridos `[vm|vmss] assign-identity` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1444">Deprecated `[vm|vmss] assign-identity` and</span></span> `[vm|vmss] remove-identity`
* <span data-ttu-id="a948f-1445">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="a948f-1445">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="a948f-1446">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="a948f-1446">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="a948f-1447">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1447">February 27, 2018</span></span>

<span data-ttu-id="a948f-1448">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="a948f-1448">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1449">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1449">Core</span></span>

* <span data-ttu-id="a948f-1450">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="a948f-1450">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="a948f-1451">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="a948f-1451">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="a948f-1452">Adição de log HTTP a</span><span class="sxs-lookup"><span data-stu-id="a948f-1452">Added HTTP logging to</span></span> `--debug`

### <a name="acs"></a><span data-ttu-id="a948f-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1453">ACS</span></span>

* <span data-ttu-id="a948f-1454">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-1454">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="a948f-1455">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="a948f-1455">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="a948f-1456">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao</span><span class="sxs-lookup"><span data-stu-id="a948f-1456">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to</span></span> `aks install-connector`
* <span data-ttu-id="a948f-1457">Remoção do aviso de reprovação de</span><span class="sxs-lookup"><span data-stu-id="a948f-1457">Removed deprecation notice from</span></span> `aks get-versions`

### <a name="appservice"></a><span data-ttu-id="a948f-1458">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1458">Appservice</span></span>

* <span data-ttu-id="a948f-1459">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="a948f-1459">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="a948f-1460">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="a948f-1460">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="a948f-1461">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1461">Cognitive Services</span></span>

* <span data-ttu-id="a948f-1462">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1462">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="a948f-1463">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1463">Consumption</span></span>

* <span data-ttu-id="a948f-1464">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="a948f-1464">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="a948f-1465">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="a948f-1465">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1466">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1466">Container</span></span>

* <span data-ttu-id="a948f-1467">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="a948f-1467">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1468">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1468">Network</span></span>

* <span data-ttu-id="a948f-1469">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): Cliente ausente em</span><span class="sxs-lookup"><span data-stu-id="a948f-1469">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in</span></span> `network vnet-gateway vpn-client generate`

### <a name="resource"></a><span data-ttu-id="a948f-1470">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1470">Resource</span></span>

* <span data-ttu-id="a948f-1471">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="a948f-1471">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="a948f-1472">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1472">Role</span></span>

* <span data-ttu-id="a948f-1473">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-1473">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1474">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1474">SQL</span></span>

* <span data-ttu-id="a948f-1475">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="a948f-1475">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1476">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1476">Storage</span></span>

* <span data-ttu-id="a948f-1477">Habilitação de especificação de caminho de destino/prefixo do</span><span class="sxs-lookup"><span data-stu-id="a948f-1477">Enabled specifying destination-path/prefix for</span></span> `storage blob [upload-batch|download-batch]`

### <a name="vm"></a><span data-ttu-id="a948f-1478">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1478">VM</span></span>

* <span data-ttu-id="a948f-1479">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="a948f-1479">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="a948f-1480">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1480">February 13, 2018</span></span>

<span data-ttu-id="a948f-1481">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="a948f-1481">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1482">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1482">Core</span></span>

* <span data-ttu-id="a948f-1483">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="a948f-1483">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1484">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1484">ACS</span></span>

* <span data-ttu-id="a948f-1485">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="a948f-1485">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="a948f-1486">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para</span><span class="sxs-lookup"><span data-stu-id="a948f-1486">Changed `aks get-versions` to show Kubernetes versions available for</span></span> `aks create`
* <span data-ttu-id="a948f-1487">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a948f-1487">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="a948f-1488">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-1488">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="a948f-1489">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="a948f-1489">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="a948f-1490">Aumentada a confiabilidade ao localizar o pod de painel para</span><span class="sxs-lookup"><span data-stu-id="a948f-1490">Improved reliability when locating the dashboard pod for</span></span> `az aks browse`
* <span data-ttu-id="a948f-1491">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="a948f-1491">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="a948f-1492">Adicionada uma mensagem a `az aks install-cli` para ajudar a obter `kubectl` em</span><span class="sxs-lookup"><span data-stu-id="a948f-1492">Added a message to `az aks install-cli` to help get `kubectl` in</span></span> `$PATH`

### <a name="appservice"></a><span data-ttu-id="a948f-1493">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1493">Appservice</span></span>

* <span data-ttu-id="a948f-1494">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="a948f-1494">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="a948f-1495">Adicionado suporte para planos de serviço de aplicativo padrão por meio de</span><span class="sxs-lookup"><span data-stu-id="a948f-1495">Added support for default app service plans through</span></span> `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a><span data-ttu-id="a948f-1496">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-1496">CDN</span></span>

* <span data-ttu-id="a948f-1497">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="a948f-1497">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1498">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1498">Container</span></span>

* <span data-ttu-id="a948f-1499">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="a948f-1499">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="a948f-1500">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1500">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-1501">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-1501">CosmosDB</span></span>

* <span data-ttu-id="a948f-1502">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="a948f-1502">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1503">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1503">Extension</span></span>

* <span data-ttu-id="a948f-1504">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a948f-1504">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="a948f-1505">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="a948f-1505">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="a948f-1506">Comentários</span><span class="sxs-lookup"><span data-stu-id="a948f-1506">Feedback</span></span>

* <span data-ttu-id="a948f-1507">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="a948f-1507">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1508">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1508">Interactive</span></span>

* <span data-ttu-id="a948f-1509">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="a948f-1509">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="a948f-1510">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1510">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-1511">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-1511">IoT</span></span>

* <span data-ttu-id="a948f-1512">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="a948f-1512">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a948f-1513">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="a948f-1513">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="a948f-1514">Adicionado suporte `--no-wait` a `iot dps access policy [create|update]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1514">Added `--no-wait` support to `iot dps access policy [create|update]` and</span></span> `iot dps linked-hub [create|update]`
* <span data-ttu-id="a948f-1515">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="a948f-1515">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1516">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1516">Monitor</span></span>

* <span data-ttu-id="a948f-1517">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1517">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1518">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1518">Network</span></span>

* <span data-ttu-id="a948f-1519">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="a948f-1519">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="a948f-1520">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1520">Profile</span></span>

* <span data-ttu-id="a948f-1521">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1521">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1522">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1522">Resource</span></span>

* <span data-ttu-id="a948f-1523">Adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="a948f-1523">Added back</span></span> `feature show`

### <a name="role"></a><span data-ttu-id="a948f-1524">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1524">Role</span></span>

* <span data-ttu-id="a948f-1525">Adicionado argumento `--available-to-other-tenants` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1525">Added `--available-to-other-tenants` argument to</span></span> `ad app update`

### <a name="sql"></a><span data-ttu-id="a948f-1526">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1526">SQL</span></span>

* <span data-ttu-id="a948f-1527">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="a948f-1527">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="a948f-1528">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-1528">Added</span></span> `sql db rename`
* <span data-ttu-id="a948f-1529">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="a948f-1529">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1530">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1530">Storage</span></span>

* <span data-ttu-id="a948f-1531">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="a948f-1531">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1532">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1532">VM</span></span>

* <span data-ttu-id="a948f-1533">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="a948f-1533">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="a948f-1534">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="a948f-1534">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="a948f-1535">Correção</span><span class="sxs-lookup"><span data-stu-id="a948f-1535">Fixed</span></span> `vm boot-diagnostics get-boot-log`


## <a name="january-31-2018"></a><span data-ttu-id="a948f-1536">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1536">January 31, 2018</span></span>

<span data-ttu-id="a948f-1537">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="a948f-1537">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1538">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1538">Core</span></span>

* <span data-ttu-id="a948f-1539">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="a948f-1539">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="a948f-1540">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="a948f-1540">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="a948f-1541">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="a948f-1541">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="a948f-1542">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="a948f-1542">Use `--verbose` to see</span></span>
* <span data-ttu-id="a948f-1543">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="a948f-1543">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1544">ACS</span></span>

* <span data-ttu-id="a948f-1545">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="a948f-1545">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="a948f-1546">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="a948f-1546">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1547">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1547">Appservice</span></span>

* <span data-ttu-id="a948f-1548">Correção</span><span class="sxs-lookup"><span data-stu-id="a948f-1548">Fixed</span></span> `webapp log [tail|download]`
* <span data-ttu-id="a948f-1549">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="a948f-1549">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="a948f-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-1550">CDN</span></span>

* <span data-ttu-id="a948f-1551">Corrigido o problema de cliente ausente com</span><span class="sxs-lookup"><span data-stu-id="a948f-1551">Fixed missing client issue with</span></span> `cdn custom-domain create`

### <a name="cosmosdb"></a><span data-ttu-id="a948f-1552">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-1552">CosmosDB</span></span>

* <span data-ttu-id="a948f-1553">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="a948f-1553">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1554">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1554">Interactive</span></span>

* <span data-ttu-id="a948f-1555">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="a948f-1555">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1556">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1556">Network</span></span>

* <span data-ttu-id="a948f-1557">Adicionada proteção para `--cert-password` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1557">Added protection for `--cert-password` to</span></span> `application-gateway create`
* <span data-ttu-id="a948f-1558">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="a948f-1558">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="a948f-1559">Adicionada proteção para `--shared-key` e `--authorization-key` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1559">Added protection for `--shared-key` and `--authorization-key` to</span></span> `vpn-connection create`
* <span data-ttu-id="a948f-1560">Corrigido o problema de cliente ausente com</span><span class="sxs-lookup"><span data-stu-id="a948f-1560">Fixed missing client issue with</span></span> `asg create`
* <span data-ttu-id="a948f-1561">Adicionado parâmetro `--file-name / -f` para nomes exportados a</span><span class="sxs-lookup"><span data-stu-id="a948f-1561">Added `--file-name / -f` parameter for exported names to</span></span> `dns zone export`
* <span data-ttu-id="a948f-1562">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="a948f-1562">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="a948f-1563">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-1563">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="a948f-1564">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="a948f-1564">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="a948f-1565">Corrigido o problema em que determinados registros foram importados duas vezes com</span><span class="sxs-lookup"><span data-stu-id="a948f-1565">Fixed issue where certain records were imported twice with</span></span> `dns zone import`
* <span data-ttu-id="a948f-1566">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="a948f-1566">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="a948f-1567">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1567">Profile</span></span>

* <span data-ttu-id="a948f-1568">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="a948f-1568">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1569">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1569">Resource</span></span>

* <span data-ttu-id="a948f-1570">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="a948f-1570">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1571">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1571">Storage</span></span>

* <span data-ttu-id="a948f-1572">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="a948f-1572">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="a948f-1573">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="a948f-1573">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="a948f-1574">Corrigido o bug que impedia a opção “-n” arg com</span><span class="sxs-lookup"><span data-stu-id="a948f-1574">Fixed bug preventing "-n" arg option with</span></span> `storage account check-name`
* <span data-ttu-id="a948f-1575">Adicionada a coluna ‘instantâneo’ à saída de tabela para</span><span class="sxs-lookup"><span data-stu-id="a948f-1575">Added 'snapshot' column to table output for</span></span> `blob [list|show]`
* <span data-ttu-id="a948f-1576">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="a948f-1576">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1577">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1577">VM</span></span>

* <span data-ttu-id="a948f-1578">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="a948f-1578">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="a948f-1579">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="a948f-1579">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="a948f-1580">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="a948f-1580">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="a948f-1581">Adicionada proteção para `--admin-password` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1581">Added protection for `--admin-password` to</span></span> `[vm|vmss] create`


## <a name="january-17-2018"></a><span data-ttu-id="a948f-1582">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="a948f-1582">January 17, 2018</span></span>

<span data-ttu-id="a948f-1583">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="a948f-1583">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1584">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1584">ACR</span></span>

* <span data-ttu-id="a948f-1585">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-1585">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="a948f-1586">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="a948f-1586">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1587">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1587">ACS</span></span>

* <span data-ttu-id="a948f-1588">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="a948f-1588">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="a948f-1589">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="a948f-1589">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1590">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1590">Appservice</span></span>

* <span data-ttu-id="a948f-1591">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="a948f-1591">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="a948f-1592">Adicionado suporte para URLs personalizadas a</span><span class="sxs-lookup"><span data-stu-id="a948f-1592">Added support for custom URLs to</span></span> `browse`
* <span data-ttu-id="a948f-1593">Corrigido o suporte de slot para</span><span class="sxs-lookup"><span data-stu-id="a948f-1593">Fixed slot support for</span></span> `log tail`

### <a name="backup"></a><span data-ttu-id="a948f-1594">Backup</span><span class="sxs-lookup"><span data-stu-id="a948f-1594">Backup</span></span>

* <span data-ttu-id="a948f-1595">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="a948f-1595">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="a948f-1596">Adicionadas opções da conta de armazenamento para</span><span class="sxs-lookup"><span data-stu-id="a948f-1596">Added storage account options to</span></span> `backup restore restore-disks`
* <span data-ttu-id="a948f-1597">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-1597">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="a948f-1598">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="a948f-1598">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="a948f-1599">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-1599">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-1600">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1600">Batch</span></span>

* <span data-ttu-id="a948f-1601">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="a948f-1601">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="a948f-1602">Nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-1602">Cloud</span></span>

* <span data-ttu-id="a948f-1603">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-1603">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="a948f-1604">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1604">Consumption</span></span>

* <span data-ttu-id="a948f-1605">Adicionados novos comandos para reservas: `consumption reservations summaries` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1605">Added new commands for reservations: `consumption reservations summaries` and</span></span> `consumption reservations details`

### <a name="event-grid"></a><span data-ttu-id="a948f-1606">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-1606">Event Grid</span></span>

* <span data-ttu-id="a948f-1607">[ALTERAÇÃO DA FALHA] Comandos `az eventgrid topic event-subscription` transferidos para</span><span class="sxs-lookup"><span data-stu-id="a948f-1607">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="a948f-1608">[ALTERAÇÃO DA FALHA] Comandos `az eventgrid resource event-subscription` transferidos para</span><span class="sxs-lookup"><span data-stu-id="a948f-1608">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="a948f-1609">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="a948f-1609">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="a948f-1610">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="a948f-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="a948f-1611">Adicionado comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1611">Added command</span></span> `eventgrid topic update`
* <span data-ttu-id="a948f-1612">Adicionado comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1612">Added command</span></span> `eventgrid event-subscription update`
* <span data-ttu-id="a948f-1613">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="a948f-1613">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="a948f-1614">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="a948f-1614">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-1615">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1615">Interactive</span></span>

* <span data-ttu-id="a948f-1616">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="a948f-1616">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="a948f-1617">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="a948f-1617">Fixed errors on startup</span></span>
* <span data-ttu-id="a948f-1618">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1618">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-1619">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-1619">IoT</span></span>

* <span data-ttu-id="a948f-1620">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1620">Added support for device provisioning service</span></span>
* <span data-ttu-id="a948f-1621">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1621">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="a948f-1622">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-1622">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1623">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1623">Monitor</span></span>

* <span data-ttu-id="a948f-1624">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="a948f-1624">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="a948f-1625">Agora o parâmetro `--name` é necessário para</span><span class="sxs-lookup"><span data-stu-id="a948f-1625">The `--name` parameter is now required for</span></span> `az monitor diagnostic-settings create`
* <span data-ttu-id="a948f-1626">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="a948f-1626">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1627">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1627">Network</span></span>

* <span data-ttu-id="a948f-1628">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com</span><span class="sxs-lookup"><span data-stu-id="a948f-1628">Fixed issue when trying to change to/from active-standby mode with</span></span> `vnet-gateway update`
* <span data-ttu-id="a948f-1629">Adicionado suporte para HTTP2 a</span><span class="sxs-lookup"><span data-stu-id="a948f-1629">Added support for HTTP2 to</span></span> `application-gateway [create|update]`

### <a name="profile"></a><span data-ttu-id="a948f-1630">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1630">Profile</span></span>

* <span data-ttu-id="a948f-1631">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="a948f-1631">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="a948f-1632">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1632">Role</span></span>

* <span data-ttu-id="a948f-1633">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="a948f-1633">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a948f-1634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a948f-1634">Service Fabric</span></span>

* <span data-ttu-id="a948f-1635">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="a948f-1635">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="a948f-1636">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="a948f-1636">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1637">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1637">VM</span></span>

* <span data-ttu-id="a948f-1638">[VERSÃO PRÉVIA] Suporte entre zonas para</span><span class="sxs-lookup"><span data-stu-id="a948f-1638">[PREVIEW] Cross-zone support for</span></span> `vmss`
* <span data-ttu-id="a948f-1639">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="a948f-1639">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="a948f-1640">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="a948f-1640">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="a948f-1641">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a948f-1641">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="a948f-1642">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="a948f-1642">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="a948f-1643">Adicionados argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1643">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to</span></span> `[vm|vmss] create`
* <span data-ttu-id="a948f-1644">Corrigidos os problemas de erro com</span><span class="sxs-lookup"><span data-stu-id="a948f-1644">Fixed error issues with</span></span> `[vm|vmss] create`
* <span data-ttu-id="a948f-1645">Corrigido o uso excessivo de recursos causados por</span><span class="sxs-lookup"><span data-stu-id="a948f-1645">Fixed excessive resource usage caused by</span></span> `vm image list --all`

## <a name="december-19-2017"></a><span data-ttu-id="a948f-1646">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1646">December 19, 2017</span></span>

<span data-ttu-id="a948f-1647">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="a948f-1647">Version 2.0.23</span></span>

* <span data-ttu-id="a948f-1648">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="a948f-1648">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1649">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1649">Container</span></span>

* <span data-ttu-id="a948f-1650">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1650">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1651">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1651">Network</span></span>

* <span data-ttu-id="a948f-1652">Adicionado argumento `--disable-bgp-route-propagation` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1652">Added `--disable-bgp-route-propagation` argument to</span></span> `route-table [create|update]`
* <span data-ttu-id="a948f-1653">Adicionado argumento `--ip-tags` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1653">Added `--ip-tags` argument to</span></span> `public-ip [create|update]`

### <a name="storage"></a><span data-ttu-id="a948f-1654">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1654">Storage</span></span>

* <span data-ttu-id="a948f-1655">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="a948f-1655">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1656">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1656">VM</span></span>

* <span data-ttu-id="a948f-1657">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="a948f-1657">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="a948f-1658">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1658">December 5, 2017</span></span>

<span data-ttu-id="a948f-1659">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="a948f-1659">Version 2.0.22</span></span>

* <span data-ttu-id="a948f-1660">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="a948f-1660">Removed `az component` commands.</span></span> <span data-ttu-id="a948f-1661">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="a948f-1661">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1662">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1662">Core</span></span>
* <span data-ttu-id="a948f-1663">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="a948f-1663">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="a948f-1664">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="a948f-1664">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1665">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1665">ACS</span></span>

* <span data-ttu-id="a948f-1666">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1666">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="a948f-1667">Relatório de erros aprimorado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1667">Improved error reporting for</span></span> `acs create`
* <span data-ttu-id="a948f-1668">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="a948f-1668">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="a948f-1669">Supervisor</span><span class="sxs-lookup"><span data-stu-id="a948f-1669">Advisor</span></span>

* <span data-ttu-id="a948f-1670">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1670">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1671">Appservice</span></span>

* <span data-ttu-id="a948f-1672">Corrigida a geração de nome do certificado com</span><span class="sxs-lookup"><span data-stu-id="a948f-1672">Fixed cert name generation with</span></span> `webapp config ssl upload`
* <span data-ttu-id="a948f-1673">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="a948f-1673">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="a948f-1674">Valor padrão adicionado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1674">Added default value for</span></span> `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a><span data-ttu-id="a948f-1675">Consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1675">Consumption</span></span>

* <span data-ttu-id="a948f-1676">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1676">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1677">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1677">Container</span></span>

* <span data-ttu-id="a948f-1678">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-1678">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1679">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1679">Monitor</span></span>

* <span data-ttu-id="a948f-1680">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="a948f-1680">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1681">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1681">Resource</span></span>

* <span data-ttu-id="a948f-1682">Adicionado argumento `--include-response-body` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1682">Added `--include-response-body` argument to</span></span> `resource show`

### <a name="role"></a><span data-ttu-id="a948f-1683">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-1683">Role</span></span>

* <span data-ttu-id="a948f-1684">Exibição de atribuições padrão adicionada dos administradores "clássicos" a</span><span class="sxs-lookup"><span data-stu-id="a948f-1684">Added display of default assignments for "classic" administraors to</span></span> `role assignment list`
* <span data-ttu-id="a948f-1685">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="a948f-1685">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="a948f-1686">Relatório de erros aprimorado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1686">Improved error reporting for</span></span> `ad sp create-for-rbac`

### <a name="sql"></a><span data-ttu-id="a948f-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1687">SQL</span></span>

* <span data-ttu-id="a948f-1688">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1688">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="a948f-1689">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1689">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1690">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1690">VM</span></span>

* <span data-ttu-id="a948f-1691">Informações da zona adicionadas a</span><span class="sxs-lookup"><span data-stu-id="a948f-1691">Added zone information to</span></span> `az vm list-skus`


## <a name="november-14-2017"></a><span data-ttu-id="a948f-1692">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1692">November 14, 2017</span></span>

<span data-ttu-id="a948f-1693">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="a948f-1693">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-1694">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1694">ACR</span></span>

* <span data-ttu-id="a948f-1695">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="a948f-1695">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="a948f-1696">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1696">ACS</span></span>

* <span data-ttu-id="a948f-1697">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="a948f-1697">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="a948f-1698">Opção `--orchestrator-release` preterida para</span><span class="sxs-lookup"><span data-stu-id="a948f-1698">Deprecated `--orchestrator-release` option for</span></span> `acs create`
* <span data-ttu-id="a948f-1699">Alterado tamanho padrão da VM do AKS para</span><span class="sxs-lookup"><span data-stu-id="a948f-1699">Changed default VM size for AKS to</span></span> `Standard_D1_v2`
* <span data-ttu-id="a948f-1700">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-1700">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="a948f-1701">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="a948f-1701">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1702">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1702">Appservice</span></span>

* <span data-ttu-id="a948f-1703">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="a948f-1703">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="a948f-1704">Adição da opção `--docker-container-logging` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1704">Added `--docker-container-logging` option to</span></span> `az webapp log config`
* <span data-ttu-id="a948f-1705">Removida a opção `storage` do parâmetro `--web-server-logging` de</span><span class="sxs-lookup"><span data-stu-id="a948f-1705">Removed the `storage` option from the parameter `--web-server-logging` of</span></span> `az webapp log config`
* <span data-ttu-id="a948f-1706">Mensagens de erro aprimoradas para</span><span class="sxs-lookup"><span data-stu-id="a948f-1706">Improved error messages for</span></span> `deployment user set`
* <span data-ttu-id="a948f-1707">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="a948f-1707">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="a948f-1708">Correção</span><span class="sxs-lookup"><span data-stu-id="a948f-1708">Fixed</span></span> `list-locations`

### <a name="batch"></a><span data-ttu-id="a948f-1709">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1709">Batch</span></span>

* <span data-ttu-id="a948f-1710">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="a948f-1710">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="a948f-1711">Batchai</span><span class="sxs-lookup"><span data-stu-id="a948f-1711">Batchai</span></span>

* <span data-ttu-id="a948f-1712">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1712">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="a948f-1713">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1713">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="a948f-1714">Documentação corrigida para `job list-files` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1714">Fixed documentation for `job list-files` and</span></span> `job stream-file`
* <span data-ttu-id="a948f-1715">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1715">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="a948f-1716">Nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-1716">Cloud</span></span>

* <span data-ttu-id="a948f-1717">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="a948f-1717">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1718">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1718">Container</span></span>

* <span data-ttu-id="a948f-1719">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="a948f-1719">Added support to open multiple ports</span></span>
* <span data-ttu-id="a948f-1720">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="a948f-1720">Added container group restart policy</span></span>
* <span data-ttu-id="a948f-1721">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="a948f-1721">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="a948f-1722">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="a948f-1722">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a948f-1723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a948f-1723">Data Lake Analytics</span></span>

* <span data-ttu-id="a948f-1724">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="a948f-1724">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a948f-1725">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-1725">Data Lake Store</span></span>

* <span data-ttu-id="a948f-1726">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="a948f-1726">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="a948f-1727">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1727">Extension</span></span>

* <span data-ttu-id="a948f-1728">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a948f-1728">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="a948f-1729">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="a948f-1729">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-1730">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-1730">IoT</span></span>

* <span data-ttu-id="a948f-1731">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="a948f-1731">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1732">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1732">Monitor</span></span>

* <span data-ttu-id="a948f-1733">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="a948f-1733">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1734">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1734">Network</span></span>

* <span data-ttu-id="a948f-1735">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="a948f-1735">Added support for CAA DNS records</span></span>
* <span data-ttu-id="a948f-1736">Problema corrigido em que os pontos de extremidade não podiam ser atualizados com</span><span class="sxs-lookup"><span data-stu-id="a948f-1736">Fixed issue where endpoints could not be updated with</span></span> `traffic-manager profile update`
* <span data-ttu-id="a948f-1737">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="a948f-1737">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="a948f-1738">Problema corrigido em que os nomes DNS relativos eram importados incorretamente por</span><span class="sxs-lookup"><span data-stu-id="a948f-1738">Fixed issue where relative DNS names were incorrectly imported by</span></span> `dns zone import`

### <a name="reservations"></a><span data-ttu-id="a948f-1739">Reservas</span><span class="sxs-lookup"><span data-stu-id="a948f-1739">Reservations</span></span>

* <span data-ttu-id="a948f-1740">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1740">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1741">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1741">Resource</span></span>

* <span data-ttu-id="a948f-1742">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1742">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1743">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1743">SQL</span></span>

* <span data-ttu-id="a948f-1744">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1744">Added `--ignore-missing-vnet-service-endpoint` parameter to</span></span> `sql server vnet-rule [create|update]`

### <a name="storage"></a><span data-ttu-id="a948f-1745">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1745">Storage</span></span>

* <span data-ttu-id="a948f-1746">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-1746">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="a948f-1747">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="a948f-1747">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="a948f-1748">Bug corrigido que impedia usar `--source-uri` com</span><span class="sxs-lookup"><span data-stu-id="a948f-1748">Fixed bug that prevented using `--source-uri` with</span></span> `storage [blob|file] copy start-batch`
* <span data-ttu-id="a948f-1749">Comandos adicionados para usar o glob e excluir vários objetos com</span><span class="sxs-lookup"><span data-stu-id="a948f-1749">Added commands to glob and delete multiple objects with</span></span> `storage [blob|file] delete-batch`
* <span data-ttu-id="a948f-1750">Problema corrigido ao habilitar métricas com</span><span class="sxs-lookup"><span data-stu-id="a948f-1750">Fixed issue when enabling metrics with</span></span> `storage metrics update`
* <span data-ttu-id="a948f-1751">Problema corrigido com arquivos acima de 200 GB ao usar</span><span class="sxs-lookup"><span data-stu-id="a948f-1751">Fixed issue with files over 200GB when using</span></span> `storage blob upload-batch`
* <span data-ttu-id="a948f-1752">Problema corrigido em que `--bypass` e `--default-action` foram ignorados por</span><span class="sxs-lookup"><span data-stu-id="a948f-1752">Fixed issue where `--bypass` and `--default-action` were ignored by</span></span> `storage account [create|update]`

### <a name="vm"></a><span data-ttu-id="a948f-1753">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1753">VM</span></span>

* <span data-ttu-id="a948f-1754">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="a948f-1754">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="a948f-1755">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="a948f-1755">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="a948f-1756">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1756">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="a948f-1757">`vm format-secret` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1757">Renamed `vm format-secret` to</span></span> `vm secret format`
* <span data-ttu-id="a948f-1758">Adicionado argumento `--encrypt format` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1758">Added `--encrypt format` argument to</span></span> `vm encryption enable`

## <a name="october-24-2017"></a><span data-ttu-id="a948f-1759">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1759">October 24, 2017</span></span>

<span data-ttu-id="a948f-1760">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="a948f-1760">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1761">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1761">Core</span></span>

* <span data-ttu-id="a948f-1762">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API</span><span class="sxs-lookup"><span data-stu-id="a948f-1762">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version</span></span> `2016-01-01`

### <a name="acr"></a><span data-ttu-id="a948f-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-1763">ACR</span></span>

* <span data-ttu-id="a948f-1764">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="a948f-1764">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="a948f-1765">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="a948f-1765">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="a948f-1766">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="a948f-1766">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1767">ACS</span></span>

* <span data-ttu-id="a948f-1768">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="a948f-1768">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="a948f-1769">Kubernetes corrigido</span><span class="sxs-lookup"><span data-stu-id="a948f-1769">Fixed kubernetes</span></span> `get-credentials`

### <a name="appservice"></a><span data-ttu-id="a948f-1770">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1770">Appservice</span></span>

* <span data-ttu-id="a948f-1771">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="a948f-1771">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="a948f-1772">Componente</span><span class="sxs-lookup"><span data-stu-id="a948f-1772">Component</span></span>

* <span data-ttu-id="a948f-1773">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="a948f-1773">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-1774">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-1774">Monitor</span></span>

* <span data-ttu-id="a948f-1775">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="a948f-1775">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1776">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1776">Resource</span></span>

* <span data-ttu-id="a948f-1777">Incompatibilidade corrigida com a versão mais recente de dependência msrest em</span><span class="sxs-lookup"><span data-stu-id="a948f-1777">Fixed incompatibility with most recent version of msrest dependency in</span></span> `group export`
* <span data-ttu-id="a948f-1778">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="a948f-1778">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1779">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1779">VM</span></span>

* <span data-ttu-id="a948f-1780">Adicionado argumento `--accelerated-networking` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1780">Added `--accelerated-networking` argument to</span></span> `vmss create`


## <a name="october-9-2017"></a><span data-ttu-id="a948f-1781">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1781">October 9, 2017</span></span>

<span data-ttu-id="a948f-1782">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="a948f-1782">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1783">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1783">Core</span></span>

* <span data-ttu-id="a948f-1784">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a948f-1784">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1785">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1785">Appservice</span></span>

* <span data-ttu-id="a948f-1786">Atualização genérica adicionada com o novo comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1786">Added generic update with new command</span></span> `webapp update`

### <a name="batch"></a><span data-ttu-id="a948f-1787">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1787">Batch</span></span>

* <span data-ttu-id="a948f-1788">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="a948f-1788">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="a948f-1789">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="a948f-1789">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="a948f-1790">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1790">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="a948f-1791">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="a948f-1791">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="a948f-1792">Batchai</span><span class="sxs-lookup"><span data-stu-id="a948f-1792">Batchai</span></span>

* <span data-ttu-id="a948f-1793">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1793">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-1794">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a948f-1794">Keyvault</span></span>

* <span data-ttu-id="a948f-1795">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="a948f-1795">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="a948f-1796">(#4448)</span><span class="sxs-lookup"><span data-stu-id="a948f-1796">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="a948f-1797">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1797">Network</span></span>

* <span data-ttu-id="a948f-1798">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="a948f-1798">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="a948f-1799">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1799">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1800">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1800">Resource</span></span>

* <span data-ttu-id="a948f-1801">Suporte adicionado para opções `--resource-group/-g` do nome do grupo de recursos a</span><span class="sxs-lookup"><span data-stu-id="a948f-1801">Added support for `--resource-group/-g` options for resource group name to</span></span> `group`
* <span data-ttu-id="a948f-1802">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-1802">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="a948f-1803">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="a948f-1803">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="a948f-1804">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1804">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1805">Sql</span><span class="sxs-lookup"><span data-stu-id="a948f-1805">Sql</span></span>

* <span data-ttu-id="a948f-1806">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="a948f-1806">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="a948f-1807">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="a948f-1807">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="a948f-1808">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="a948f-1808">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1809">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1809">Storage</span></span>

* <span data-ttu-id="a948f-1810">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="a948f-1810">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1811">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1811">Vm</span></span>

* <span data-ttu-id="a948f-1812">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1812">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="a948f-1813">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção a</span><span class="sxs-lookup"><span data-stu-id="a948f-1813">[PREVIEW] Added support for rolling upgrade to</span></span> `vmss create`
* <span data-ttu-id="a948f-1814">Suporte adicionado para atualizar as configurações de criptografia com</span><span class="sxs-lookup"><span data-stu-id="a948f-1814">Added support for updating encryption settings with</span></span> `vm encryption enable`
* <span data-ttu-id="a948f-1815">Parâmetro `--os-disk-size-gb` adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1815">Added `--os-disk-size-gb` parameter to</span></span> `vm create`
* <span data-ttu-id="a948f-1816">Parâmetro `--license-type` para Windows adicionado a</span><span class="sxs-lookup"><span data-stu-id="a948f-1816">Added `--license-type` parameter for Windows to</span></span> `vmss create`


## <a name="september-22-2017"></a><span data-ttu-id="a948f-1817">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1817">September 22, 2017</span></span>

<span data-ttu-id="a948f-1818">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="a948f-1818">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-1819">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1819">Resource</span></span>

* <span data-ttu-id="a948f-1820">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="a948f-1820">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="a948f-1821">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="a948f-1821">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="a948f-1822">Suporte adicionado para definições de interface do usuário e modelos a</span><span class="sxs-lookup"><span data-stu-id="a948f-1822">Added support for UI definitions and templates to</span></span> `managedapp definition create`
* <span data-ttu-id="a948f-1823">[ALTERAÇÃO DA FALHA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para</span><span class="sxs-lookup"><span data-stu-id="a948f-1823">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to</span></span> `applicationDefinitions`

### <a name="network"></a><span data-ttu-id="a948f-1824">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1824">Network</span></span>

* <span data-ttu-id="a948f-1825">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="a948f-1825">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="a948f-1826">Suporte adicionado para Emparelhamento IPv6 da Microsoft a</span><span class="sxs-lookup"><span data-stu-id="a948f-1826">Added support for IPv6 Microsoft Peering to</span></span> `express-route`
* <span data-ttu-id="a948f-1827">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1827">Added `asg` application security group commands</span></span>
* <span data-ttu-id="a948f-1828">Adicionado argumento `--application-security-groups` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1828">Added `--application-security-groups` argument to</span></span> `nic [create|ip-config create|ip-config update]`
* <span data-ttu-id="a948f-1829">Adicionados argumentos `--source-asgs` e `--destination-asgs` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1829">Added `--source-asgs` and `--destination-asgs` arguments to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="a948f-1830">Adicionados argumentos `--ddos-protection` e `--vm-protection` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1830">Added `--ddos-protection` and `--vm-protection` arguments to</span></span> `vnet [create|update]`
* <span data-ttu-id="a948f-1831">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="a948f-1831">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1832">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1832">Storage</span></span>

* <span data-ttu-id="a948f-1833">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="a948f-1833">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="a948f-1834">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-1834">Eventgrid</span></span>

* <span data-ttu-id="a948f-1835">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="a948f-1835">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1836">SQL</span></span>

* <span data-ttu-id="a948f-1837">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="a948f-1837">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="a948f-1838">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="a948f-1838">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="a948f-1839">Adicionado parâmetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1839">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and</span></span> `dw [create|update]`

### <a name="keyvault"></a><span data-ttu-id="a948f-1840">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a948f-1840">Keyvault</span></span>

* <span data-ttu-id="a948f-1841">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="a948f-1841">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1842">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1842">VM</span></span>

* <span data-ttu-id="a948f-1843">Adicionado suporte para zona de disponibilidade a</span><span class="sxs-lookup"><span data-stu-id="a948f-1843">Added for support to availability zone to</span></span> `[vm|vmss|disk] create`
* <span data-ttu-id="a948f-1844">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="a948f-1844">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="a948f-1845">Adicionado argumento `--asgs` a</span><span class="sxs-lookup"><span data-stu-id="a948f-1845">Added `--asgs` argument to</span></span> `vm create`
* <span data-ttu-id="a948f-1846">Suporte adicionado para executar comandos em VMs com</span><span class="sxs-lookup"><span data-stu-id="a948f-1846">Added support for running commands on VMs with</span></span> `vm run-command`
* <span data-ttu-id="a948f-1847">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com</span><span class="sxs-lookup"><span data-stu-id="a948f-1847">[PREVIEW] Added support for VMSS disk encryption with</span></span> `vmss encryption`
* <span data-ttu-id="a948f-1848">Suporte adicionado para realizar a manutenção nas máquinas virtuais com</span><span class="sxs-lookup"><span data-stu-id="a948f-1848">Added support for performing maintenance on VMs with</span></span> `vm perform-maintenance`

### <a name="acs"></a><span data-ttu-id="a948f-1849">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1849">ACS</span></span>

* <span data-ttu-id="a948f-1850">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1850">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1851">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1851">Appservice</span></span>

* <span data-ttu-id="a948f-1852">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com</span><span class="sxs-lookup"><span data-stu-id="a948f-1852">Added ability to update and show authentication settings with</span></span> `webapp auth [update|show]`

### <a name="backup"></a><span data-ttu-id="a948f-1853">Backup</span><span class="sxs-lookup"><span data-stu-id="a948f-1853">Backup</span></span>

* <span data-ttu-id="a948f-1854">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-1854">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="a948f-1855">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1855">September 11, 2017</span></span>

<span data-ttu-id="a948f-1856">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="a948f-1856">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="a948f-1857">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1857">Core</span></span>

* <span data-ttu-id="a948f-1858">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="a948f-1858">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="a948f-1859">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="a948f-1859">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1860">Acs</span><span class="sxs-lookup"><span data-stu-id="a948f-1860">Acs</span></span>

* <span data-ttu-id="a948f-1861">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="a948f-1861">Added `acs list-locations` command</span></span>
* <span data-ttu-id="a948f-1862">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="a948f-1862">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1863">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1863">Appservice</span></span>

* <span data-ttu-id="a948f-1864">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1864">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="a948f-1865">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-1865">CDN</span></span>

* <span data-ttu-id="a948f-1866">Bug “Não é possível interar CustomDomain” corrigido para</span><span class="sxs-lookup"><span data-stu-id="a948f-1866">Fixed 'CustomDomain is not interable' bug for</span></span> `cdn custom-domain create`

### <a name="extension"></a><span data-ttu-id="a948f-1867">Extensão</span><span class="sxs-lookup"><span data-stu-id="a948f-1867">Extension</span></span>

* <span data-ttu-id="a948f-1868">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1868">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-1869">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a948f-1869">Keyvault</span></span>

* <span data-ttu-id="a948f-1870">Correção de problema em que as permissões diferenciam maiúsculas e minúsculas para</span><span class="sxs-lookup"><span data-stu-id="a948f-1870">Fixed issue where permissions were case sensitive for</span></span> `keyvault set-policy`

### <a name="network"></a><span data-ttu-id="a948f-1871">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1871">Network</span></span>

* <span data-ttu-id="a948f-1872">`vnet list-private-access-services` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1872">Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="a948f-1873">Argumento `--private-access-services` renomeado para `--service-endpoints` de</span><span class="sxs-lookup"><span data-stu-id="a948f-1873">Renamed `--private-access-services` argument to `--service-endpoints` for</span></span> `vnet subnet create/update`
* <span data-ttu-id="a948f-1874">Adição de suporte para intervalos de IP múltiplos e intervalos de porta a</span><span class="sxs-lookup"><span data-stu-id="a948f-1874">Added support for multiple IP ranges and port ranges to</span></span> `nsg rule create/update`
* <span data-ttu-id="a948f-1875">Adição de suporte para SKU a</span><span class="sxs-lookup"><span data-stu-id="a948f-1875">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="a948f-1876">Adição de suporte para SKU a</span><span class="sxs-lookup"><span data-stu-id="a948f-1876">Added support for SKU to</span></span> `public-ip create`

### <a name="resource"></a><span data-ttu-id="a948f-1877">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1877">Resource</span></span>

* <span data-ttu-id="a948f-1878">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-1878">Allow passing in resource policy parameter definitions in `policy definition create`, and</span></span> `policy definition update`
* <span data-ttu-id="a948f-1879">Permitir a passagem de valores de parâmetro para</span><span class="sxs-lookup"><span data-stu-id="a948f-1879">Allow passing in parameter values for</span></span> `policy assignment create`
* <span data-ttu-id="a948f-1880">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="a948f-1880">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="a948f-1881">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="a948f-1881">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-1882">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-1882">SQL</span></span>

* <span data-ttu-id="a948f-1883">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="a948f-1883">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1884">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1884">VM</span></span>

* <span data-ttu-id="a948f-1885">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="a948f-1885">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="a948f-1886">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="a948f-1886">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="a948f-1887">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="a948f-1887">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="a948f-1888">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-1888">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="a948f-1889">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="a948f-1889">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="a948f-1890">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1890">August 31, 2017</span></span>

<span data-ttu-id="a948f-1891">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="a948f-1891">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-1892">Keyvault</span><span class="sxs-lookup"><span data-stu-id="a948f-1892">Keyvault</span></span>

* <span data-ttu-id="a948f-1893">Correção de bug ao tentar resolver automaticamente a codificação secreta com</span><span class="sxs-lookup"><span data-stu-id="a948f-1893">Fixed bug when trying to automatically resolve secret encoding with</span></span> `secret download`

### <a name="sf"></a><span data-ttu-id="a948f-1894">Sf</span><span class="sxs-lookup"><span data-stu-id="a948f-1894">Sf</span></span>

* <span data-ttu-id="a948f-1895">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="a948f-1895">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1896">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1896">Storage</span></span>

* <span data-ttu-id="a948f-1897">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="a948f-1897">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="a948f-1898">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="a948f-1898">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="a948f-1899">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1899">August 28, 2017</span></span>

<span data-ttu-id="a948f-1900">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="a948f-1900">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="a948f-1901">CLI</span><span class="sxs-lookup"><span data-stu-id="a948f-1901">CLI</span></span>

* <span data-ttu-id="a948f-1902">Nota legal adicionada ao</span><span class="sxs-lookup"><span data-stu-id="a948f-1902">Added legal note to</span></span> `--version`

### <a name="acs"></a><span data-ttu-id="a948f-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1903">ACS</span></span>

* <span data-ttu-id="a948f-1904">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="a948f-1904">Corrected preview regions</span></span>
* <span data-ttu-id="a948f-1905">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="a948f-1905">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="a948f-1906">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="a948f-1906">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1907">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1907">Appservice</span></span>

* <span data-ttu-id="a948f-1908">[ALTERAÇÃO DA FALHA] Corrigidas as inconsistências na saída de</span><span class="sxs-lookup"><span data-stu-id="a948f-1908">[BREAKING CHANGE] Fixed inconsistencies in the output of</span></span> `az webapp config appsettings [delete|set]`
* <span data-ttu-id="a948f-1909">Adicionado um novo alias de `-i` para</span><span class="sxs-lookup"><span data-stu-id="a948f-1909">Added a new alias of `-i` for</span></span> `az webapp config container set --docker-custom-image-name`
* <span data-ttu-id="a948f-1910">Exposto</span><span class="sxs-lookup"><span data-stu-id="a948f-1910">Exposed</span></span> `az webapp log show`
* <span data-ttu-id="a948f-1911">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-1911">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="a948f-1912">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-1912">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-1913">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-1913">IoT</span></span>

* <span data-ttu-id="a948f-1914">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="a948f-1914">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1915">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1915">Network</span></span>

* <span data-ttu-id="a948f-1916">[ALTERAÇÃO DA FALHA] `vnet list-private-access-services` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-1916">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="a948f-1917">[ALTERAÇÃO DA FALHA] Opção `--private-access-services` renomeada como `--service-endpoints` para</span><span class="sxs-lookup"><span data-stu-id="a948f-1917">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for</span></span> `vnet subnet [create|update]`
* <span data-ttu-id="a948f-1918">Adicionado suporte para vários intervalos de IP e portas a</span><span class="sxs-lookup"><span data-stu-id="a948f-1918">Added support for multiple IP and port ranges to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="a948f-1919">Adição de suporte para SKU a</span><span class="sxs-lookup"><span data-stu-id="a948f-1919">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="a948f-1920">Adição de suporte para SKU a</span><span class="sxs-lookup"><span data-stu-id="a948f-1920">Added support for SKU to</span></span> `public-ip create`

### <a name="profile"></a><span data-ttu-id="a948f-1921">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1921">Profile</span></span>

* <span data-ttu-id="a948f-1922">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="a948f-1922">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a948f-1923">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a948f-1923">Service Fabric</span></span>

* <span data-ttu-id="a948f-1924">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="a948f-1924">Preview release</span></span>
* <span data-ttu-id="a948f-1925">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1925">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="a948f-1926">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="a948f-1926">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="a948f-1927">Adicionado suporte para vazio de</span><span class="sxs-lookup"><span data-stu-id="a948f-1927">Added support for empty</span></span> `registry_cred`

### <a name="storage"></a><span data-ttu-id="a948f-1928">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1928">Storage</span></span>

* <span data-ttu-id="a948f-1929">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="a948f-1929">Enabled setting blob tier</span></span>
* <span data-ttu-id="a948f-1930">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="a948f-1930">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="a948f-1931">Adicionados comandos para adicionar regras de rede virtual e regras baseadas em IP a</span><span class="sxs-lookup"><span data-stu-id="a948f-1931">Added commands to add VNET rules and IP based rules to</span></span> `storage account network-rule`
* <span data-ttu-id="a948f-1932">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="a948f-1932">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="a948f-1933">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="a948f-1933">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="a948f-1934">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="a948f-1934">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1935">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1935">VM</span></span>

* <span data-ttu-id="a948f-1936">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar</span><span class="sxs-lookup"><span data-stu-id="a948f-1936">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using</span></span> `--instance-id *`
* <span data-ttu-id="a948f-1937">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="a948f-1937">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="a948f-1938">Removidos nomes humanos da lista de bloqueio de nomes de administrador para</span><span class="sxs-lookup"><span data-stu-id="a948f-1938">Removed human names from the admin name blacklist for</span></span> `[vm|vmss] create`
* <span data-ttu-id="a948f-1939">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="a948f-1939">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="a948f-1940">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="a948f-1940">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="a948f-1941">Corrigido o problema em que o argumento `--no-wait` não funcionava com</span><span class="sxs-lookup"><span data-stu-id="a948f-1941">Fixed issue where `--no-wait` argument did not work wth</span></span> `vm availability-set create`


## <a name="august-15-2017"></a><span data-ttu-id="a948f-1942">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1942">August 15, 2017</span></span>

<span data-ttu-id="a948f-1943">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="a948f-1943">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1944">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1944">ACS</span></span>

* <span data-ttu-id="a948f-1945">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="a948f-1945">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-1946">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-1946">Appservice</span></span>

* <span data-ttu-id="a948f-1947">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="a948f-1947">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="a948f-1948">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-1948">Event Grid</span></span>

* <span data-ttu-id="a948f-1949">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="a948f-1949">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="a948f-1950">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1950">August 11, 2017</span></span>

<span data-ttu-id="a948f-1951">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="a948f-1951">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-1952">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-1952">ACS</span></span>

* <span data-ttu-id="a948f-1953">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="a948f-1953">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="a948f-1954">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-1954">Batch</span></span>

* <span data-ttu-id="a948f-1955">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="a948f-1955">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="a948f-1956">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="a948f-1956">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="a948f-1957">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-1957">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="a948f-1958">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="a948f-1958">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="a948f-1959">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="a948f-1959">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="a948f-1960">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="a948f-1960">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="a948f-1961">Componente</span><span class="sxs-lookup"><span data-stu-id="a948f-1961">Component</span></span>

* <span data-ttu-id="a948f-1962">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="a948f-1962">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="a948f-1963">Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1963">Container</span></span>

* `create`<span data-ttu-id="a948f-1964">: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="a948f-1964">: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="a948f-1965">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-1965">Data Lake Store</span></span>

* <span data-ttu-id="a948f-1966">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1966">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="a948f-1967">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="a948f-1967">Event Grid</span></span>

* <span data-ttu-id="a948f-1968">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="a948f-1968">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="a948f-1969">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-1969">Network</span></span>

* `lb`<span data-ttu-id="a948f-1970">: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="a948f-1970">: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* `application-gateway {subresource} delete`<span data-ttu-id="a948f-1971">: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="a948f-1971">: Fixed issue where `--no-wait` was not honored</span></span>
* `application-gateway http-settings update`<span data-ttu-id="a948f-1972">: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="a948f-1972">: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="a948f-1973">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com</span><span class="sxs-lookup"><span data-stu-id="a948f-1973">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with</span></span> `az network vpn-connection ipsec-policy add`

### <a name="profile"></a><span data-ttu-id="a948f-1974">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-1974">Profile</span></span>

* `account list`<span data-ttu-id="a948f-1975">: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="a948f-1975">: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-1976">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-1976">Storage</span></span>

* <span data-ttu-id="a948f-1977">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="a948f-1977">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-1978">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-1978">VM</span></span>

* `availability-set`<span data-ttu-id="a948f-1979">: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="a948f-1979">: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="a948f-1980">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="a948f-1980">Exposed `list-skus` command</span></span>
* <span data-ttu-id="a948f-1981">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="a948f-1981">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="a948f-1982">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="a948f-1982">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="a948f-1983">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="a948f-1983">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="a948f-1984">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-1984">July 28, 2017</span></span>

<span data-ttu-id="a948f-1985">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="a948f-1985">Version 2.0.12</span></span>

* <span data-ttu-id="a948f-1986">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-1986">Added container commands</span></span>
* <span data-ttu-id="a948f-1987">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="a948f-1987">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="a948f-1988">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-1988">Core</span></span>

* <span data-ttu-id="a948f-1989">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="a948f-1989">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="a948f-1990">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="a948f-1990">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="a948f-1991">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="a948f-1991">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="a948f-1992">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="a948f-1992">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="a948f-1993">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="a948f-1993">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="a948f-1994">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="a948f-1994">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="a948f-1995">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="a948f-1995">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a948f-1996">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="a948f-1996">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="a948f-1997">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="a948f-1997">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="a948f-1998">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="a948f-1998">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="a948f-1999">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="a948f-1999">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="a948f-2000">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="a948f-2000">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="a948f-2001">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-2001">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="a948f-2002">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="a948f-2002">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="a948f-2003">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="a948f-2003">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="a948f-2004">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="a948f-2004">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="a948f-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-2005">ACR</span></span>

* <span data-ttu-id="a948f-2006">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="a948f-2006">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="a948f-2007">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="a948f-2007">Support SKU update for managed registries</span></span>
* <span data-ttu-id="a948f-2008">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="a948f-2008">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="a948f-2009">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-2009">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="a948f-2010">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-2010">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="a948f-2011">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="a948f-2011">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-2012">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-2012">ACS</span></span>

* <span data-ttu-id="a948f-2013">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="a948f-2013">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-2014">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-2014">Appservice</span></span>

* <span data-ttu-id="a948f-2015">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="a948f-2015">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="a948f-2016">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="a948f-2016">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="a948f-2017">Remover todos os comandos em</span><span class="sxs-lookup"><span data-stu-id="a948f-2017">Remove all commands under</span></span> `appservice web`
* <span data-ttu-id="a948f-2018">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="a948f-2018">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="a948f-2019">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="a948f-2019">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="a948f-2020">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="a948f-2020">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="a948f-2021">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="a948f-2021">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="a948f-2022">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="a948f-2022">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="a948f-2023">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="a948f-2023">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="a948f-2024">Em vez disso, use</span><span class="sxs-lookup"><span data-stu-id="a948f-2024">Instead use</span></span> `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a><span data-ttu-id="a948f-2025">Lote</span><span class="sxs-lookup"><span data-stu-id="a948f-2025">Batch</span></span>

* <span data-ttu-id="a948f-2026">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="a948f-2026">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="a948f-2027">Opção `pool create` renomeada como `--target-dedicated` para</span><span class="sxs-lookup"><span data-stu-id="a948f-2027">Renamed `pool create` option `--target-dedicated` to</span></span> `--target-dedicated-nodes`
* <span data-ttu-id="a948f-2028">Adicionadas opções `pool create` e `--target-low-priority-nodes` de</span><span class="sxs-lookup"><span data-stu-id="a948f-2028">Added `pool create` options `--target-low-priority-nodes` and</span></span> `--application-licenses`

### <a name="cdn"></a><span data-ttu-id="a948f-2029">CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-2029">CDN</span></span>

* <span data-ttu-id="a948f-2030">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="a948f-2030">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="a948f-2031">Nuvem</span><span class="sxs-lookup"><span data-stu-id="a948f-2031">Cloud</span></span>

* <span data-ttu-id="a948f-2032">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="a948f-2032">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="a948f-2033">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="a948f-2033">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="a948f-2034">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="a948f-2034">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="a948f-2035">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="a948f-2035">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="a948f-2036">Exposto</span><span class="sxs-lookup"><span data-stu-id="a948f-2036">Exposed</span></span> `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a><span data-ttu-id="a948f-2037">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-2037">CosmosDB</span></span>

* <span data-ttu-id="a948f-2038">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="a948f-2038">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="a948f-2039">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="a948f-2039">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a948f-2040">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a948f-2040">Data Lake Analytics</span></span>

* <span data-ttu-id="a948f-2041">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="a948f-2041">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="a948f-2042">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-2042">Added</span></span> `dla job pipeline show`
* <span data-ttu-id="a948f-2043">Added</span><span class="sxs-lookup"><span data-stu-id="a948f-2043">Added</span></span> `dla job recurrence list`

### <a name="data-lake-store"></a><span data-ttu-id="a948f-2044">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-2044">Data Lake Store</span></span>

* <span data-ttu-id="a948f-2045">Adicionado suporte para a rotação de chaves gerenciadas do usuário do cofre de chaves em</span><span class="sxs-lookup"><span data-stu-id="a948f-2045">Added support for user managed key vault key rotation in</span></span> `dls account update`
* <span data-ttu-id="a948f-2046">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="a948f-2046">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="a948f-2047">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="a948f-2047">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="a948f-2048">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-2048">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="a948f-2049">Interativo</span><span class="sxs-lookup"><span data-stu-id="a948f-2049">Interactive</span></span>

* <span data-ttu-id="a948f-2050">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="a948f-2050">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="a948f-2051">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="a948f-2051">Increased test coverage</span></span>
* <span data-ttu-id="a948f-2052">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="a948f-2052">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="a948f-2053">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="a948f-2053">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="a948f-2054">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="a948f-2054">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="a948f-2055">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="a948f-2055">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="a948f-2056">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="a948f-2056">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="a948f-2057">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="a948f-2057">Added `--progress` flag</span></span>
* <span data-ttu-id="a948f-2058">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="a948f-2058">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="a948f-2059">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="a948f-2059">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="a948f-2060">IoT</span><span class="sxs-lookup"><span data-stu-id="a948f-2060">IoT</span></span>

* <span data-ttu-id="a948f-2061">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="a948f-2061">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="a948f-2062">(#3934)</span><span class="sxs-lookup"><span data-stu-id="a948f-2062">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="a948f-2063">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="a948f-2063">Key vault</span></span>

* <span data-ttu-id="a948f-2064">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="a948f-2064">Added commands for key vault recovery features:</span></span>
  * `keyvault` <span data-ttu-id="a948f-2065">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2065">subcommands `purge`, `recover`,</span></span> `keyvault list-deleted`
  * `keyvault secret` <span data-ttu-id="a948f-2066">subcomandos `backup`, `restore`, `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2066">subcommands `backup`, `restore`, `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault certificate` <span data-ttu-id="a948f-2067">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2067">subcommands `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault key` <span data-ttu-id="a948f-2068">subcomandos `purge`, `recover`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2068">subcommands `purge`, `recover`,</span></span> `list-deleted`
* <span data-ttu-id="a948f-2069">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="a948f-2069">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="a948f-2070">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="a948f-2070">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="a948f-2071">(#3307)</span><span class="sxs-lookup"><span data-stu-id="a948f-2071">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="a948f-2072">Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2072">Lab</span></span>

* <span data-ttu-id="a948f-2073">Adicionado suporte para reivindicar qualquer VM no laboratório por meio de</span><span class="sxs-lookup"><span data-stu-id="a948f-2073">Added support for claiming any vm in the lab through</span></span> `az lab vm claim`
* <span data-ttu-id="a948f-2074">Adicionado formatador de saída da tabela para `az lab vm list` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2074">Added table output formatter for `az lab vm list` and</span></span> `az lab vm show`

### <a name="monitor"></a><span data-ttu-id="a948f-2075">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-2075">Monitor</span></span>

* <span data-ttu-id="a948f-2076">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="a948f-2076">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="a948f-2077">`monitor alert-rule-incidents list` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-2077">Renamed `monitor alert-rule-incidents list` to</span></span> `monitor alert list-incidents`
* <span data-ttu-id="a948f-2078">`monitor alert-rule-incidents show` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-2078">Renamed `monitor alert-rule-incidents show` to</span></span> `monitor alert show-incident`
* <span data-ttu-id="a948f-2079">`monitor metric-defintions list` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-2079">Renamed `monitor metric-defintions list` to</span></span> `monitor metrics list-definitions`
* <span data-ttu-id="a948f-2080">`monitor alert-rules` renomeado para</span><span class="sxs-lookup"><span data-stu-id="a948f-2080">Renamed `monitor alert-rules` to</span></span> `monitor alert`
* <span data-ttu-id="a948f-2081">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="a948f-2081">Changed `monitor alert create`:</span></span>
  * `condition` <span data-ttu-id="a948f-2082">e JSON não será mais aceito pelos subcomandos `action`</span><span class="sxs-lookup"><span data-stu-id="a948f-2082">and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="a948f-2083">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="a948f-2083">Add numerous parameters to simplify the rule creation process</span></span>
  * `location` <span data-ttu-id="a948f-2084">não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="a948f-2084">no longer required</span></span>
  * <span data-ttu-id="a948f-2085">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="a948f-2085">Add name and ID support for target</span></span>
  * <span data-ttu-id="a948f-2086">Remover</span><span class="sxs-lookup"><span data-stu-id="a948f-2086">Remove</span></span> `--alert-rule-resource-name`
  * <span data-ttu-id="a948f-2087">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="a948f-2087">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * `description` <span data-ttu-id="a948f-2088">agora os padrões são baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="a948f-2088">defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="a948f-2089">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="a948f-2089">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="a948f-2090">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="a948f-2090">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="a948f-2091">Exemplos e argumentos de conveniência adicionados ao</span><span class="sxs-lookup"><span data-stu-id="a948f-2091">Added convenience arguments and examples to</span></span> `monitor alert rule update`

### <a name="network"></a><span data-ttu-id="a948f-2092">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-2092">Network</span></span>

* <span data-ttu-id="a948f-2093">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="a948f-2093">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="a948f-2094">Adicionado argumento `--private-access-services` a `vnet subnet create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2094">Added `--private-access-services` argument to `vnet subnet create` and</span></span> `vnet subnet update`
* <span data-ttu-id="a948f-2095">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="a948f-2095">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="a948f-2096">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="a948f-2096">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="a948f-2097">Corrigido bug ao usar o argumento `--servers` com `application-gateway address-pool create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2097">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and</span></span> `application-gateway address-pool update`
* <span data-ttu-id="a948f-2098">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="a948f-2098">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="a948f-2099">Adicionados comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2099">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`,</span></span> `predefined show`
* <span data-ttu-id="a948f-2100">Adicionados argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2100">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span></span> `--min-protocol-version`
* <span data-ttu-id="a948f-2101">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="a948f-2101">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="a948f-2102">Adicionados argumentos a `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2102">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`,</span></span> `--redirect-config`
* <span data-ttu-id="a948f-2103">Adicionado argumento `--redirect-config` a</span><span class="sxs-lookup"><span data-stu-id="a948f-2103">Added argument `--redirect-config` to</span></span> `application-gateway url-path-map rule create`
* <span data-ttu-id="a948f-2104">Adição do suporte para `--no-wait` a</span><span class="sxs-lookup"><span data-stu-id="a948f-2104">Added support for `--no-wait` to</span></span> `application-gateway url-path-map rule delete`
* <span data-ttu-id="a948f-2105">Adicionados argumentos a `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span><span class="sxs-lookup"><span data-stu-id="a948f-2105">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span></span> `--match-status-codes`
* <span data-ttu-id="a948f-2106">Adicionado argumento `--redirect-config` a `application-gateway rule create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2106">Added argument `--redirect-config` to `application-gateway rule create` and</span></span> `application-gateway rule update`
* <span data-ttu-id="a948f-2107">Adicionado suporte para `--accelerated-networking` a `nic create` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2107">Added support for `--accelerated-networking` to `nic create` and</span></span> `nic update`
* <span data-ttu-id="a948f-2108">Removido argumento `--internal-dns-name-suffix` de</span><span class="sxs-lookup"><span data-stu-id="a948f-2108">Removed `--internal-dns-name-suffix` argument from</span></span> `nic create`
* <span data-ttu-id="a948f-2109">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="a948f-2109">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="a948f-2110">Corrigido bug em que `local-gateway create` ignorava</span><span class="sxs-lookup"><span data-stu-id="a948f-2110">Fixed bug where `local-gateway create` ignored</span></span> `--local-address-prefixes`
* <span data-ttu-id="a948f-2111">Adição do suporte para `--dns-servers` a</span><span class="sxs-lookup"><span data-stu-id="a948f-2111">Added support for `--dns-servers` to</span></span> `vnet update`
* <span data-ttu-id="a948f-2112">Corrigido bug ao criar um emparelhamento sem filtragem de rotas com</span><span class="sxs-lookup"><span data-stu-id="a948f-2112">Fixed bug when creating a peering without route filtering with</span></span> `express-route peering create`
* <span data-ttu-id="a948f-2113">Corrigido bug em que os argumentos `--provider` e `--bandwidth` não funcionavam com</span><span class="sxs-lookup"><span data-stu-id="a948f-2113">Fixed bug where `--provider` and `--bandwidth` arguments did not work with</span></span> `express-route update`
* <span data-ttu-id="a948f-2114">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="a948f-2114">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="a948f-2115">Aprimorada a formatação de saída para</span><span class="sxs-lookup"><span data-stu-id="a948f-2115">Improved output formatting for</span></span> `network list-usages`
* <span data-ttu-id="a948f-2116">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="a948f-2116">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="a948f-2117">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="a948f-2117">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="a948f-2118">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="a948f-2118">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="a948f-2119">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="a948f-2119">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="a948f-2120">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-2120">Profile</span></span>

* <span data-ttu-id="a948f-2121">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="a948f-2121">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="a948f-2122">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="a948f-2122">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="a948f-2123">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="a948f-2123">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="a948f-2124">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="a948f-2124">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="a948f-2125">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="a948f-2125">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="a948f-2126">RDBMS</span><span class="sxs-lookup"><span data-stu-id="a948f-2126">RDBMS</span></span>

* <span data-ttu-id="a948f-2127">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="a948f-2127">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="a948f-2128">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="a948f-2128">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="a948f-2129">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="a948f-2129">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="a948f-2130">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="a948f-2130">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-2131">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-2131">Resource</span></span>

* <span data-ttu-id="a948f-2132">Aprimorados os prompts para parâmetros ausentes para</span><span class="sxs-lookup"><span data-stu-id="a948f-2132">Improved prompts for missing parameters for</span></span> `group deployment create`
* <span data-ttu-id="a948f-2133">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="a948f-2133">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="a948f-2134">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="a948f-2134">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="a948f-2135">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="a948f-2135">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="a948f-2136">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="a948f-2136">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="a948f-2137">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2137">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and</span></span> `<resource-type>`
* <span data-ttu-id="a948f-2138">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="a948f-2138">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="a948f-2139">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="a948f-2139">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="a948f-2140">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-2140">Role</span></span>

* <span data-ttu-id="a948f-2141">Suporte à saída no formato de arquivo de autenticação do SDK para</span><span class="sxs-lookup"><span data-stu-id="a948f-2141">Support output in SDK auth file format for</span></span> `create-for-rbac`
* <span data-ttu-id="a948f-2142">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="a948f-2142">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="a948f-2143">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="a948f-2143">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="a948f-2144">Mostrar avisos de reprovação ao usar</span><span class="sxs-lookup"><span data-stu-id="a948f-2144">Show deprecation warnings when using</span></span> `--expanded-view`
* <span data-ttu-id="a948f-2145">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="a948f-2145">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="a948f-2146">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a948f-2146">Service Fabric</span></span>
* <span data-ttu-id="a948f-2147">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="a948f-2147">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="a948f-2148">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="a948f-2148">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="a948f-2149">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="a948f-2149">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-2150">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-2150">SQL</span></span>

* <span data-ttu-id="a948f-2151">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="a948f-2151">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="a948f-2152">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="a948f-2152">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="a948f-2153">Adicionados comandos `sql db list-editions` e</span><span class="sxs-lookup"><span data-stu-id="a948f-2153">Added commands `sql db list-editions` and</span></span> `sql elastic-pool list-editions`

### <a name="storage"></a><span data-ttu-id="a948f-2154">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-2154">Storage</span></span>

* <span data-ttu-id="a948f-2155">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="a948f-2155">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="a948f-2156">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="a948f-2156">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="a948f-2157">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="a948f-2157">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="a948f-2158">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="a948f-2158">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="a948f-2159">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="a948f-2159">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="a948f-2160">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="a948f-2160">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-2161">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-2161">VM</span></span>

* <span data-ttu-id="a948f-2162">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="a948f-2162">Support configuring nsg</span></span>
* <span data-ttu-id="a948f-2163">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-2163">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="a948f-2164">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="a948f-2164">Support managed service identities</span></span>
* <span data-ttu-id="a948f-2165">Corrigido o problema em que `cmss create` com um balanceador de carga existente exigia</span><span class="sxs-lookup"><span data-stu-id="a948f-2165">Fixed issue where `cmss create` with an existing load balancer required</span></span> `--backend-pool-name`
* <span data-ttu-id="a948f-2166">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="a948f-2166">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="a948f-2167">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-2167">May 10, 2017</span></span>

<span data-ttu-id="a948f-2168">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="a948f-2168">Version 2.0.6</span></span>

* <span data-ttu-id="a948f-2169">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-2169">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="a948f-2170">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="a948f-2170">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="a948f-2171">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-2171">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="a948f-2172">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="a948f-2172">Include Cognitive Services module</span></span>
* <span data-ttu-id="a948f-2173">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a948f-2173">Include Service Fabric module</span></span>
* <span data-ttu-id="a948f-2174">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="a948f-2174">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="a948f-2175">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="a948f-2175">Add support for CDN commands</span></span>
* <span data-ttu-id="a948f-2176">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="a948f-2176">Remove Container module</span></span>
* <span data-ttu-id="a948f-2177">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="a948f-2177">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="a948f-2178">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a948f-2178">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="a948f-2179">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-2179">Core</span></span>

* <span data-ttu-id="a948f-2180">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="a948f-2180">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="a948f-2181">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="a948f-2181">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="a948f-2182">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="a948f-2182">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="a948f-2183">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="a948f-2183">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="a948f-2184">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="a948f-2184">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="a948f-2185">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="a948f-2185">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="a948f-2186">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="a948f-2186">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="a948f-2187">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="a948f-2187">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="a948f-2188">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="a948f-2188">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="a948f-2189">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="a948f-2189">core: Improved performance</span></span>
* <span data-ttu-id="a948f-2190">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="a948f-2190">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="a948f-2191">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="a948f-2191">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-2192">ACS</span></span>

* <span data-ttu-id="a948f-2193">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a948f-2193">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="a948f-2194">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="a948f-2194">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="a948f-2195">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="a948f-2195">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="a948f-2196">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="a948f-2196">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-2197">AppService</span></span>

* <span data-ttu-id="a948f-2198">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="a948f-2198">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="a948f-2199">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="a948f-2199">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="a948f-2200">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="a948f-2200">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="a948f-2201">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="a948f-2201">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="a948f-2202">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="a948f-2202">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="a948f-2203">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="a948f-2203">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="a948f-2204">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="a948f-2204">support slot swap with preview</span></span>
* <span data-ttu-id="a948f-2205">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="a948f-2205">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="a948f-2206">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="a948f-2206">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="a948f-2207">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-2207">CosmosDB</span></span>

* <span data-ttu-id="a948f-2208">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="a948f-2208">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="a948f-2209">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="a948f-2209">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="a948f-2210">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="a948f-2210">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="a948f-2211">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="a948f-2211">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="a948f-2212">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a948f-2212">Data Lake Analytics</span></span>

* <span data-ttu-id="a948f-2213">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="a948f-2213">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="a948f-2214">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="a948f-2214">Add support for new catalog item type: package.</span></span> <span data-ttu-id="a948f-2215">acessado por meio de:</span><span class="sxs-lookup"><span data-stu-id="a948f-2215">accessed through:</span></span> `az dla catalog package`
* <span data-ttu-id="a948f-2216">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="a948f-2216">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="a948f-2217">Tabela</span><span class="sxs-lookup"><span data-stu-id="a948f-2217">Table</span></span>
  * <span data-ttu-id="a948f-2218">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="a948f-2218">Table valued function</span></span>
  * <span data-ttu-id="a948f-2219">Visualizar</span><span class="sxs-lookup"><span data-stu-id="a948f-2219">View</span></span>
  * <span data-ttu-id="a948f-2220">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="a948f-2220">Table Statistics.</span></span> <span data-ttu-id="a948f-2221">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="a948f-2221">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="a948f-2222">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-2222">Data Lake Store</span></span>

* <span data-ttu-id="a948f-2223">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="a948f-2223">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="a948f-2224">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="a948f-2224">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="a948f-2225">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="a948f-2225">missed help for access show.</span></span> <span data-ttu-id="a948f-2226">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="a948f-2226">adding it.</span></span> <span data-ttu-id="a948f-2227">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="a948f-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="a948f-2228">Localizar</span><span class="sxs-lookup"><span data-stu-id="a948f-2228">Find</span></span>

* <span data-ttu-id="a948f-2229">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="a948f-2229">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="a948f-2230">KeyVault</span><span class="sxs-lookup"><span data-stu-id="a948f-2230">KeyVault</span></span>

* <span data-ttu-id="a948f-2231">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="a948f-2231">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="a948f-2232">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="a948f-2232">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="a948f-2233">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="a948f-2233">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="a948f-2234">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="a948f-2234">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="a948f-2235">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="a948f-2235">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="a948f-2236">Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2236">Lab</span></span>

* <span data-ttu-id="a948f-2237">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2237">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="a948f-2238">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2238">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="a948f-2239">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2239">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="a948f-2240">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2240">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="a948f-2241">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="a948f-2241">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="a948f-2242">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="a948f-2242">Monitor</span></span>

* <span data-ttu-id="a948f-2243">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="a948f-2243">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="a948f-2244">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="a948f-2244">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="a948f-2245">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-2245">Network</span></span>

* <span data-ttu-id="a948f-2246">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="a948f-2246">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="a948f-2247">Adição de suporte para o parâmetro `--filters` de</span><span class="sxs-lookup"><span data-stu-id="a948f-2247">Add support for `--filters` parameter for</span></span> `network watcher packet-capture create`
* <span data-ttu-id="a948f-2248">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-2248">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="a948f-2249">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a948f-2249">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="a948f-2250">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="a948f-2250">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="a948f-2251">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="a948f-2251">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="a948f-2252">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="a948f-2252">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="a948f-2253">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="a948f-2253">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="a948f-2254">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="a948f-2254">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="a948f-2255">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="a948f-2255">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="a948f-2256">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="a948f-2256">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="a948f-2257">BC: Corrigido bug na saída de</span><span class="sxs-lookup"><span data-stu-id="a948f-2257">BC: Fix bug in the output of</span></span> `vpn-connection create`
* <span data-ttu-id="a948f-2258">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-2258">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="a948f-2259">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="a948f-2259">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="a948f-2260">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="a948f-2260">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="a948f-2261">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="a948f-2261">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="a948f-2262">Perfil</span><span class="sxs-lookup"><span data-stu-id="a948f-2262">Profile</span></span>

* <span data-ttu-id="a948f-2263">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="a948f-2263">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="a948f-2264">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="a948f-2264">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="a948f-2265">Redis</span><span class="sxs-lookup"><span data-stu-id="a948f-2265">Redis</span></span>

* <span data-ttu-id="a948f-2266">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="a948f-2266">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="a948f-2267">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="a948f-2267">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="a948f-2268">Recurso</span><span class="sxs-lookup"><span data-stu-id="a948f-2268">Resource</span></span>

* <span data-ttu-id="a948f-2269">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="a948f-2269">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="a948f-2270">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="a948f-2270">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="a948f-2271">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="a948f-2271">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="a948f-2272">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="a948f-2272">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="a948f-2273">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="a948f-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="a948f-2274">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="a948f-2274">Add docs for az lock update.</span></span> <span data-ttu-id="a948f-2275">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="a948f-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="a948f-2276">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="a948f-2276">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="a948f-2277">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="a948f-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="a948f-2278">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="a948f-2278">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="a948f-2279">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="a948f-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="a948f-2280">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="a948f-2280">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="a948f-2281">Função</span><span class="sxs-lookup"><span data-stu-id="a948f-2281">Role</span></span>

* <span data-ttu-id="a948f-2282">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="a948f-2282">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="a948f-2283">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="a948f-2283">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="a948f-2284">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="a948f-2284">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="a948f-2285">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="a948f-2285">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="a948f-2286">SQL</span><span class="sxs-lookup"><span data-stu-id="a948f-2286">SQL</span></span>

* <span data-ttu-id="a948f-2287">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="a948f-2287">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="a948f-2288">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="a948f-2288">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="a948f-2289">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-2289">Storage</span></span>

* <span data-ttu-id="a948f-2290">Localização padrão da localização do grupo de recursos de</span><span class="sxs-lookup"><span data-stu-id="a948f-2290">Default location to resource group location for</span></span> `storage account create`
* <span data-ttu-id="a948f-2291">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="a948f-2291">Add support for incremental blob copy</span></span>
* <span data-ttu-id="a948f-2292">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="a948f-2292">Add support for large block blob upload</span></span>
* <span data-ttu-id="a948f-2293">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="a948f-2293">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-2294">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-2294">VM</span></span>

* <span data-ttu-id="a948f-2295">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="a948f-2295">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="a948f-2296">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="a948f-2296">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="a948f-2297">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="a948f-2297">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="a948f-2298">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="a948f-2298">az vm/vmss disk</span></span>
  3. <span data-ttu-id="a948f-2299">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="a948f-2299">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="a948f-2300">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="a948f-2300">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="a948f-2301">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="a948f-2301">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="a948f-2302">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-2302">April 3, 2017</span></span>

<span data-ttu-id="a948f-2303">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="a948f-2303">Version 2.0.2</span></span>

<span data-ttu-id="a948f-2304">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="a948f-2304">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="a948f-2305">Núcleo</span><span class="sxs-lookup"><span data-stu-id="a948f-2305">Core</span></span>

* <span data-ttu-id="a948f-2306">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-2306">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="a948f-2307">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="a948f-2307">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="a948f-2308">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="a948f-2308">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="a948f-2309">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a948f-2309">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a948f-2310">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="a948f-2310">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="a948f-2311">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="a948f-2311">Add prompting for missing template parameters.</span></span> <span data-ttu-id="a948f-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="a948f-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="a948f-2313">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="a948f-2313">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="a948f-2314">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="a948f-2314">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="a948f-2315">ACS</span><span class="sxs-lookup"><span data-stu-id="a948f-2315">ACS</span></span>

* <span data-ttu-id="a948f-2316">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="a948f-2316">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="a948f-2317">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="a948f-2317">Add support for ssh key password prompting.</span></span> <span data-ttu-id="a948f-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="a948f-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="a948f-2319">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="a948f-2319">Add support for windows clusters.</span></span> <span data-ttu-id="a948f-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="a948f-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="a948f-2321">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="a948f-2321">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="a948f-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="a948f-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="a948f-2323">AppService</span><span class="sxs-lookup"><span data-stu-id="a948f-2323">AppService</span></span>

* <span data-ttu-id="a948f-2324">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="a948f-2324">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="a948f-2325">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="a948f-2325">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="a948f-2326">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="a948f-2326">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="a948f-2327">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="a948f-2327">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="a948f-2328">DataLake</span><span class="sxs-lookup"><span data-stu-id="a948f-2328">DataLake</span></span>

* <span data-ttu-id="a948f-2329">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="a948f-2329">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="a948f-2330">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="a948f-2330">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="a948f-2331">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="a948f-2331">DocuemntDB</span></span>

* <span data-ttu-id="a948f-2332">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="a948f-2332">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="a948f-2333">VM</span><span class="sxs-lookup"><span data-stu-id="a948f-2333">VM</span></span>

* <span data-ttu-id="a948f-2334">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="a948f-2334">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="a948f-2335">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="a948f-2335">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="a948f-2336">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="a948f-2336">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="a948f-2337">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="a948f-2337">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="a948f-2338">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="a948f-2338">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="a948f-2339">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="a948f-2339">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="a948f-2340">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="a948f-2340">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="a948f-2341">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="a948f-2341">February 27, 2017</span></span>

<span data-ttu-id="a948f-2342">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="a948f-2342">Version 2.0.0</span></span>

<span data-ttu-id="a948f-2343">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="a948f-2343">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="a948f-2344">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="a948f-2344">Container Service (acs)</span></span>
- <span data-ttu-id="a948f-2345">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="a948f-2345">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="a948f-2346">Rede</span><span class="sxs-lookup"><span data-stu-id="a948f-2346">Networking</span></span>
- <span data-ttu-id="a948f-2347">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="a948f-2347">Storage</span></span>

<span data-ttu-id="a948f-2348">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="a948f-2348">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="a948f-2349">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="a948f-2349">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="a948f-2350">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="a948f-2350">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="a948f-2351">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="a948f-2351">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="a948f-2352">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="a948f-2352">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="a948f-2353">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="a948f-2353">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="a948f-2354">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="a948f-2354">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="a948f-2355">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="a948f-2355">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="a948f-2356">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="a948f-2356">Provide feedback from the command line with the `az feedback` command</span></span>

