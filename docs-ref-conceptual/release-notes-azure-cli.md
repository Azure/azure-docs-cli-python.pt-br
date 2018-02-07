---
title: "Notas de versão da CLI do Azure 2.0"
description: "Saiba mais sobre as últimas atualizações da CLI do Azure 2.0"
keywords: "Notas da versão, CLI do Azure 2.0"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/17/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 86babea3030ea932de1858a391014e5d0bba7f73
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="5f3a4-104">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="5f3a4-104">Azure CLI 2.0 release notes</span></span>

## <a name="january-17-2018"></a><span data-ttu-id="5f3a4-105">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="5f3a4-105">January 17, 2018</span></span>

<span data-ttu-id="5f3a4-106">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="5f3a4-106">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="5f3a4-107">ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-107">ACR</span></span>

* <span data-ttu-id="5f3a4-108">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="5f3a4-108">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="5f3a4-109">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="5f3a4-109">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-110">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-110">ACS</span></span>

* <span data-ttu-id="5f3a4-111">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-111">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="5f3a4-112">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="5f3a4-112">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-113">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-113">Appservice</span></span>

* <span data-ttu-id="5f3a4-114">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-114">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="5f3a4-115">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-115">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="5f3a4-116">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-116">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="5f3a4-117">Backup</span><span class="sxs-lookup"><span data-stu-id="5f3a4-117">Backup</span></span>

* <span data-ttu-id="5f3a4-118">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="5f3a4-118">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="5f3a4-119">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-119">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="5f3a4-120">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-120">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="5f3a4-121">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="5f3a4-121">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="5f3a4-122">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-122">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="5f3a4-123">Batch</span><span class="sxs-lookup"><span data-stu-id="5f3a4-123">Batch</span></span>

* <span data-ttu-id="5f3a4-124">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="5f3a4-124">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="5f3a4-125">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-125">Cloud</span></span>

* <span data-ttu-id="5f3a4-126">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-126">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="5f3a4-127">Consumo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-127">Consumption</span></span>

* <span data-ttu-id="5f3a4-128">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-128">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f3a4-129">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-129">Event Grid</span></span>

* <span data-ttu-id="5f3a4-130">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid topic event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-130">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f3a4-131">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid resource event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-131">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="5f3a4-132">[ALTERAÇÃO SIGNIFICATIVA] Removido o comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-132">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="5f3a4-133">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-133">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="5f3a4-134">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-134">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="5f3a4-135">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-135">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="5f3a4-136">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-136">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="5f3a4-137">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-137">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="5f3a4-138">Interativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-138">Interactive</span></span>

* <span data-ttu-id="5f3a4-139">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="5f3a4-139">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="5f3a4-140">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="5f3a4-140">Fixed errors on startup</span></span>
* <span data-ttu-id="5f3a4-141">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-141">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="5f3a4-142">IoT</span><span class="sxs-lookup"><span data-stu-id="5f3a4-142">IoT</span></span>

* <span data-ttu-id="5f3a4-143">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-143">Added support for device provisioning service</span></span>
* <span data-ttu-id="5f3a4-144">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="5f3a4-144">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="5f3a4-145">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="5f3a4-145">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-146">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-146">Monitor</span></span>

* <span data-ttu-id="5f3a4-147">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-147">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="5f3a4-148">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-148">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="5f3a4-149">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-149">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span> 

### <a name="network"></a><span data-ttu-id="5f3a4-150">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-150">Network</span></span>

* <span data-ttu-id="5f3a4-151">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-151">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="5f3a4-152">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-152">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="5f3a4-153">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f3a4-153">Profile</span></span>

* <span data-ttu-id="5f3a4-154">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="5f3a4-154">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="5f3a4-155">Função</span><span class="sxs-lookup"><span data-stu-id="5f3a4-155">Role</span></span>

* <span data-ttu-id="5f3a4-156">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-156">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f3a4-157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f3a4-157">Service Fabric</span></span>

* <span data-ttu-id="5f3a4-158">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="5f3a4-158">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="5f3a4-159">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-159">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-160">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-160">VM</span></span>

* <span data-ttu-id="5f3a4-161">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-161">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="5f3a4-162">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="5f3a4-162">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="5f3a4-163">[ALTERAÇÃO SIGNIFICATIVA] Alterado `externalIdentities` para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="5f3a4-163">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="5f3a4-164">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="5f3a4-164">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="5f3a4-165">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-165">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="5f3a4-166">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-166">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f3a4-167">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-167">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f3a4-168">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-168">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="5f3a4-169">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-169">December 19, 2017</span></span>

<span data-ttu-id="5f3a4-170">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="5f3a4-170">Version 2.0.23</span></span>

* <span data-ttu-id="5f3a4-171">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="5f3a4-171">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="5f3a4-172">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-172">Container</span></span>

* <span data-ttu-id="5f3a4-173">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-173">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-174">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-174">Network</span></span>

* <span data-ttu-id="5f3a4-175">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-175">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="5f3a4-176">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-176">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-177">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-177">Storage</span></span>

* <span data-ttu-id="5f3a4-178">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="5f3a4-178">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-179">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-179">VM</span></span>

* <span data-ttu-id="5f3a4-180">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-180">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="5f3a4-181">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-181">December 5, 2017</span></span>

<span data-ttu-id="5f3a4-182">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="5f3a4-182">Version 2.0.22</span></span>

* <span data-ttu-id="5f3a4-183">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-183">Removed `az component` commands.</span></span> <span data-ttu-id="5f3a4-184">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-184">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="5f3a4-185">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-185">Core</span></span>
* <span data-ttu-id="5f3a4-186">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="5f3a4-186">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="5f3a4-187">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-187">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-188">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-188">ACS</span></span>

* <span data-ttu-id="5f3a4-189">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-189">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="5f3a4-190">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-190">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="5f3a4-191">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-191">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="5f3a4-192">Supervisor</span><span class="sxs-lookup"><span data-stu-id="5f3a4-192">Advisor</span></span>

* <span data-ttu-id="5f3a4-193">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5f3a4-193">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-194">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-194">Appservice</span></span>

* <span data-ttu-id="5f3a4-195">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-195">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="5f3a4-196">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-196">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="5f3a4-197">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-197">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="5f3a4-198">Consumo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-198">Consumption</span></span>

* <span data-ttu-id="5f3a4-199">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-199">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="5f3a4-200">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-200">Container</span></span>

* <span data-ttu-id="5f3a4-201">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-201">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-202">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-202">Monitor</span></span>

* <span data-ttu-id="5f3a4-203">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-203">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-204">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-204">Resource</span></span>

* <span data-ttu-id="5f3a4-205">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-205">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="5f3a4-206">Função</span><span class="sxs-lookup"><span data-stu-id="5f3a4-206">Role</span></span>

* <span data-ttu-id="5f3a4-207">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-207">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="5f3a4-208">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="5f3a4-208">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="5f3a4-209">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-209">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-210">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-210">SQL</span></span>

* <span data-ttu-id="5f3a4-211">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-211">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="5f3a4-212">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-212">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-213">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-213">VM</span></span>

* <span data-ttu-id="5f3a4-214">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-214">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="5f3a4-215">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-215">November 14, 2017</span></span>

<span data-ttu-id="5f3a4-216">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="5f3a4-216">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="5f3a4-217">ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-217">ACR</span></span>

* <span data-ttu-id="5f3a4-218">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="5f3a4-218">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="5f3a4-219">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-219">ACS</span></span>

* <span data-ttu-id="5f3a4-220">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-220">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="5f3a4-221">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-221">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="5f3a4-222">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-222">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="5f3a4-223">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="5f3a4-223">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="5f3a4-224">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="5f3a4-224">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-225">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-225">Appservice</span></span>

* <span data-ttu-id="5f3a4-226">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="5f3a4-226">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="5f3a4-227">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-227">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="5f3a4-228">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-228">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="5f3a4-229">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-229">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="5f3a4-230">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="5f3a4-230">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="5f3a4-231">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-231">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="5f3a4-232">Batch</span><span class="sxs-lookup"><span data-stu-id="5f3a4-232">Batch</span></span>

* <span data-ttu-id="5f3a4-233">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-233">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="5f3a4-234">Batchai</span><span class="sxs-lookup"><span data-stu-id="5f3a4-234">Batchai</span></span>

* <span data-ttu-id="5f3a4-235">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-235">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="5f3a4-236">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-236">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="5f3a4-237">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-237">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="5f3a4-238">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-238">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="5f3a4-239">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-239">Cloud</span></span>

* <span data-ttu-id="5f3a4-240">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="5f3a4-240">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="5f3a4-241">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-241">Container</span></span>

* <span data-ttu-id="5f3a4-242">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-242">Added support to open multiple ports</span></span>
* <span data-ttu-id="5f3a4-243">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-243">Added container group restart policy</span></span>
* <span data-ttu-id="5f3a4-244">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="5f3a4-244">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="5f3a4-245">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-245">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f3a4-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f3a4-246">Data Lake Analytics</span></span>

* <span data-ttu-id="5f3a4-247">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-247">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f3a4-248">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f3a4-248">Data Lake Store</span></span>

* <span data-ttu-id="5f3a4-249">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-249">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="5f3a4-250">Extensão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-250">Extension</span></span>

* <span data-ttu-id="5f3a4-251">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="5f3a4-251">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="5f3a4-252">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="5f3a4-252">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="5f3a4-253">IoT</span><span class="sxs-lookup"><span data-stu-id="5f3a4-253">IoT</span></span>

* <span data-ttu-id="5f3a4-254">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-254">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-255">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-255">Monitor</span></span>

* <span data-ttu-id="5f3a4-256">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-256">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-257">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-257">Network</span></span>

* <span data-ttu-id="5f3a4-258">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="5f3a4-258">Added support for CAA DNS records</span></span>
* <span data-ttu-id="5f3a4-259">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-259">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="5f3a4-260">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-260">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="5f3a4-261">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-261">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="5f3a4-262">Reservas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-262">Reservations</span></span>

* <span data-ttu-id="5f3a4-263">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="5f3a4-263">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-264">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-264">Resource</span></span>

* <span data-ttu-id="5f3a4-265">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-265">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-266">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-266">SQL</span></span>

* <span data-ttu-id="5f3a4-267">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-267">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-268">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-268">Storage</span></span>

* <span data-ttu-id="5f3a4-269">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-269">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="5f3a4-270">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="5f3a4-270">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="5f3a4-271">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-271">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="5f3a4-272">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-272">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="5f3a4-273">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-273">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="5f3a4-274">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-274">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="5f3a4-275">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-275">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-276">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-276">VM</span></span>

* <span data-ttu-id="5f3a4-277">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-277">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="5f3a4-278">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="5f3a4-278">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="5f3a4-279">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-279">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="5f3a4-280">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-280">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="5f3a4-281">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-281">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="5f3a4-282">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-282">October 24, 2017</span></span>

<span data-ttu-id="5f3a4-283">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="5f3a4-283">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="5f3a4-284">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-284">Core</span></span>

* <span data-ttu-id="5f3a4-285">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-285">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="5f3a4-286">ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-286">ACR</span></span>

* <span data-ttu-id="5f3a4-287">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-287">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="5f3a4-288">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-288">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="5f3a4-289">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="5f3a4-289">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-290">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-290">ACS</span></span>

* <span data-ttu-id="5f3a4-291">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-291">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="5f3a4-292">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="5f3a4-292">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-293">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-293">Appservice</span></span>

* <span data-ttu-id="5f3a4-294">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-294">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="5f3a4-295">Componente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-295">Component</span></span>

* <span data-ttu-id="5f3a4-296">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="5f3a4-296">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-297">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-297">Monitor</span></span>

* <span data-ttu-id="5f3a4-298">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-298">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-299">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-299">Resource</span></span>

* <span data-ttu-id="5f3a4-300">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-300">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="5f3a4-301">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-301">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-302">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-302">VM</span></span>

* <span data-ttu-id="5f3a4-303">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-303">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="5f3a4-304">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-304">October 9, 2017</span></span>

<span data-ttu-id="5f3a4-305">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="5f3a4-305">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="5f3a4-306">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-306">Core</span></span>

* <span data-ttu-id="5f3a4-307">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5f3a4-307">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-308">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-308">Appservice</span></span>

* <span data-ttu-id="5f3a4-309">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-309">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="5f3a4-310">Batch</span><span class="sxs-lookup"><span data-stu-id="5f3a4-310">Batch</span></span>

* <span data-ttu-id="5f3a4-311">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="5f3a4-311">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="5f3a4-312">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="5f3a4-312">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="5f3a4-313">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="5f3a4-313">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="5f3a4-314">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-314">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="5f3a4-315">Batchai</span><span class="sxs-lookup"><span data-stu-id="5f3a4-315">Batchai</span></span>

* <span data-ttu-id="5f3a4-316">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="5f3a4-316">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f3a4-317">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f3a4-317">Keyvault</span></span>

* <span data-ttu-id="5f3a4-318">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-318">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="5f3a4-319">(#4448)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-319">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="5f3a4-320">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-320">Network</span></span>

* <span data-ttu-id="5f3a4-321">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="5f3a4-321">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="5f3a4-322">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-322">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-323">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-323">Resource</span></span>

* <span data-ttu-id="5f3a4-324">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-324">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="5f3a4-325">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="5f3a4-325">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="5f3a4-326">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-326">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="5f3a4-327">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-327">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-328">Sql</span><span class="sxs-lookup"><span data-stu-id="5f3a4-328">Sql</span></span>

* <span data-ttu-id="5f3a4-329">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="5f3a4-329">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="5f3a4-330">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-330">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="5f3a4-331">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-331">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-332">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-332">Storage</span></span>

* <span data-ttu-id="5f3a4-333">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-333">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-334">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-334">Vm</span></span>

* <span data-ttu-id="5f3a4-335">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-335">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="5f3a4-336">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-336">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="5f3a4-337">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-337">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="5f3a4-338">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-338">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="5f3a4-339">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-339">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="5f3a4-340">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-340">September 22, 2017</span></span>

<span data-ttu-id="5f3a4-341">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="5f3a4-341">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-342">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-342">Resource</span></span>

* <span data-ttu-id="5f3a4-343">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-343">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="5f3a4-344">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="5f3a4-344">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="5f3a4-345">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-345">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="5f3a4-346">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-346">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-347">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-347">Network</span></span>

* <span data-ttu-id="5f3a4-348">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-348">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="5f3a4-349">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-349">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="5f3a4-350">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-350">Added `asg` application security group commands</span></span>
* <span data-ttu-id="5f3a4-351">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-351">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="5f3a4-352">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-352">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f3a4-353">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-353">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="5f3a4-354">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-354">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-355">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-355">Storage</span></span>

* <span data-ttu-id="5f3a4-356">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="5f3a4-356">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="5f3a4-357">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-357">Eventgrid</span></span>

* <span data-ttu-id="5f3a4-358">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="5f3a4-358">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-359">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-359">SQL</span></span>

* <span data-ttu-id="5f3a4-360">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-360">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="5f3a4-361">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-361">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="5f3a4-362">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-362">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f3a4-363">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f3a4-363">Keyvault</span></span>

* <span data-ttu-id="5f3a4-364">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="5f3a4-364">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-365">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-365">VM</span></span>

* <span data-ttu-id="5f3a4-366">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-366">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="5f3a4-367">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="5f3a4-367">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="5f3a4-368">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-368">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="5f3a4-369">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-369">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="5f3a4-370">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-370">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="5f3a4-371">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-371">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-372">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-372">ACS</span></span>

* <span data-ttu-id="5f3a4-373">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-373">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-374">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-374">Appservice</span></span>

* <span data-ttu-id="5f3a4-375">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-375">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="5f3a4-376">Backup</span><span class="sxs-lookup"><span data-stu-id="5f3a4-376">Backup</span></span>

* <span data-ttu-id="5f3a4-377">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5f3a4-377">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="5f3a4-378">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-378">September 11, 2017</span></span>

<span data-ttu-id="5f3a4-379">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="5f3a4-379">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="5f3a4-380">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-380">Core</span></span>

* <span data-ttu-id="5f3a4-381">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="5f3a4-381">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="5f3a4-382">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-382">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-383">Acs</span><span class="sxs-lookup"><span data-stu-id="5f3a4-383">Acs</span></span>

* <span data-ttu-id="5f3a4-384">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-384">Added `acs list-locations` command</span></span>
* <span data-ttu-id="5f3a4-385">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-385">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-386">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-386">Appservice</span></span>

* <span data-ttu-id="5f3a4-387">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-387">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="5f3a4-388">CDN</span><span class="sxs-lookup"><span data-stu-id="5f3a4-388">CDN</span></span>

* <span data-ttu-id="5f3a4-389">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-389">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="5f3a4-390">Extensão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-390">Extension</span></span>

* <span data-ttu-id="5f3a4-391">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-391">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f3a4-392">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f3a4-392">Keyvault</span></span>

* <span data-ttu-id="5f3a4-393">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-393">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-394">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-394">Network</span></span>

* <span data-ttu-id="5f3a4-395">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-395">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f3a4-396">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-396">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="5f3a4-397">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-397">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="5f3a4-398">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-398">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f3a4-399">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-399">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-400">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-400">Resource</span></span>

* <span data-ttu-id="5f3a4-401">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-401">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="5f3a4-402">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-402">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="5f3a4-403">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="5f3a4-403">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="5f3a4-404">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-404">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-405">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-405">SQL</span></span>

* <span data-ttu-id="5f3a4-406">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-406">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-407">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-407">VM</span></span>

* <span data-ttu-id="5f3a4-408">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="5f3a4-408">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="5f3a4-409">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="5f3a4-409">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="5f3a4-410">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-410">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="5f3a4-411">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-411">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="5f3a4-412">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="5f3a4-412">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="5f3a4-413">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-413">August 31, 2017</span></span>

<span data-ttu-id="5f3a4-414">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="5f3a4-414">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f3a4-415">Keyvault</span><span class="sxs-lookup"><span data-stu-id="5f3a4-415">Keyvault</span></span>

* <span data-ttu-id="5f3a4-416">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-416">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="5f3a4-417">Sf</span><span class="sxs-lookup"><span data-stu-id="5f3a4-417">Sf</span></span>

* <span data-ttu-id="5f3a4-418">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-418">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-419">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-419">Storage</span></span>

* <span data-ttu-id="5f3a4-420">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="5f3a4-420">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="5f3a4-421">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-421">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="5f3a4-422">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-422">August 28, 2017</span></span>

<span data-ttu-id="5f3a4-423">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="5f3a4-423">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="5f3a4-424">CLI</span><span class="sxs-lookup"><span data-stu-id="5f3a4-424">CLI</span></span>

* <span data-ttu-id="5f3a4-425">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-425">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-426">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-426">ACS</span></span>

* <span data-ttu-id="5f3a4-427">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-427">Corrected preview regions.</span></span>
* <span data-ttu-id="5f3a4-428">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-428">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="5f3a4-429">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-429">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-430">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-430">Appservice</span></span>

* <span data-ttu-id="5f3a4-431">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-431">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="5f3a4-432">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-432">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="5f3a4-433">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-433">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="5f3a4-434">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-434">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="5f3a4-435">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-435">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="5f3a4-436">IoT</span><span class="sxs-lookup"><span data-stu-id="5f3a4-436">IoT</span></span>

* <span data-ttu-id="5f3a4-437">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-437">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-438">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-438">Network</span></span>

* <span data-ttu-id="5f3a4-439">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-439">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="5f3a4-440">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-440">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="5f3a4-441">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-441">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="5f3a4-442">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-442">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="5f3a4-443">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-443">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="5f3a4-444">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f3a4-444">Profile</span></span>

* <span data-ttu-id="5f3a4-445">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="5f3a4-445">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f3a4-446">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f3a4-446">Service Fabric</span></span>

* <span data-ttu-id="5f3a4-447">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="5f3a4-447">Preview release</span></span>
* <span data-ttu-id="5f3a4-448">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="5f3a4-448">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="5f3a4-449">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="5f3a4-449">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="5f3a4-450">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="5f3a4-450">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-451">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-451">Storage</span></span>

* <span data-ttu-id="5f3a4-452">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="5f3a4-452">Enabled setting blob tier</span></span>
* <span data-ttu-id="5f3a4-453">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="5f3a4-453">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="5f3a4-454">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="5f3a4-454">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="5f3a4-455">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-455">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="5f3a4-456">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-456">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="5f3a4-457">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="5f3a4-457">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-458">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-458">VM</span></span>

* <span data-ttu-id="5f3a4-459">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-459">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="5f3a4-460">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-460">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="5f3a4-461">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-461">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="5f3a4-462">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-462">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="5f3a4-463">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="5f3a4-463">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="5f3a4-464">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-464">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="5f3a4-465">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-465">August 15, 2017</span></span>

<span data-ttu-id="5f3a4-466">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="5f3a4-466">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-467">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-467">ACS</span></span>

* <span data-ttu-id="5f3a4-468">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-468">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-469">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-469">Appservice</span></span>

* <span data-ttu-id="5f3a4-470">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="5f3a4-470">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f3a4-471">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-471">Event Grid</span></span>

* <span data-ttu-id="5f3a4-472">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="5f3a4-472">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="5f3a4-473">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-473">August 11, 2017</span></span>

<span data-ttu-id="5f3a4-474">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="5f3a4-474">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-475">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-475">ACS</span></span>

* <span data-ttu-id="5f3a4-476">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="5f3a4-476">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="5f3a4-477">Batch</span><span class="sxs-lookup"><span data-stu-id="5f3a4-477">Batch</span></span>

* <span data-ttu-id="5f3a4-478">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="5f3a4-478">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="5f3a4-479">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="5f3a4-479">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="5f3a4-480">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-480">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="5f3a4-481">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="5f3a4-481">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="5f3a4-482">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="5f3a4-482">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="5f3a4-483">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="5f3a4-483">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="5f3a4-484">Componente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-484">Component</span></span>

* <span data-ttu-id="5f3a4-485">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="5f3a4-485">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="5f3a4-486">Contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-486">Container</span></span>

* <span data-ttu-id="5f3a4-487">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-487">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="5f3a4-488">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f3a4-488">Data Lake Store</span></span>

* <span data-ttu-id="5f3a4-489">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-489">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="5f3a4-490">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-490">Event Grid</span></span>

* <span data-ttu-id="5f3a4-491">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="5f3a4-491">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-492">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-492">Network</span></span>

* <span data-ttu-id="5f3a4-493">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-493">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="5f3a4-494">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-494">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="5f3a4-495">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-495">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="5f3a4-496">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-496">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="5f3a4-497">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f3a4-497">Profile</span></span>

* <span data-ttu-id="5f3a4-498">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="5f3a4-498">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-499">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-499">Storage</span></span>

* <span data-ttu-id="5f3a4-500">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="5f3a4-500">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-501">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-501">VM</span></span>

* <span data-ttu-id="5f3a4-502">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-502">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="5f3a4-503">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-503">Exposed `list-skus` command</span></span>
* <span data-ttu-id="5f3a4-504">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="5f3a4-504">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="5f3a4-505">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-505">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="5f3a4-506">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-506">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="5f3a4-507">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-507">July 28, 2017</span></span>

<span data-ttu-id="5f3a4-508">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="5f3a4-508">Version 2.0.12</span></span>

* <span data-ttu-id="5f3a4-509">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="5f3a4-509">Added container commands</span></span>
* <span data-ttu-id="5f3a4-510">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-510">Added billing and consumption modules</span></span>

```
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

### <a name="core"></a><span data-ttu-id="5f3a4-511">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-511">Core</span></span>

* <span data-ttu-id="5f3a4-512">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-512">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="5f3a4-513">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="5f3a4-513">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="5f3a4-514">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="5f3a4-514">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="5f3a4-515">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-515">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="5f3a4-516">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="5f3a4-516">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="5f3a4-517">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-517">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="5f3a4-518">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-518">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f3a4-519">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-519">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="5f3a4-520">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-520">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="5f3a4-521">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="5f3a4-521">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="5f3a4-522">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-522">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="5f3a4-523">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-523">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="5f3a4-524">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-524">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="5f3a4-525">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="5f3a4-525">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="5f3a4-526">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5f3a4-526">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="5f3a4-527">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-527">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="5f3a4-528">ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-528">ACR</span></span>

* <span data-ttu-id="5f3a4-529">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-529">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="5f3a4-530">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-530">Support SKU update for managed registries</span></span>
* <span data-ttu-id="5f3a4-531">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-531">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="5f3a4-532">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-532">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="5f3a4-533">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-533">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="5f3a4-534">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="5f3a4-534">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-535">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-535">ACS</span></span>

* <span data-ttu-id="5f3a4-536">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="5f3a4-536">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-537">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-537">Appservice</span></span>

* <span data-ttu-id="5f3a4-538">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-538">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="5f3a4-539">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="5f3a4-539">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="5f3a4-540">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-540">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="5f3a4-541">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-541">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="5f3a4-542">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-542">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="5f3a4-543">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-543">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="5f3a4-544">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-544">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="5f3a4-545">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-545">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="5f3a4-546">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-546">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="5f3a4-547">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-547">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="5f3a4-548">Batch</span><span class="sxs-lookup"><span data-stu-id="5f3a4-548">Batch</span></span>

* <span data-ttu-id="5f3a4-549">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="5f3a4-549">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="5f3a4-550">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-550">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="5f3a4-551">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-551">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="5f3a4-552">CDN</span><span class="sxs-lookup"><span data-stu-id="5f3a4-552">CDN</span></span>

* <span data-ttu-id="5f3a4-553">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-553">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="5f3a4-554">Nuvem</span><span class="sxs-lookup"><span data-stu-id="5f3a4-554">Cloud</span></span>

* <span data-ttu-id="5f3a4-555">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="5f3a4-555">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="5f3a4-556">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="5f3a4-556">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="5f3a4-557">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-557">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="5f3a4-558">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="5f3a4-558">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="5f3a4-559">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-559">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f3a4-560">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f3a4-560">CosmosDB</span></span>

* <span data-ttu-id="5f3a4-561">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-561">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="5f3a4-562">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-562">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f3a4-563">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f3a4-563">Data Lake Analytics</span></span>

* <span data-ttu-id="5f3a4-564">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-564">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="5f3a4-565">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-565">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="5f3a4-566">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-566">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f3a4-567">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f3a4-567">Data Lake Store</span></span>

* <span data-ttu-id="5f3a4-568">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-568">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="5f3a4-569">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="5f3a4-569">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="5f3a4-570">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-570">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="5f3a4-571">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="5f3a4-571">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="5f3a4-572">Interativo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-572">Interactive</span></span>

* <span data-ttu-id="5f3a4-573">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="5f3a4-573">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="5f3a4-574">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="5f3a4-574">Increased test coverage</span></span>
* <span data-ttu-id="5f3a4-575">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="5f3a4-575">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="5f3a4-576">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-576">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="5f3a4-577">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-577">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="5f3a4-578">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-578">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="5f3a4-579">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-579">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="5f3a4-580">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-580">Added `--progress` flag</span></span>
* <span data-ttu-id="5f3a4-581">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="5f3a4-581">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="5f3a4-582">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-582">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="5f3a4-583">IoT</span><span class="sxs-lookup"><span data-stu-id="5f3a4-583">IoT</span></span>

* <span data-ttu-id="5f3a4-584">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-584">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="5f3a4-585">(#3934)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-585">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="5f3a4-586">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="5f3a4-586">Key vault</span></span>

* <span data-ttu-id="5f3a4-587">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-587">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="5f3a4-588">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-588">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="5f3a4-589">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-589">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f3a4-590">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-590">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="5f3a4-591">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-591">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="5f3a4-592">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-592">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="5f3a4-593">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-593">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="5f3a4-594">(#3307)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-594">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="5f3a4-595">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5f3a4-595">Lab</span></span>

* <span data-ttu-id="5f3a4-596">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-596">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="5f3a4-597">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-597">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-598">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-598">Monitor</span></span>

* <span data-ttu-id="5f3a4-599">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-599">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="5f3a4-600">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-600">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="5f3a4-601">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-601">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="5f3a4-602">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-602">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="5f3a4-603">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-603">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="5f3a4-604">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-604">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="5f3a4-605">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="5f3a4-605">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="5f3a4-606">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="5f3a4-606">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="5f3a4-607">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="5f3a4-607">`location` no longer required</span></span>
  * <span data-ttu-id="5f3a4-608">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="5f3a4-608">Add name and ID support for target</span></span>
  * <span data-ttu-id="5f3a4-609">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-609">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="5f3a4-610">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="5f3a4-610">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="5f3a4-611">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="5f3a4-611">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="5f3a4-612">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="5f3a4-612">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="5f3a4-613">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-613">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="5f3a4-614">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-614">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-615">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-615">Network</span></span>

* <span data-ttu-id="5f3a4-616">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-616">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="5f3a4-617">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-617">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="5f3a4-618">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="5f3a4-618">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="5f3a4-619">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="5f3a4-619">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="5f3a4-620">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-620">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="5f3a4-621">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-621">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="5f3a4-622">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-622">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="5f3a4-623">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-623">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="5f3a4-624">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-624">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="5f3a4-625">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-625">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="5f3a4-626">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-626">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="5f3a4-627">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-627">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="5f3a4-628">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-628">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="5f3a4-629">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-629">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="5f3a4-630">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-630">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="5f3a4-631">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-631">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="5f3a4-632">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-632">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="5f3a4-633">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-633">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="5f3a4-634">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-634">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="5f3a4-635">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-635">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="5f3a4-636">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-636">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="5f3a4-637">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-637">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="5f3a4-638">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-638">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="5f3a4-639">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5f3a4-639">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="5f3a4-640">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5f3a4-640">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="5f3a4-641">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5f3a4-641">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="5f3a4-642">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="5f3a4-642">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="5f3a4-643">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f3a4-643">Profile</span></span>

* <span data-ttu-id="5f3a4-644">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-644">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="5f3a4-645">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="5f3a4-645">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="5f3a4-646">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="5f3a4-646">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="5f3a4-647">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="5f3a4-647">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="5f3a4-648">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-648">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="5f3a4-649">RDBMS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-649">RDBMS</span></span>

* <span data-ttu-id="5f3a4-650">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-650">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="5f3a4-651">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-651">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="5f3a4-652">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-652">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="5f3a4-653">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-653">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-654">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-654">Resource</span></span>

* <span data-ttu-id="5f3a4-655">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-655">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="5f3a4-656">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-656">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="5f3a4-657">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-657">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="5f3a4-658">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-658">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="5f3a4-659">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-659">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="5f3a4-660">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-660">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="5f3a4-661">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-661">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="5f3a4-662">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-662">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="5f3a4-663">Função</span><span class="sxs-lookup"><span data-stu-id="5f3a4-663">Role</span></span>

* <span data-ttu-id="5f3a4-664">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-664">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="5f3a4-665">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-665">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="5f3a4-666">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-666">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="5f3a4-667">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-667">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="5f3a4-668">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-668">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="5f3a4-669">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="5f3a4-669">Service Fabric</span></span>
* <span data-ttu-id="5f3a4-670">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-670">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="5f3a4-671">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-671">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="5f3a4-672">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-672">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-673">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-673">SQL</span></span>

* <span data-ttu-id="5f3a4-674">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-674">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="5f3a4-675">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-675">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="5f3a4-676">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-676">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-677">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-677">Storage</span></span>

* <span data-ttu-id="5f3a4-678">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-678">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="5f3a4-679">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="5f3a4-679">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="5f3a4-680">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-680">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="5f3a4-681">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-681">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="5f3a4-682">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-682">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="5f3a4-683">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-683">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-684">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-684">VM</span></span>

* <span data-ttu-id="5f3a4-685">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="5f3a4-685">Support configuring nsg</span></span>
* <span data-ttu-id="5f3a4-686">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="5f3a4-686">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="5f3a4-687">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="5f3a4-687">Support managed service identities</span></span>
* <span data-ttu-id="5f3a4-688">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-688">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="5f3a4-689">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="5f3a4-689">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="5f3a4-690">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-690">May 10, 2017</span></span>

<span data-ttu-id="5f3a4-691">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="5f3a4-691">Version 2.0.6</span></span>

* <span data-ttu-id="5f3a4-692">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f3a4-692">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="5f3a4-693">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-693">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="5f3a4-694">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-694">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="5f3a4-695">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-695">Include Cognitive Services module.</span></span>
* <span data-ttu-id="5f3a4-696">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-696">Include Service Fabric module.</span></span>
* <span data-ttu-id="5f3a4-697">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="5f3a4-697">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="5f3a4-698">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-698">Add support for CDN commands.</span></span>
* <span data-ttu-id="5f3a4-699">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-699">Remove Container module.</span></span>
* <span data-ttu-id="5f3a4-700">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-700">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="5f3a4-701">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-701">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

```
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

### <a name="core"></a><span data-ttu-id="5f3a4-702">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-702">Core</span></span>

* <span data-ttu-id="5f3a4-703">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="5f3a4-703">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="5f3a4-704">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-704">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="5f3a4-705">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-705">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="5f3a4-706">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-706">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="5f3a4-707">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-707">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="5f3a4-708">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-708">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="5f3a4-709">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-709">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="5f3a4-710">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-710">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="5f3a4-711">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-711">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="5f3a4-712">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="5f3a4-712">core: Improved performance</span></span>
* <span data-ttu-id="5f3a4-713">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="5f3a4-713">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="5f3a4-714">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="5f3a4-714">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-715">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-715">ACS</span></span>

* <span data-ttu-id="5f3a4-716">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f3a4-716">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="5f3a4-717">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="5f3a4-717">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="5f3a4-718">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="5f3a4-718">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="5f3a4-719">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-719">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-720">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-720">AppService</span></span>

* <span data-ttu-id="5f3a4-721">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-721">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="5f3a4-722">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="5f3a4-722">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="5f3a4-723">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-723">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="5f3a4-724">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="5f3a4-724">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="5f3a4-725">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="5f3a4-725">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="5f3a4-726">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-726">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="5f3a4-727">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="5f3a4-727">support slot swap with preview</span></span>
* <span data-ttu-id="5f3a4-728">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-728">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="5f3a4-729">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-729">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="5f3a4-730">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="5f3a4-730">CosmosDB</span></span>

* <span data-ttu-id="5f3a4-731">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-731">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="5f3a4-732">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="5f3a4-732">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="5f3a4-733">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="5f3a4-733">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="5f3a4-734">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="5f3a4-734">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="5f3a4-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="5f3a4-735">Data Lake Analytics</span></span>

* <span data-ttu-id="5f3a4-736">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-736">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="5f3a4-737">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-737">Add support for new catalog item type: package.</span></span> <span data-ttu-id="5f3a4-738">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-738">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="5f3a4-739">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="5f3a4-739">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="5f3a4-740">Tabela</span><span class="sxs-lookup"><span data-stu-id="5f3a4-740">Table</span></span>
  * <span data-ttu-id="5f3a4-741">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="5f3a4-741">Table valued function</span></span>
  * <span data-ttu-id="5f3a4-742">Visualizar</span><span class="sxs-lookup"><span data-stu-id="5f3a4-742">View</span></span>
  * <span data-ttu-id="5f3a4-743">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-743">Table Statistics.</span></span> <span data-ttu-id="5f3a4-744">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-744">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="5f3a4-745">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="5f3a4-745">Data Lake Store</span></span>

* <span data-ttu-id="5f3a4-746">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-746">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="5f3a4-747">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-747">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="5f3a4-748">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-748">missed help for access show.</span></span> <span data-ttu-id="5f3a4-749">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-749">adding it.</span></span> <span data-ttu-id="5f3a4-750">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="5f3a4-751">Localizar</span><span class="sxs-lookup"><span data-stu-id="5f3a4-751">Find</span></span>

* <span data-ttu-id="5f3a4-752">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="5f3a4-752">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="5f3a4-753">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5f3a4-753">KeyVault</span></span>

* <span data-ttu-id="5f3a4-754">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="5f3a4-754">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="5f3a4-755">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-755">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="5f3a4-756">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="5f3a4-756">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="5f3a4-757">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-757">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="5f3a4-758">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-758">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="5f3a4-759">Laboratório</span><span class="sxs-lookup"><span data-stu-id="5f3a4-759">Lab</span></span>

* <span data-ttu-id="5f3a4-760">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-760">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="5f3a4-761">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-761">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="5f3a4-762">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-762">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="5f3a4-763">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-763">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="5f3a4-764">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-764">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="5f3a4-765">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-765">Monitor</span></span>

* <span data-ttu-id="5f3a4-766">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-766">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="5f3a4-767">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-767">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="5f3a4-768">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-768">Network</span></span>

* <span data-ttu-id="5f3a4-769">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-769">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="5f3a4-770">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-770">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="5f3a4-771">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-771">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="5f3a4-772">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-772">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="5f3a4-773">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-773">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="5f3a4-774">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-774">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="5f3a4-775">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-775">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="5f3a4-776">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-776">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="5f3a4-777">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-777">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="5f3a4-778">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="5f3a4-778">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="5f3a4-779">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-779">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="5f3a4-780">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="5f3a4-780">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="5f3a4-781">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-781">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="5f3a4-782">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-782">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="5f3a4-783">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-783">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="5f3a4-784">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-784">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="5f3a4-785">Perfil</span><span class="sxs-lookup"><span data-stu-id="5f3a4-785">Profile</span></span>

* <span data-ttu-id="5f3a4-786">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-786">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="5f3a4-787">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-787">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="5f3a4-788">Redis</span><span class="sxs-lookup"><span data-stu-id="5f3a4-788">Redis</span></span>

* <span data-ttu-id="5f3a4-789">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="5f3a4-789">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="5f3a4-790">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-790">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="5f3a4-791">Recurso</span><span class="sxs-lookup"><span data-stu-id="5f3a4-791">Resource</span></span>

* <span data-ttu-id="5f3a4-792">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-792">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="5f3a4-793">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-793">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="5f3a4-794">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-794">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="5f3a4-795">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-795">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="5f3a4-796">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="5f3a4-797">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-797">Add docs for az lock update.</span></span> <span data-ttu-id="5f3a4-798">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="5f3a4-799">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-799">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="5f3a4-800">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="5f3a4-801">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-801">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="5f3a4-802">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="5f3a4-803">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-803">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="5f3a4-804">Função</span><span class="sxs-lookup"><span data-stu-id="5f3a4-804">Role</span></span>

* <span data-ttu-id="5f3a4-805">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-805">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="5f3a4-806">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-806">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="5f3a4-807">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-807">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="5f3a4-808">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="5f3a4-808">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="5f3a4-809">SQL</span><span class="sxs-lookup"><span data-stu-id="5f3a4-809">SQL</span></span>

* <span data-ttu-id="5f3a4-810">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-810">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="5f3a4-811">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-811">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="5f3a4-812">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-812">Storage</span></span>

* <span data-ttu-id="5f3a4-813">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-813">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="5f3a4-814">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="5f3a4-814">Add support for incremental blob copy</span></span>
* <span data-ttu-id="5f3a4-815">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="5f3a4-815">Add support for large block blob upload</span></span>
* <span data-ttu-id="5f3a4-816">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="5f3a4-816">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-817">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-817">VM</span></span>

* <span data-ttu-id="5f3a4-818">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="5f3a4-818">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="5f3a4-819">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-819">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="5f3a4-820">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="5f3a4-820">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="5f3a4-821">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="5f3a4-821">az vm/vmss disk</span></span>
  3. <span data-ttu-id="5f3a4-822">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="5f3a4-822">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="5f3a4-823">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="5f3a4-823">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="5f3a4-824">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-824">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="5f3a4-825">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-825">April 3, 2017</span></span>

<span data-ttu-id="5f3a4-826">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="5f3a4-826">Version 2.0.2</span></span>

<span data-ttu-id="5f3a4-827">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-827">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

```
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

### <a name="core"></a><span data-ttu-id="5f3a4-828">Núcleo</span><span class="sxs-lookup"><span data-stu-id="5f3a4-828">Core</span></span>

* <span data-ttu-id="5f3a4-829">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-829">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="5f3a4-830">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-830">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="5f3a4-831">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-831">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="5f3a4-832">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-832">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f3a4-833">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-833">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="5f3a4-834">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-834">Add prompting for missing template parameters.</span></span> <span data-ttu-id="5f3a4-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="5f3a4-836">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="5f3a4-836">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="5f3a4-837">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="5f3a4-837">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="5f3a4-838">ACS</span><span class="sxs-lookup"><span data-stu-id="5f3a4-838">ACS</span></span>

* <span data-ttu-id="5f3a4-839">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-839">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="5f3a4-840">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-840">Add support for ssh key password prompting.</span></span> <span data-ttu-id="5f3a4-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="5f3a4-842">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-842">Add support for windows clusters.</span></span> <span data-ttu-id="5f3a4-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="5f3a4-844">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-844">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="5f3a4-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="5f3a4-846">AppService</span><span class="sxs-lookup"><span data-stu-id="5f3a4-846">AppService</span></span>

* <span data-ttu-id="5f3a4-847">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-847">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="5f3a4-848">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-848">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="5f3a4-849">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-849">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="5f3a4-850">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-850">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="5f3a4-851">DataLake</span><span class="sxs-lookup"><span data-stu-id="5f3a4-851">DataLake</span></span>

* <span data-ttu-id="5f3a4-852">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-852">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="5f3a4-853">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-853">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="5f3a4-854">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="5f3a4-854">DocuemntDB</span></span>

* <span data-ttu-id="5f3a4-855">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-855">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="5f3a4-856">VM</span><span class="sxs-lookup"><span data-stu-id="5f3a4-856">VM</span></span>

* <span data-ttu-id="5f3a4-857">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-857">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="5f3a4-858">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-858">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="5f3a4-859">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-859">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="5f3a4-860">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-860">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="5f3a4-861">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-861">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="5f3a4-862">Adicionar --secrets para o conjunto de dimensionamento de máquinas virtuais e VM ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-862">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="5f3a4-863">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="5f3a4-863">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="5f3a4-864">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="5f3a4-864">February 27, 2017</span></span>

<span data-ttu-id="5f3a4-865">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="5f3a4-865">Version 2.0.0</span></span>

<span data-ttu-id="5f3a4-866">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-866">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="5f3a4-867">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-867">General availability applies to these command modules:</span></span>
- <span data-ttu-id="5f3a4-868">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-868">Container Service (acs)</span></span>
- <span data-ttu-id="5f3a4-869">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-869">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="5f3a4-870">Rede</span><span class="sxs-lookup"><span data-stu-id="5f3a4-870">Networking</span></span>
- <span data-ttu-id="5f3a4-871">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5f3a4-871">Storage</span></span>

<span data-ttu-id="5f3a4-872">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-872">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="5f3a4-873">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="5f3a4-873">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="5f3a4-874">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-874">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="5f3a4-875">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-875">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="5f3a4-876">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-876">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="5f3a4-877">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-877">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

```
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
> <span data-ttu-id="5f3a4-878">Alguns dos módulos de comando têm um “b*n*” ou “rc*n*” pós-fixado.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-878">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="5f3a4-879">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-879">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="5f3a4-880">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-880">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="5f3a4-881">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="5f3a4-881">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="5f3a4-882">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="5f3a4-882">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="5f3a4-883">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="5f3a4-883">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="5f3a4-884">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="5f3a4-884">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="5f3a4-885">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="5f3a4-885">Provide feedback from the command line with the `az feedback` command.</span></span>

