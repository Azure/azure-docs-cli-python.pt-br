---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/14/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: cf9c4e1a86b3315d45a7533f67b731ee2f3d6bc0
ms.sourcegitcommit: 857d0f19fd87d37d134efdf0dda0e7003260938b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86308671"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="aae04-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="aae04-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="aae04-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="july-14-2020"></a><span data-ttu-id="aae04-105">14 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-105">July 14, 2020</span></span>

<span data-ttu-id="aae04-106">Versão 2.9.0</span><span class="sxs-lookup"><span data-stu-id="aae04-106">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-107">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-107">ACR</span></span>

* <span data-ttu-id="aae04-108">Manipular o link do artefato de log do Registro para os logs de fluxo</span><span class="sxs-lookup"><span data-stu-id="aae04-108">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="aae04-109">Substituir comandos helm2</span><span class="sxs-lookup"><span data-stu-id="aae04-109">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-110">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-110">AKS</span></span>

* <span data-ttu-id="aae04-111">`az aks create`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="aae04-111">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="aae04-112">`az aks update`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="aae04-112">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="aae04-113">APIM</span><span class="sxs-lookup"><span data-stu-id="aae04-113">APIM</span></span>

* <span data-ttu-id="aae04-114">Comandos az apim api gerais adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-114">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-115">AppConfig</span></span>

* <span data-ttu-id="aae04-116">Adicionar exemplo para usar --fields na revisão do appconfig</span><span class="sxs-lookup"><span data-stu-id="aae04-116">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-117">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-117">AppService</span></span>

* <span data-ttu-id="aae04-118">`az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-118">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="aae04-119">Suporte à API de pilhas adicionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-119">Added Stacks API Support.</span></span>
* <span data-ttu-id="aae04-120">Correção nº 14208 falha na criação de um aplicativo com vários contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-120">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="aae04-121">Corrige az webapp create – usa pilhas de runtime embutidas em código</span><span class="sxs-lookup"><span data-stu-id="aae04-121">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-122">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-122">ARM</span></span>

* <span data-ttu-id="aae04-123">`az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="aae04-123">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-124">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-124">Compute</span></span>

* <span data-ttu-id="aae04-125">Avançar os discos de versão 2020-05-01, computação 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="aae04-125">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="aae04-126">Criptografia dupla do conjunto de criptografia de disco</span><span class="sxs-lookup"><span data-stu-id="aae04-126">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="aae04-127">`az vmss update`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="aae04-127">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="aae04-128">`az sig image-version create`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="aae04-128">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="aae04-129">vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-129">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="aae04-130">Adicionar operação de remoção simulada para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-130">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-131">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-131">CosmosDB</span></span>

* <span data-ttu-id="aae04-132">Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="aae04-132">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aae04-133">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aae04-133">EventGrid</span></span>

* <span data-ttu-id="aae04-134">Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="aae04-134">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="aae04-135">Localizar</span><span class="sxs-lookup"><span data-stu-id="aae04-135">Find</span></span>

* <span data-ttu-id="aae04-136">Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada</span><span class="sxs-lookup"><span data-stu-id="aae04-136">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-137">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-137">HDInsight</span></span>

* <span data-ttu-id="aae04-138">Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight</span><span class="sxs-lookup"><span data-stu-id="aae04-138">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-139">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-139">Monitor</span></span>

* <span data-ttu-id="aae04-140">Remover sinalizador de visualização para comandos no workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-140">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="aae04-141">`az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-141">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="aae04-142">`az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica</span><span class="sxs-lookup"><span data-stu-id="aae04-142">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="aae04-143">`az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-143">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="aae04-144">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-144">Network</span></span>

* <span data-ttu-id="aae04-145">`az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="aae04-145">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="aae04-146">Avançar azure-mgmt-network para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-146">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="aae04-147">`az network express-route gateway connection`: dá suporte à configuração de roteamento</span><span class="sxs-lookup"><span data-stu-id="aae04-147">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="aae04-148">`az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.</span><span class="sxs-lookup"><span data-stu-id="aae04-148">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="aae04-149">Recurso de link privado de suporte do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-149">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="aae04-150">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="aae04-150">PolicyInsights</span></span>

* <span data-ttu-id="aae04-151">`az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política</span><span class="sxs-lookup"><span data-stu-id="aae04-151">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="aae04-152">`az policy state list`: expõe versões de entidades de política em cada registro de conformidade</span><span class="sxs-lookup"><span data-stu-id="aae04-152">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-153">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-153">Profile</span></span>

* <span data-ttu-id="aae04-154">`az account get-access-token`: Mostra expiresOn para Identidade Gerenciada</span><span class="sxs-lookup"><span data-stu-id="aae04-154">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-155">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-155">RDBMS</span></span>

* <span data-ttu-id="aae04-156">Dar suporte à versão mínima do TLS</span><span class="sxs-lookup"><span data-stu-id="aae04-156">Support Minimum TLS version</span></span>
* <span data-ttu-id="aae04-157">Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-157">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="aae04-158">Segurança</span><span class="sxs-lookup"><span data-stu-id="aae04-158">Security</span></span>

* <span data-ttu-id="aae04-159">Adicionar comandos allowed_connections</span><span class="sxs-lookup"><span data-stu-id="aae04-159">Add allowed_connections commands</span></span>
* <span data-ttu-id="aae04-160">Adicionar comandos hardeningss da rede adaptável</span><span class="sxs-lookup"><span data-stu-id="aae04-160">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="aae04-161">Adicionar comandos adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="aae04-161">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="aae04-162">Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-162">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="aae04-163">Adicionar CLI de conformidade regulatória</span><span class="sxs-lookup"><span data-stu-id="aae04-163">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="aae04-164">SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-164">SignalR</span></span>

* <span data-ttu-id="aae04-165">Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream</span><span class="sxs-lookup"><span data-stu-id="aae04-165">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-166">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-166">SQL</span></span>

* <span data-ttu-id="aae04-167">`az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-167">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="aae04-168">`az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário</span><span class="sxs-lookup"><span data-stu-id="aae04-168">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-169">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-169">Storage</span></span>

* <span data-ttu-id="aae04-170">`az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-170">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="aae04-171">`az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-171">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="aae04-172">Remover credencial de token de check-in</span><span class="sxs-lookup"><span data-stu-id="aae04-172">Remove check in token credential</span></span>
* <span data-ttu-id="aae04-173">Corrigir o nome da conta de armazenamento em exemplos</span><span class="sxs-lookup"><span data-stu-id="aae04-173">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="aae04-174">Webapp</span><span class="sxs-lookup"><span data-stu-id="aae04-174">Webapp</span></span>

* <span data-ttu-id="aae04-175">Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log</span><span class="sxs-lookup"><span data-stu-id="aae04-175">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="aae04-176">Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet</span><span class="sxs-lookup"><span data-stu-id="aae04-176">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="aae04-177">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-177">June 23, 2020</span></span>

<span data-ttu-id="aae04-178">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="aae04-178">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-179">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-179">ACR</span></span>

* <span data-ttu-id="aae04-180">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="aae04-180">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="aae04-181">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="aae04-181">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-182">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-182">ACS</span></span>

* <span data-ttu-id="aae04-183">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="aae04-183">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-184">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-184">AKS</span></span>

* <span data-ttu-id="aae04-185">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="aae04-185">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="aae04-186">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="aae04-186">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="aae04-187">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="aae04-187">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="aae04-188">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="aae04-188">Fix typo in az aks update command</span></span>
* <span data-ttu-id="aae04-189">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="aae04-189">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="aae04-190">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-190">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-191">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-191">AMS</span></span>

* <span data-ttu-id="aae04-192">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="aae04-192">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-193">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-193">AppService</span></span>

* <span data-ttu-id="aae04-194">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="aae04-194">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="aae04-195">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="aae04-195">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="aae04-196">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-196">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="aae04-197">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="aae04-197">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="aae04-198">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="aae04-198">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="aae04-199">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="aae04-199">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="aae04-200">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-200">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="aae04-201">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="aae04-201">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="aae04-202">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-202">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="aae04-203">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="aae04-203">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="aae04-204">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="aae04-204">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-205">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-205">ARM</span></span>

* <span data-ttu-id="aae04-206">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="aae04-206">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="aae04-207">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="aae04-207">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="aae04-208">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="aae04-208">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="aae04-209">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="aae04-209">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="aae04-210">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="aae04-210">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="aae04-211">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="aae04-211">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="aae04-212">ARO</span><span class="sxs-lookup"><span data-stu-id="aae04-212">ARO</span></span>

* <span data-ttu-id="aae04-213">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="aae04-213">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-214">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-214">Batch</span></span>

* <span data-ttu-id="aae04-215">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="aae04-215">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="aae04-216">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="aae04-216">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="aae04-217">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="aae04-217">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="aae04-218">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="aae04-218">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="aae04-219">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="aae04-219">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="aae04-220">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="aae04-220">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="aae04-221">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="aae04-221">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="aae04-222">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="aae04-222">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-223">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-223">CDN</span></span>

* <span data-ttu-id="aae04-224">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="aae04-224">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="aae04-225">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="aae04-225">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aae04-226">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-226">Cognitive Services</span></span>

* <span data-ttu-id="aae04-227">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="aae04-227">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="aae04-228">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="aae04-228">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-229">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-229">Compute</span></span>

* <span data-ttu-id="aae04-230">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="aae04-230">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="aae04-231">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="aae04-231">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="aae04-232">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-232">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="aae04-233">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="aae04-233">New command `az image builder cancel`</span></span>
* <span data-ttu-id="aae04-234">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="aae04-234">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-235">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-235">Cosmos DB</span></span>

* <span data-ttu-id="aae04-236">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-236">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="aae04-237">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="aae04-237">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="aae04-238">EventHub</span><span class="sxs-lookup"><span data-stu-id="aae04-238">EventHub</span></span>

* <span data-ttu-id="aae04-239">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="aae04-239">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-240">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-240">Extension</span></span>

* <span data-ttu-id="aae04-241">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="aae04-241">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="aae04-242">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="aae04-242">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="aae04-243">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-243">Iot Hub</span></span>

* <span data-ttu-id="aae04-244">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-244">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-245">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-245">KeyVault</span></span>

* <span data-ttu-id="aae04-246">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="aae04-246">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="aae04-247">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="aae04-247">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-248">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-248">Monitor</span></span>

* <span data-ttu-id="aae04-249">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-249">Support no wait for cluster creation</span></span>
* <span data-ttu-id="aae04-250">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="aae04-250">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="aae04-251">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-251">Network</span></span>

* <span data-ttu-id="aae04-252">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="aae04-252">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="aae04-253">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="aae04-253">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="aae04-254">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="aae04-254">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="aae04-255">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="aae04-255">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-256">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-256">RBAC</span></span>

* <span data-ttu-id="aae04-257">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="aae04-257">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="aae04-258">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="aae04-258">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="aae04-259">Segurança</span><span class="sxs-lookup"><span data-stu-id="aae04-259">Security</span></span>

* <span data-ttu-id="aae04-260">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="aae04-260">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-261">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-261">SQL</span></span>

* <span data-ttu-id="aae04-262">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="aae04-262">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-263">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-263">Storage</span></span>

* <span data-ttu-id="aae04-264">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="aae04-264">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="aae04-265">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="aae04-265">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="aae04-266">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="aae04-266">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="aae04-267">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="aae04-267">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="aae04-268">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="aae04-268">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="aae04-269">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="aae04-269">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="aae04-270">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="aae04-270">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="aae04-271">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="aae04-271">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="aae04-272">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="aae04-272">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="aae04-273">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="aae04-273">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="aae04-274">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-274">June 02, 2020</span></span>

<span data-ttu-id="aae04-275">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="aae04-275">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-276">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-276">ACR</span></span>

* <span data-ttu-id="aae04-277">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="aae04-277">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-278">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-278">AKS</span></span>

* <span data-ttu-id="aae04-279">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="aae04-279">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="aae04-280">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="aae04-280">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-281">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-281">AppService</span></span>

* <span data-ttu-id="aae04-282">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="aae04-282">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-283">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-283">ARM</span></span>

* <span data-ttu-id="aae04-284">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="aae04-284">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="aae04-285">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="aae04-285">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="aae04-286">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-286">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="aae04-287">ARO</span><span class="sxs-lookup"><span data-stu-id="aae04-287">ARO</span></span>

* <span data-ttu-id="aae04-288">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="aae04-288">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="aae04-289">EventHub</span><span class="sxs-lookup"><span data-stu-id="aae04-289">EventHub</span></span>

* <span data-ttu-id="aae04-290">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="aae04-290">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-291">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-291">HDInsight</span></span>

* <span data-ttu-id="aae04-292">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="aae04-292">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-293">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-293">Monitor</span></span>

* <span data-ttu-id="aae04-294">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-294">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="aae04-295">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="aae04-295">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="aae04-296">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="aae04-296">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="aae04-297">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-297">Network</span></span>

* <span data-ttu-id="aae04-298">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="aae04-298">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="aae04-299">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="aae04-299">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="aae04-300">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="aae04-300">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="aae04-301">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-301">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="aae04-302">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-302">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-303">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-303">Packaging</span></span>

* <span data-ttu-id="aae04-304">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="aae04-304">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-305">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-305">RBAC</span></span>

* <span data-ttu-id="aae04-306">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="aae04-306">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-307">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-307">Redis</span></span>

* <span data-ttu-id="aae04-308">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="aae04-308">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-309">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-309">Storage</span></span>

* <span data-ttu-id="aae04-310">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="aae04-310">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="aae04-311">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-311">Enable local context for storage account</span></span>
* <span data-ttu-id="aae04-312">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="aae04-312">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="aae04-313">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-313">May 19, 2020</span></span>

<span data-ttu-id="aae04-314">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="aae04-314">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-315">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-315">ACR</span></span>

* <span data-ttu-id="aae04-316">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-316">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="aae04-317">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="aae04-317">Support disable public network access</span></span>
* <span data-ttu-id="aae04-318">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="aae04-318">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="aae04-319">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="aae04-319">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-320">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-320">ACS</span></span>

* <span data-ttu-id="aae04-321">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="aae04-321">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-322">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-322">AKS</span></span>

* <span data-ttu-id="aae04-323">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="aae04-323">Update uptime-sla command help context</span></span>
* <span data-ttu-id="aae04-324">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="aae04-324">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="aae04-325">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-325">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-326">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-326">AMS</span></span>

* <span data-ttu-id="aae04-327">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="aae04-327">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="aae04-328">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="aae04-328">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-329">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-329">AppConfig</span></span>

* <span data-ttu-id="aae04-330">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="aae04-330">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-331">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-331">AppService</span></span>

* <span data-ttu-id="aae04-332">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="aae04-332">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="aae04-333">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="aae04-333">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="aae04-334">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="aae04-334">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="aae04-335">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-335">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-336">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-336">ARM</span></span>

* <span data-ttu-id="aae04-337">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="aae04-337">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="aae04-338">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="aae04-338">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="aae04-339">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="aae04-339">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="aae04-340">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="aae04-340">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="aae04-341">ARO</span><span class="sxs-lookup"><span data-stu-id="aae04-341">ARO</span></span>

* <span data-ttu-id="aae04-342">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="aae04-342">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="aae04-343">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="aae04-343">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-344">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-344">Backup</span></span>

* <span data-ttu-id="aae04-345">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="aae04-345">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="aae04-346">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="aae04-346">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="aae04-347">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="aae04-347">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="aae04-348">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="aae04-348">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="aae04-349">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-349">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="aae04-350">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="aae04-350">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="aae04-351">CI</span><span class="sxs-lookup"><span data-stu-id="aae04-351">CI</span></span>

* <span data-ttu-id="aae04-352">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="aae04-352">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-353">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-353">Compute</span></span>

* <span data-ttu-id="aae04-354">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="aae04-354">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="aae04-355">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="aae04-355">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="aae04-356">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-356">Core</span></span>

* <span data-ttu-id="aae04-357">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="aae04-357">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-358">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-358">Extension</span></span>

* <span data-ttu-id="aae04-359">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="aae04-359">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="aae04-360">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="aae04-360">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-361">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-361">IoT</span></span>

* <span data-ttu-id="aae04-362">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="aae04-362">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="aae04-363">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-363">IoT Hub</span></span>

* <span data-ttu-id="aae04-364">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="aae04-364">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aae04-365">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aae04-365">NetAppFiles</span></span>

* <span data-ttu-id="aae04-366">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="aae04-366">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="aae04-367">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-367">Network</span></span>

* <span data-ttu-id="aae04-368">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="aae04-368">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="aae04-369">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="aae04-369">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="aae04-370">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="aae04-370">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="aae04-371">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="aae04-371">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="aae04-372">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="aae04-372">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="aae04-373">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="aae04-373">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="aae04-374">Saída</span><span class="sxs-lookup"><span data-stu-id="aae04-374">Output</span></span>

* <span data-ttu-id="aae04-375">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="aae04-375">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-376">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-376">Packaging</span></span>

* <span data-ttu-id="aae04-377">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="aae04-377">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-378">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-378">RBAC</span></span>

* <span data-ttu-id="aae04-379">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="aae04-379">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-380">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-380">Storage</span></span>

* <span data-ttu-id="aae04-381">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-381">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="aae04-382">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="aae04-382">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="aae04-383">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="aae04-383">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="aae04-384">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="aae04-384">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="aae04-385">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="aae04-385">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="aae04-386">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-386">April 30, 2020</span></span>

<span data-ttu-id="aae04-387">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="aae04-387">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-388">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-388">ACR</span></span>

* <span data-ttu-id="aae04-389">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-389">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-390">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-390">Compute</span></span>

* <span data-ttu-id="aae04-391">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="aae04-391">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="aae04-392">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-392">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="aae04-393">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="aae04-393">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-394">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-394">Cosmos DB</span></span>

* <span data-ttu-id="aae04-395">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="aae04-395">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-396">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-396">Extension</span></span>

* <span data-ttu-id="aae04-397">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="aae04-397">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-398">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-398">Packaging</span></span>

* <span data-ttu-id="aae04-399">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-399">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-400">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-400">SQL</span></span>

* <span data-ttu-id="aae04-401">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="aae04-401">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-402">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-402">Storage</span></span>

* <span data-ttu-id="aae04-403">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="aae04-403">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="aae04-404">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-404">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="aae04-405">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="aae04-405">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="aae04-406">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="aae04-406">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="aae04-407">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-407">April 28, 2020</span></span>

<span data-ttu-id="aae04-408">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="aae04-408">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-409">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-409">ACS</span></span>

* <span data-ttu-id="aae04-410">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="aae04-410">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="aae04-411">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="aae04-411">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="aae04-412">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="aae04-412">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="aae04-413">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="aae04-413">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-414">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-414">AKS</span></span>

* <span data-ttu-id="aae04-415">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-415">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-416">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-416">AppService</span></span>

* <span data-ttu-id="aae04-417">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="aae04-417">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-418">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-418">ARM</span></span>

* <span data-ttu-id="aae04-419">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="aae04-419">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="aae04-420">ARO</span><span class="sxs-lookup"><span data-stu-id="aae04-420">ARO</span></span>

* <span data-ttu-id="aae04-421">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-421">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="aae04-422">CI</span><span class="sxs-lookup"><span data-stu-id="aae04-422">CI</span></span>

* <span data-ttu-id="aae04-423">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="aae04-423">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-424">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-424">Compute</span></span>

* <span data-ttu-id="aae04-425">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="aae04-425">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="aae04-426">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="aae04-426">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="aae04-427">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-427">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-428">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-428">KeyVault</span></span>

* <span data-ttu-id="aae04-429">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="aae04-429">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-430">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-430">Monitor</span></span>

* <span data-ttu-id="aae04-431">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="aae04-431">Support LA cluster CMK features</span></span>
* <span data-ttu-id="aae04-432">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="aae04-432">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="aae04-433">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-433">Network</span></span>

* <span data-ttu-id="aae04-434">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="aae04-434">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="aae04-435">Privatedns</span><span class="sxs-lookup"><span data-stu-id="aae04-435">Privatedns</span></span>

* <span data-ttu-id="aae04-436">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="aae04-436">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="aae04-437">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-437">April 21, 2020</span></span>

<span data-ttu-id="aae04-438">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="aae04-438">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-439">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-439">ACR</span></span>

* <span data-ttu-id="aae04-440">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-440">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="aae04-441">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="aae04-441">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-442">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-442">AKS</span></span>

* <span data-ttu-id="aae04-443">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="aae04-443">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="aae04-444">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="aae04-444">Add --uptime-sla</span></span>
* <span data-ttu-id="aae04-445">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="aae04-445">Update containerservice package</span></span>
* <span data-ttu-id="aae04-446">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="aae04-446">Add node public IP support</span></span>
* <span data-ttu-id="aae04-447">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-447">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-448">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-448">AppConfig</span></span>

* <span data-ttu-id="aae04-449">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="aae04-449">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="aae04-450">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="aae04-450">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-451">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-451">AppService</span></span>

* <span data-ttu-id="aae04-452">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="aae04-452">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="aae04-453">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="aae04-453">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="aae04-454">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="aae04-454">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="aae04-455">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="aae04-455">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="aae04-456">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="aae04-456">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-457">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-457">ARM</span></span>

* <span data-ttu-id="aae04-458">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="aae04-458">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="aae04-459">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-459">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="aae04-460">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="aae04-460">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="aae04-461">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="aae04-461">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="aae04-462">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="aae04-462">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="aae04-463">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="aae04-463">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="aae04-464">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="aae04-464">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="aae04-465">ARO</span><span class="sxs-lookup"><span data-stu-id="aae04-465">ARO</span></span>

* <span data-ttu-id="aae04-466">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="aae04-466">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-467">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-467">Batch</span></span>

* <span data-ttu-id="aae04-468">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-468">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-469">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-469">Compute</span></span>

* <span data-ttu-id="aae04-470">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="aae04-470">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="aae04-471">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="aae04-471">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="aae04-472">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="aae04-472">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="aae04-473">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="aae04-473">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="aae04-474">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="aae04-474">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="aae04-475">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="aae04-475">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-476">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-476">CosmosDB</span></span>

* <span data-ttu-id="aae04-477">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="aae04-477">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="aae04-478">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-478">IoT Central</span></span>

* <span data-ttu-id="aae04-479">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="aae04-479">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="aae04-480">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="aae04-480">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-481">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-481">Monitor</span></span>

* <span data-ttu-id="aae04-482">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-482">Support private link scenario for monitor</span></span>
* <span data-ttu-id="aae04-483">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="aae04-483">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="aae04-484">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-484">Network</span></span>

* <span data-ttu-id="aae04-485">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="aae04-485">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="aae04-486">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="aae04-486">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="aae04-487">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="aae04-487">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="aae04-488">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="aae04-488">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-489">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-489">Packaging</span></span>

* <span data-ttu-id="aae04-490">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="aae04-490">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-491">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-491">RBAC</span></span>

* <span data-ttu-id="aae04-492">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="aae04-492">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-493">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-493">RDBMS</span></span>

* <span data-ttu-id="aae04-494">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-494">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aae04-495">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-495">Service Fabric</span></span>

* <span data-ttu-id="aae04-496">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="aae04-496">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="aae04-497">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="aae04-497">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-498">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-498">SQL</span></span>

* <span data-ttu-id="aae04-499">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="aae04-499">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="aae04-500">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="aae04-500">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-501">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-501">Storage</span></span>

* <span data-ttu-id="aae04-502">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-502">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="aae04-503">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-503">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="aae04-504">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="aae04-504">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="aae04-505">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="aae04-505">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="aae04-506">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-506">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="aae04-507">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="aae04-507">Survey</span></span>

* <span data-ttu-id="aae04-508">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="aae04-508">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="aae04-509">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-509">April 01, 2020</span></span>

<span data-ttu-id="aae04-510">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="aae04-510">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-511">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-511">ACR</span></span>

* <span data-ttu-id="aae04-512">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-512">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-513">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-513">Profile</span></span>

* <span data-ttu-id="aae04-514">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="aae04-514">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="aae04-515">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-515">March 31, 2020</span></span>

<span data-ttu-id="aae04-516">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="aae04-516">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-517">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-517">ACR</span></span>

* <span data-ttu-id="aae04-518">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="aae04-518">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="aae04-519">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="aae04-519">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="aae04-520">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="aae04-520">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="aae04-521">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="aae04-521">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="aae04-522">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-522">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="aae04-523">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="aae04-523">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="aae04-524">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-524">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-525">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-525">AKS</span></span>

* <span data-ttu-id="aae04-526">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="aae04-526">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="aae04-527">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="aae04-527">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="aae04-528">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="aae04-528">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-529">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-529">AMS</span></span>

* <span data-ttu-id="aae04-530">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="aae04-530">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-531">AppConfig</span></span>

* <span data-ttu-id="aae04-532">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="aae04-532">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-533">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-533">AppService</span></span>

* <span data-ttu-id="aae04-534">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-534">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="aae04-535">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="aae04-535">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="aae04-536">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-536">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-537">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-537">ARM</span></span>

* <span data-ttu-id="aae04-538">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-538">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="aae04-539">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-539">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="aae04-540">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="aae04-540">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="aae04-541">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="aae04-541">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-542">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-542">Backup</span></span>

* <span data-ttu-id="aae04-543">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="aae04-543">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="aae04-544">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="aae04-544">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="aae04-545">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="aae04-545">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-546">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-546">Compute</span></span>

* <span data-ttu-id="aae04-547">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="aae04-547">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="aae04-548">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="aae04-548">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="aae04-549">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="aae04-549">az vm update: Support --workspace</span></span>
* <span data-ttu-id="aae04-550">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="aae04-550">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="aae04-551">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="aae04-551">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="aae04-552">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="aae04-552">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="aae04-553">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="aae04-553">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="aae04-554">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="aae04-554">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-555">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-555">Cosmos DB</span></span>

* <span data-ttu-id="aae04-556">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="aae04-556">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="aae04-557">Docker</span><span class="sxs-lookup"><span data-stu-id="aae04-557">Docker</span></span>

* <span data-ttu-id="aae04-558">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="aae04-558">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-559">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-559">Extension</span></span>

* <span data-ttu-id="aae04-560">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="aae04-560">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-561">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-561">HDInsight</span></span>

* <span data-ttu-id="aae04-562">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="aae04-562">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="aae04-563">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="aae04-563">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-564">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-564">IoT</span></span>

* <span data-ttu-id="aae04-565">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="aae04-565">Add codeowner</span></span>
* <span data-ttu-id="aae04-566">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="aae04-566">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="aae04-567">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="aae04-567">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="aae04-568">IoT Central</span><span class="sxs-lookup"><span data-stu-id="aae04-568">IoTCentral</span></span>

* <span data-ttu-id="aae04-569">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="aae04-569">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-570">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-570">KeyVault</span></span>

* <span data-ttu-id="aae04-571">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="aae04-571">Support certificate backup/restore</span></span>
* <span data-ttu-id="aae04-572">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="aae04-572">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="aae04-573">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="aae04-573">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="aae04-574">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="aae04-574">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="aae04-575">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="aae04-575">Lock</span></span>

* <span data-ttu-id="aae04-576">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="aae04-576">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-577">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-577">Monitor</span></span>

* <span data-ttu-id="aae04-578">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="aae04-578">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="aae04-579">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="aae04-579">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aae04-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aae04-580">NetAppFiles</span></span>

* <span data-ttu-id="aae04-581">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="aae04-581">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="aae04-582">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-582">Network</span></span>

* <span data-ttu-id="aae04-583">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="aae04-583">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="aae04-584">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="aae04-584">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="aae04-585">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-585">support host names in application gateway listener</span></span>
* <span data-ttu-id="aae04-586">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="aae04-586">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="aae04-587">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="aae04-587">Support vpn gateway generation</span></span>
* <span data-ttu-id="aae04-588">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="aae04-588">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-589">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-589">Packaging</span></span>

* <span data-ttu-id="aae04-590">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="aae04-590">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-591">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-591">Profile</span></span>

* <span data-ttu-id="aae04-592">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="aae04-592">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-593">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-593">RDBMS</span></span>

* <span data-ttu-id="aae04-594">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-594">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="aae04-595">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-595">March 10, 2020</span></span>

<span data-ttu-id="aae04-596">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="aae04-596">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-597">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-597">ACR</span></span>

* <span data-ttu-id="aae04-598">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-598">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="aae04-599">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="aae04-599">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="aae04-600">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="aae04-600">Add private link and CMK support</span></span>
* <span data-ttu-id="aae04-601">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="aae04-601">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-602">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-602">AKS</span></span>

* <span data-ttu-id="aae04-603">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aae04-603">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="aae04-604">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="aae04-604">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="aae04-605">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-605">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="aae04-606">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-606">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="aae04-607">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="aae04-607">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="aae04-608">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-608">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="aae04-609">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-609">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="aae04-610">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="aae04-610">add missing / in the dashboard url</span></span>
* <span data-ttu-id="aae04-611">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="aae04-611">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="aae04-612">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="aae04-612">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="aae04-613">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="aae04-613">az aks: Add aad session key support</span></span>
* <span data-ttu-id="aae04-614">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="aae04-614">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="aae04-615">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="aae04-615">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-616">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-616">AppConfig</span></span>

* <span data-ttu-id="aae04-617">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="aae04-617">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-618">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-618">AppService</span></span>

* <span data-ttu-id="aae04-619">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="aae04-619">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="aae04-620">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="aae04-620">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="aae04-621">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="aae04-621">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="aae04-622">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-622">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="aae04-623">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-623">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="aae04-624">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="aae04-624">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-625">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-625">ARM</span></span>

* <span data-ttu-id="aae04-626">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-626">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="aae04-627">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="aae04-627">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="aae04-628">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="aae04-628">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="aae04-629">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="aae04-629">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="aae04-630">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="aae04-630">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="aae04-631">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="aae04-631">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="aae04-632">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-632">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="aae04-633">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="aae04-633">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="aae04-634">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="aae04-634">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="aae04-635">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="aae04-635">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-636">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-636">CDN</span></span>

* <span data-ttu-id="aae04-637">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-637">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-638">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-638">Compute</span></span>

* <span data-ttu-id="aae04-639">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="aae04-639">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="aae04-640">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="aae04-640">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="aae04-641">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="aae04-641">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="aae04-642">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="aae04-642">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="aae04-643">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="aae04-643">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-644">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-644">Cosmos DB</span></span>

* <span data-ttu-id="aae04-645">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="aae04-645">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="aae04-646">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="aae04-646">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-647">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-647">KeyVault</span></span>

* <span data-ttu-id="aae04-648">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-648">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-649">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-649">Monitor</span></span>

* <span data-ttu-id="aae04-650">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="aae04-650">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-651">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-651">Network</span></span>

* <span data-ttu-id="aae04-652">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="aae04-652">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="aae04-653">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="aae04-653">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="aae04-654">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="aae04-654">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="aae04-655">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="aae04-655">az network bastion: support bastion</span></span>
* <span data-ttu-id="aae04-656">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="aae04-656">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="aae04-657">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="aae04-657">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="aae04-658">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-658">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="aae04-659">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="aae04-659">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="aae04-660">Política</span><span class="sxs-lookup"><span data-stu-id="aae04-660">Policy</span></span>

* <span data-ttu-id="aae04-661">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="aae04-661">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-662">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-662">RBAC</span></span>

* <span data-ttu-id="aae04-663">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="aae04-663">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-664">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-664">RDBMS</span></span>

* <span data-ttu-id="aae04-665">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-665">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="aae04-666">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="aae04-666">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="aae04-667">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="aae04-667">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="aae04-668">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-668">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="aae04-669">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-669">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="aae04-670">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="aae04-670">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="aae04-671">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="aae04-671">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="aae04-672">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-672">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-673">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-673">SQL</span></span>

* <span data-ttu-id="aae04-674">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="aae04-674">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="aae04-675">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="aae04-675">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="aae04-676">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="aae04-676">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="aae04-677">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-677">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-678">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-678">Storage</span></span>

* <span data-ttu-id="aae04-679">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="aae04-679">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="aae04-680">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="aae04-680">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="aae04-681">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="aae04-681">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="aae04-682">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-682">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="aae04-683">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="aae04-683">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="aae04-684">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-684">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="aae04-685">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="aae04-685">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="aae04-686">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="aae04-686">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="aae04-687">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="aae04-687">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="aae04-688">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-688">February 18, 2020</span></span>

<span data-ttu-id="aae04-689">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="aae04-689">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-690">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-690">ACR</span></span>

* <span data-ttu-id="aae04-691">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="aae04-691">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="aae04-692">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="aae04-692">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="aae04-693">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="aae04-693">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-694">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-694">ACS</span></span>

* <span data-ttu-id="aae04-695">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="aae04-695">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="aae04-696">Aladdin</span><span class="sxs-lookup"><span data-stu-id="aae04-696">Aladdin</span></span>

* <span data-ttu-id="aae04-697">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="aae04-697">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-698">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-698">AMS</span></span>

* <span data-ttu-id="aae04-699">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="aae04-699">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-700">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-700">AppConfig</span></span>

* <span data-ttu-id="aae04-701">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="aae04-701">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="aae04-702">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="aae04-702">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="aae04-703">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="aae04-703">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-704">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-704">AppService</span></span>

* <span data-ttu-id="aae04-705">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="aae04-705">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="aae04-706">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="aae04-706">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="aae04-707">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="aae04-707">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-708">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-708">ARM</span></span>

* <span data-ttu-id="aae04-709">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="aae04-709">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="aae04-710">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="aae04-710">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-711">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-711">Backup</span></span>

* <span data-ttu-id="aae04-712">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="aae04-712">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="aae04-713">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="aae04-713">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-714">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-714">Compute</span></span>

* <span data-ttu-id="aae04-715">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="aae04-715">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="aae04-716">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="aae04-716">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="aae04-717">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="aae04-717">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="aae04-718">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="aae04-718">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="aae04-719">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="aae04-719">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="aae04-720">Eventhub</span><span class="sxs-lookup"><span data-stu-id="aae04-720">Eventhub</span></span>

* <span data-ttu-id="aae04-721">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="aae04-721">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-722">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-722">KeyVault</span></span>

* <span data-ttu-id="aae04-723">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="aae04-723">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="aae04-724">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="aae04-724">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="aae04-725">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="aae04-725">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="aae04-726">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-726">Network</span></span>

* <span data-ttu-id="aae04-727">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-727">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="aae04-728">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="aae04-728">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="aae04-729">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="aae04-729">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-730">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-730">Packaging</span></span>

* <span data-ttu-id="aae04-731">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="aae04-731">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-732">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-732">Profile</span></span>

* <span data-ttu-id="aae04-733">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="aae04-733">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="aae04-734">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="aae04-734">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="aae04-735">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="aae04-735">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="aae04-736">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="aae04-736">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="aae04-737">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-737">Role</span></span>

* <span data-ttu-id="aae04-738">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="aae04-738">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-739">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-739">SQL</span></span>

* <span data-ttu-id="aae04-740">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="aae04-740">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-741">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-741">Storage</span></span>

* <span data-ttu-id="aae04-742">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="aae04-742">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="aae04-743">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-743">February 04, 2020</span></span>

<span data-ttu-id="aae04-744">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="aae04-744">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-745">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-745">ACS</span></span>

* <span data-ttu-id="aae04-746">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="aae04-746">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="aae04-747">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="aae04-747">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-748">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-748">ACR</span></span>

* <span data-ttu-id="aae04-749">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="aae04-749">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="aae04-750">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="aae04-750">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="aae04-751">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="aae04-751">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-752">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-752">AKS</span></span>

* <span data-ttu-id="aae04-753">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="aae04-753">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-754">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-754">AppConfig</span></span>

* <span data-ttu-id="aae04-755">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="aae04-755">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="aae04-756">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="aae04-756">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="aae04-757">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="aae04-757">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="aae04-758">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="aae04-758">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="aae04-759">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="aae04-759">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-760">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-760">AppService</span></span>

* <span data-ttu-id="aae04-761">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="aae04-761">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="aae04-762">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-762">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-763">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-763">ARM</span></span>

* <span data-ttu-id="aae04-764">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-764">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="aae04-765">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="aae04-765">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="aae04-766">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="aae04-766">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="aae04-767">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="aae04-767">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="aae04-768">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="aae04-768">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="aae04-769">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-769">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="aae04-770">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-770">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-771">BotService</span><span class="sxs-lookup"><span data-stu-id="aae04-771">BotService</span></span>

* <span data-ttu-id="aae04-772">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="aae04-772">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="aae04-773">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="aae04-773">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-774">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-774">CDN</span></span>

* <span data-ttu-id="aae04-775">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="aae04-775">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="aae04-776">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="aae04-776">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="aae04-777">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="aae04-777">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="aae04-778">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-778">Deployment Manager</span></span>

* <span data-ttu-id="aae04-779">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="aae04-779">Add list operation for all resources.</span></span>
* <span data-ttu-id="aae04-780">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="aae04-780">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="aae04-781">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="aae04-781">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-782">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-782">IoT</span></span>

* <span data-ttu-id="aae04-783">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="aae04-783">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="aae04-784">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-784">IoT Central</span></span>

* <span data-ttu-id="aae04-785">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="aae04-785">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-786">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-786">Key Vault</span></span>

* <span data-ttu-id="aae04-787">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="aae04-787">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="aae04-788">Diversos</span><span class="sxs-lookup"><span data-stu-id="aae04-788">Misc</span></span>

* <span data-ttu-id="aae04-789">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="aae04-789">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="aae04-790">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-790">Network</span></span>

* <span data-ttu-id="aae04-791">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="aae04-791">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="aae04-792">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="aae04-792">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="aae04-793">Política</span><span class="sxs-lookup"><span data-stu-id="aae04-793">Policy</span></span>

* <span data-ttu-id="aae04-794">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="aae04-794">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="aae04-795">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="aae04-795">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-796">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-796">Profile</span></span>

* <span data-ttu-id="aae04-797">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-797">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-798">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-798">RBAC</span></span>

* <span data-ttu-id="aae04-799">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="aae04-799">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="aae04-800">Segurança</span><span class="sxs-lookup"><span data-stu-id="aae04-800">Security</span></span>

* <span data-ttu-id="aae04-801">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-801">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-802">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-802">SQL</span></span>

* <span data-ttu-id="aae04-803">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="aae04-803">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="aae04-804">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="aae04-804">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="aae04-805">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="aae04-805">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="aae04-806">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="aae04-806">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="aae04-807">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="aae04-807">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="aae04-808">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="aae04-808">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-809">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-809">Storage</span></span>

* <span data-ttu-id="aae04-810">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="aae04-810">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="aae04-811">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="aae04-811">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="aae04-812">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="aae04-812">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="aae04-813">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="aae04-813">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="aae04-814">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="aae04-814">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="aae04-815">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="aae04-815">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aae04-816">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aae04-816">ServiceFabric</span></span>

* <span data-ttu-id="aae04-817">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="aae04-817">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="aae04-818">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-818">January 13, 2020</span></span>

<span data-ttu-id="aae04-819">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="aae04-819">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-820">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-820">Compute</span></span>

* <span data-ttu-id="aae04-821">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="aae04-821">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="aae04-822">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="aae04-822">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-823">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-823">Storage</span></span>

* <span data-ttu-id="aae04-824">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="aae04-824">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="aae04-825">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="aae04-825">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="aae04-826">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-826">January 07, 2020</span></span>

<span data-ttu-id="aae04-827">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="aae04-827">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-828">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-828">ACR</span></span>

* <span data-ttu-id="aae04-829">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="aae04-829">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="aae04-830">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="aae04-830">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-831">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-831">AppConfig</span></span>

* <span data-ttu-id="aae04-832">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-832">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="aae04-833">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-833">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="aae04-834">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="aae04-834">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-835">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-835">AppService</span></span>

* <span data-ttu-id="aae04-836">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="aae04-836">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="aae04-837">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="aae04-837">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="aae04-838">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="aae04-838">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-839">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-839">ARM</span></span>

* <span data-ttu-id="aae04-840">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="aae04-840">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-841">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-841">Backup</span></span>

* <span data-ttu-id="aae04-842">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="aae04-842">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="aae04-843">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="aae04-843">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="aae04-844">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="aae04-844">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-845">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-845">Compute</span></span>

* <span data-ttu-id="aae04-846">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="aae04-846">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="aae04-847">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="aae04-847">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="aae04-848">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="aae04-848">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-849">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-849">HDInsight</span></span>

* <span data-ttu-id="aae04-850">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="aae04-850">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="aae04-851">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="aae04-851">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="aae04-852">Diversos.</span><span class="sxs-lookup"><span data-stu-id="aae04-852">Misc.</span></span>

* <span data-ttu-id="aae04-853">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="aae04-853">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="aae04-854">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-854">Event Hubs</span></span>

* <span data-ttu-id="aae04-855">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="aae04-855">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="aae04-856">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="aae04-856">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="aae04-857">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-857">Service Bus</span></span>

* <span data-ttu-id="aae04-858">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="aae04-858">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="aae04-859">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="aae04-859">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-860">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-860">RBAC</span></span>

* <span data-ttu-id="aae04-861">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="aae04-861">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-862">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-862">Storage</span></span>

* <span data-ttu-id="aae04-863">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="aae04-863">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="aae04-864">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="aae04-864">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="aae04-865">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="aae04-865">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="aae04-866">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-866">December 17, 2019</span></span>

<span data-ttu-id="aae04-867">2.0.78</span><span class="sxs-lookup"><span data-stu-id="aae04-867">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-868">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-868">ACR</span></span>

* <span data-ttu-id="aae04-869">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="aae04-869">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-870">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-870">ACS</span></span>

* <span data-ttu-id="aae04-871">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="aae04-871">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-872">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-872">AMS</span></span>

* <span data-ttu-id="aae04-873">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="aae04-873">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-874">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-874">AppConfig</span></span>

* <span data-ttu-id="aae04-875">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="aae04-875">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="aae04-876">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="aae04-876">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="aae04-877">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="aae04-877">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-878">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-878">AppService</span></span>

* <span data-ttu-id="aae04-879">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="aae04-879">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="aae04-880">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="aae04-880">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="aae04-881">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="aae04-881">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="aae04-882">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="aae04-882">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-883">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-883">ARM</span></span>

* <span data-ttu-id="aae04-884">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-884">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="aae04-885">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="aae04-885">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="aae04-886">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="aae04-886">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-887">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-887">Backup</span></span>

* <span data-ttu-id="aae04-888">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="aae04-888">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-889">BotService</span><span class="sxs-lookup"><span data-stu-id="aae04-889">BotService</span></span>

* <span data-ttu-id="aae04-890">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="aae04-890">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="aae04-891">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="aae04-891">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="aae04-892">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="aae04-892">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="aae04-893">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="aae04-893">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="aae04-894">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="aae04-894">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="aae04-895">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="aae04-895">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="aae04-896">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="aae04-896">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="aae04-897">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="aae04-897">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="aae04-898">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="aae04-898">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-899">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-899">Compute</span></span>

* <span data-ttu-id="aae04-900">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-900">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="aae04-901">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-901">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="aae04-902">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-902">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="aae04-903">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="aae04-903">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="aae04-904">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="aae04-904">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="aae04-905">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="aae04-905">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="aae04-906">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-906">Core</span></span>

* <span data-ttu-id="aae04-907">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="aae04-907">Removed support for Python 3.4</span></span>
* <span data-ttu-id="aae04-908">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-908">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="aae04-909">DLS</span><span class="sxs-lookup"><span data-stu-id="aae04-909">DLS</span></span>

* <span data-ttu-id="aae04-910">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="aae04-910">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="aae04-911">Instalar</span><span class="sxs-lookup"><span data-stu-id="aae04-911">Install</span></span>

* <span data-ttu-id="aae04-912">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="aae04-912">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-913">IOT</span><span class="sxs-lookup"><span data-stu-id="aae04-913">IOT</span></span>

* <span data-ttu-id="aae04-914">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="aae04-914">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="aae04-915">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="aae04-915">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-916">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-916">Key Vault</span></span>

* <span data-ttu-id="aae04-917">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-917">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="aae04-918">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="aae04-918">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="aae04-919">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="aae04-919">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="aae04-920">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="aae04-920">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="aae04-921">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="aae04-921">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-922">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-922">Network</span></span>

* <span data-ttu-id="aae04-923">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="aae04-923">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="aae04-924">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-924">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="aae04-925">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-925">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="aae04-926">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-926">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="aae04-927">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="aae04-927">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-928">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-928">Packaging</span></span>

* <span data-ttu-id="aae04-929">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="aae04-929">Added back edge builds for pip install</span></span>
* <span data-ttu-id="aae04-930">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-930">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="aae04-931">Política</span><span class="sxs-lookup"><span data-stu-id="aae04-931">Policy</span></span>

* <span data-ttu-id="aae04-932">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="aae04-932">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="aae04-933">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="aae04-933">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-934">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-934">Redis</span></span>

* <span data-ttu-id="aae04-935">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="aae04-935">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="aae04-936">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="aae04-936">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aae04-937">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aae04-937">ServiceFabric</span></span>

* <span data-ttu-id="aae04-938">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-938">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="aae04-939">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="aae04-939">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-940">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-940">SQL</span></span>

* <span data-ttu-id="aae04-941">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="aae04-941">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-942">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-942">Storage</span></span>

* <span data-ttu-id="aae04-943">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-943">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="aae04-944">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="aae04-944">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="aae04-945">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-945">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="aae04-946">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="aae04-946">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="aae04-947">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="aae04-947">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="aae04-948">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-948">November 26, 2019</span></span>

<span data-ttu-id="aae04-949">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="aae04-949">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-950">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-950">ACR</span></span>

* <span data-ttu-id="aae04-951">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-951">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="aae04-952">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-952">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="aae04-953">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-953">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="aae04-954">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-954">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-955">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-955">AKS</span></span>

* <span data-ttu-id="aae04-956">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="aae04-956">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-957">AppConfig</span></span>

* <span data-ttu-id="aae04-958">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="aae04-958">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="aae04-959">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="aae04-959">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="aae04-960">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="aae04-960">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="aae04-961">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-961">AppService</span></span>

* <span data-ttu-id="aae04-962">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-962">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="aae04-963">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="aae04-963">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="aae04-964">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="aae04-964">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-965">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-965">Backup</span></span>

* <span data-ttu-id="aae04-966">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="aae04-966">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="aae04-967">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="aae04-967">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-968">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-968">Compute</span></span>

* <span data-ttu-id="aae04-969">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="aae04-969">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="aae04-970">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="aae04-970">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="aae04-971">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="aae04-971">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="aae04-972">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="aae04-972">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="aae04-973">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-973">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="aae04-974">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="aae04-974">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="aae04-975">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-975">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="aae04-976">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="aae04-976">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="aae04-977">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="aae04-977">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="aae04-978">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="aae04-978">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-979">IOT</span><span class="sxs-lookup"><span data-stu-id="aae04-979">IOT</span></span>

* <span data-ttu-id="aae04-980">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="aae04-980">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="aae04-981">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-981">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="aae04-982">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="aae04-982">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-983">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-983">Key Vault</span></span>

* <span data-ttu-id="aae04-984">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="aae04-984">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aae04-985">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aae04-985">NetAppFiles</span></span>

* <span data-ttu-id="aae04-986">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="aae04-986">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="aae04-987">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-987">Network</span></span>

* <span data-ttu-id="aae04-988">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-988">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="aae04-989">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-989">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="aae04-990">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="aae04-990">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="aae04-991">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="aae04-991">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="aae04-992">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="aae04-992">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="aae04-993">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="aae04-993">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="aae04-994">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="aae04-994">Packaging</span></span>

* <span data-ttu-id="aae04-995">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="aae04-995">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="aae04-996">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="aae04-996">Added support for Python 3.8</span></span>
* <span data-ttu-id="aae04-997">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="aae04-997">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-998">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-998">Profile</span></span>

* <span data-ttu-id="aae04-999">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="aae04-999">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="aae04-1000">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="aae04-1000">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="aae04-1001">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="aae04-1001">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="aae04-1002">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="aae04-1002">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="aae04-1003">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="aae04-1003">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1004">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1004">RBAC</span></span>

* <span data-ttu-id="aae04-1005">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="aae04-1005">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-1006">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-1006">Redis</span></span>

* <span data-ttu-id="aae04-1007">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="aae04-1007">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="aae04-1008">Reservas</span><span class="sxs-lookup"><span data-stu-id="aae04-1008">Reservations</span></span>

* <span data-ttu-id="aae04-1009">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="aae04-1009">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="aae04-1010">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="aae04-1010">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="aae04-1011">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="aae04-1011">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="aae04-1012">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="aae04-1012">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="aae04-1013">Rest</span><span class="sxs-lookup"><span data-stu-id="aae04-1013">Rest</span></span>
* <span data-ttu-id="aae04-1014">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="aae04-1014">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1015">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1015">SQL</span></span>

* <span data-ttu-id="aae04-1016">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="aae04-1016">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1017">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1017">Storage</span></span>

* <span data-ttu-id="aae04-1018">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="aae04-1018">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="aae04-1019">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="aae04-1019">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="aae04-1020">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="aae04-1020">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="aae04-1021">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="aae04-1021">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="aae04-1022">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1022">November 4, 2019</span></span>

<span data-ttu-id="aae04-1023">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="aae04-1023">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1024">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1024">ACR</span></span>

* <span data-ttu-id="aae04-1025">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1025">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="aae04-1026">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="aae04-1026">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="aae04-1027">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="aae04-1027">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-1028">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1028">AKS</span></span>

* <span data-ttu-id="aae04-1029">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="aae04-1029">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="aae04-1030">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="aae04-1030">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="aae04-1031">AppConfig</span><span class="sxs-lookup"><span data-stu-id="aae04-1031">AppConfig</span></span>

* <span data-ttu-id="aae04-1032">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="aae04-1032">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="aae04-1033">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="aae04-1033">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="aae04-1034">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="aae04-1034">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1035">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1035">AppService</span></span>

* <span data-ttu-id="aae04-1036">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="aae04-1036">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="aae04-1037">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1037">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="aae04-1038">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="aae04-1038">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="aae04-1039">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-1039">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="aae04-1040">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1040">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-1041">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-1041">ARM</span></span>

* <span data-ttu-id="aae04-1042">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="aae04-1042">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="aae04-1043">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="aae04-1043">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-1044">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-1044">Backup</span></span>

* <span data-ttu-id="aae04-1045">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-1045">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-1046">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1046">Compute</span></span>

* <span data-ttu-id="aae04-1047">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="aae04-1047">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="aae04-1048">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="aae04-1048">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="aae04-1049">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="aae04-1049">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="aae04-1050">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-1050">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="aae04-1051">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="aae04-1051">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="aae04-1052">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1052">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="aae04-1053">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="aae04-1053">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="aae04-1054">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="aae04-1054">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1055">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1055">CosmosDB</span></span>

* <span data-ttu-id="aae04-1056">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="aae04-1056">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="aae04-1057">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="aae04-1057">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="aae04-1058">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1058">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="aae04-1059">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="aae04-1059">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="aae04-1060">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1060">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="aae04-1061">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="aae04-1061">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="aae04-1062">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-1062">Fixed typo in help message</span></span>
* <span data-ttu-id="aae04-1063">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-1063">database: Added deprecation information</span></span>
* <span data-ttu-id="aae04-1064">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-1064">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1065">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1065">IoT</span></span>

* <span data-ttu-id="aae04-1066">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="aae04-1066">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="aae04-1067">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1067">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-1068">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-1068">Key Vault</span></span>

* <span data-ttu-id="aae04-1069">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="aae04-1069">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="aae04-1070">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-1070">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="aae04-1071">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="aae04-1071">NetAppFiles</span></span>

* <span data-ttu-id="aae04-1072">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="aae04-1072">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="aae04-1073">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="aae04-1073">This new API version includes:</span></span>

    - <span data-ttu-id="aae04-1074">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="aae04-1074">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="aae04-1075">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="aae04-1075">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="aae04-1076">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="aae04-1076">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="aae04-1077">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="aae04-1077">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1078">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1078">Network</span></span>

* <span data-ttu-id="aae04-1079">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="aae04-1079">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="aae04-1080">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="aae04-1080">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="aae04-1081">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="aae04-1081">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="aae04-1082">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="aae04-1082">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="aae04-1083">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="aae04-1083">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="aae04-1084">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="aae04-1084">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-1085">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-1085">Profile</span></span>

* <span data-ttu-id="aae04-1086">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-1086">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="aae04-1087">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="aae04-1087">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1088">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1088">RBAC</span></span>

* <span data-ttu-id="aae04-1089">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-1089">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aae04-1090">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aae04-1090">ServiceFabric</span></span>

* <span data-ttu-id="aae04-1091">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-1091">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1092">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1092">SQL</span></span>

* <span data-ttu-id="aae04-1093">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="aae04-1093">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1094">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1094">Storage</span></span>

* <span data-ttu-id="aae04-1095">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-1095">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="aae04-1096">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-1096">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="aae04-1097">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1097">October 15, 2019</span></span>

<span data-ttu-id="aae04-1098">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="aae04-1098">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-1099">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1099">AKS</span></span>

* <span data-ttu-id="aae04-1100">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-1100">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="aae04-1101">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-1101">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1102">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1102">AMS</span></span>

* <span data-ttu-id="aae04-1103">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1103">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="aae04-1104">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="aae04-1104">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1105">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1105">AppService</span></span>

* <span data-ttu-id="aae04-1106">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="aae04-1106">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="aae04-1107">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1107">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="aae04-1108">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1108">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-1109">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-1109">ARM</span></span>

* <span data-ttu-id="aae04-1110">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="aae04-1110">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-1111">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1111">Compute</span></span>

* <span data-ttu-id="aae04-1112">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1112">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="aae04-1113">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="aae04-1113">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="aae04-1114">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-1114">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="aae04-1115">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-1115">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="aae04-1116">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="aae04-1116">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="aae04-1117">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="aae04-1117">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1118">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1118">Core</span></span>

* <span data-ttu-id="aae04-1119">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="aae04-1119">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1120">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1120">IoT</span></span>

* <span data-ttu-id="aae04-1121">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="aae04-1121">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1122">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1122">Monitor</span></span>

* <span data-ttu-id="aae04-1123">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="aae04-1123">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1124">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1124">Network</span></span>

* <span data-ttu-id="aae04-1125">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1125">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="aae04-1126">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-1126">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1127">SQL</span></span>

* <span data-ttu-id="aae04-1128">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="aae04-1128">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1129">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1129">Storage</span></span>

* <span data-ttu-id="aae04-1130">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-1130">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="aae04-1131">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1131">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="aae04-1132">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1132">September 24, 2019</span></span>

<span data-ttu-id="aae04-1133">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="aae04-1133">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1134">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1134">ACR</span></span>

* <span data-ttu-id="aae04-1135">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1135">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="aae04-1136">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="aae04-1136">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-1137">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1137">AKS</span></span>

* <span data-ttu-id="aae04-1138">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="aae04-1138">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="aae04-1139">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="aae04-1139">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="aae04-1140">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="aae04-1140">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-1141">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-1141">ARM</span></span>

* <span data-ttu-id="aae04-1142">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="aae04-1142">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-1143">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1143">Compute</span></span>

* <span data-ttu-id="aae04-1144">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="aae04-1144">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="aae04-1145">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="aae04-1145">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="aae04-1146">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1146">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="aae04-1147">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="aae04-1147">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="aae04-1148">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1148">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-1149">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-1149">Cosmos DB</span></span>

* <span data-ttu-id="aae04-1150">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="aae04-1150">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="aae04-1151">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="aae04-1151">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="aae04-1152">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-1152">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aae04-1153">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aae04-1153">EventGrid</span></span>

* <span data-ttu-id="aae04-1154">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="aae04-1154">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-1155">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-1155">Key Vault</span></span>

* <span data-ttu-id="aae04-1156">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1156">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1157">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1157">Monitor</span></span>

* <span data-ttu-id="aae04-1158">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1158">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="aae04-1159">Política</span><span class="sxs-lookup"><span data-stu-id="aae04-1159">Policy</span></span>

* <span data-ttu-id="aae04-1160">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1160">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="aae04-1161">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1161">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1162">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1162">Storage</span></span>

* <span data-ttu-id="aae04-1163">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1163">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="aae04-1164">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1164">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1165">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1165">ACR</span></span>

* <span data-ttu-id="aae04-1166">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="aae04-1166">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-1167">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1167">AKS</span></span>

* <span data-ttu-id="aae04-1168">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="aae04-1168">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="aae04-1169">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1169">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="aae04-1170">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1170">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-1171">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-1171">ARM</span></span>

* <span data-ttu-id="aae04-1172">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="aae04-1172">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1173">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1173">Batch</span></span>

* <span data-ttu-id="aae04-1174">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-1174">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="aae04-1175">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="aae04-1175">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="aae04-1176">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="aae04-1176">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="aae04-1177">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="aae04-1177">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="aae04-1178">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="aae04-1178">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="aae04-1179">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="aae04-1179">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="aae04-1180">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="aae04-1180">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1181">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1181">HDInsight</span></span>

* <span data-ttu-id="aae04-1182">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="aae04-1182">GA release</span></span>
* <span data-ttu-id="aae04-1183">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aae04-1183">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-1184">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-1184">Key Vault</span></span>

* <span data-ttu-id="aae04-1185">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1185">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="aae04-1186">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1186">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1187">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1187">Network</span></span>

* <span data-ttu-id="aae04-1188">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="aae04-1188">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="aae04-1189">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="aae04-1189">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="aae04-1190">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="aae04-1190">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="aae04-1191">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1191">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="aae04-1192">Política</span><span class="sxs-lookup"><span data-stu-id="aae04-1192">Policy</span></span>

* <span data-ttu-id="aae04-1193">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="aae04-1193">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="aae04-1194">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1194">August 27, 2019</span></span>

<span data-ttu-id="aae04-1195">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="aae04-1195">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1196">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1196">ACR</span></span>

* <span data-ttu-id="aae04-1197">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="aae04-1197">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="aae04-1198">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="aae04-1198">API Management</span></span>

* <span data-ttu-id="aae04-1199">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="aae04-1199">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1200">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1200">AppService</span></span>

* <span data-ttu-id="aae04-1201">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="aae04-1201">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="aae04-1202">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-1202">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-1203">Keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-1203">Keyvault</span></span>

* <span data-ttu-id="aae04-1204">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="aae04-1204">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1205">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1205">Network</span></span>

* <span data-ttu-id="aae04-1206">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="aae04-1206">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="aae04-1207">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="aae04-1207">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="aae04-1208">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="aae04-1208">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="aae04-1209">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1209">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1210">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1210">RBAC</span></span>

* <span data-ttu-id="aae04-1211">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="aae04-1211">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aae04-1212">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aae04-1212">ServiceFabric</span></span>

* <span data-ttu-id="aae04-1213">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-1213">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="aae04-1214">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-1214">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="aae04-1215">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="aae04-1215">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="aae04-1216">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="aae04-1216">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="aae04-1217">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-1217">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="aae04-1218">SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-1218">SignalR</span></span>

* <span data-ttu-id="aae04-1219">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="aae04-1219">Added new commands:</span></span>
  * <span data-ttu-id="aae04-1220">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-1220">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="aae04-1221">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-1221">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="aae04-1222">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-1222">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="aae04-1223">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1223">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1224">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1224">Storage</span></span>

* <span data-ttu-id="aae04-1225">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="aae04-1225">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="aae04-1226">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1226">August 13, 2019</span></span>

<span data-ttu-id="aae04-1227">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="aae04-1227">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1228">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1228">AppService</span></span>

* <span data-ttu-id="aae04-1229">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-1229">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1230">BotService</span><span class="sxs-lookup"><span data-stu-id="aae04-1230">BotService</span></span>

* <span data-ttu-id="aae04-1231">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1231">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="aae04-1232">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="aae04-1232">CognitiveServices</span></span>

* <span data-ttu-id="aae04-1233">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1233">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-1234">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-1234">Cosmos DB</span></span>

* <span data-ttu-id="aae04-1235">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="aae04-1235">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="aae04-1236">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1236">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1237">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1237">HDInsight</span></span>

<span data-ttu-id="aae04-1238">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="aae04-1238">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="aae04-1239">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-1239">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="aae04-1240">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="aae04-1240">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="aae04-1241">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="aae04-1241">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="aae04-1242">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-1242">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="aae04-1243">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="aae04-1243">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="aae04-1244">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-1244">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="aae04-1245">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="aae04-1245">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="aae04-1246">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="aae04-1246">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="aae04-1247">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="aae04-1247">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="aae04-1248">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="aae04-1248">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="aae04-1249">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-1249">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="aae04-1250">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="aae04-1250">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="aae04-1251">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="aae04-1251">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="aae04-1252">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="aae04-1252">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="aae04-1253">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="aae04-1253">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="aae04-1254">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="aae04-1254">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="aae04-1255">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="aae04-1255">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="aae04-1256">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1256">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="aae04-1257">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="aae04-1257">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="aae04-1258">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="aae04-1258">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="aae04-1259">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-1259">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="aae04-1260">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-1260">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="aae04-1261">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="aae04-1261">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-1262">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1262">Interactive</span></span>

* <span data-ttu-id="aae04-1263">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-1263">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="aae04-1264">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-1264">Kubernetes</span></span>

* <span data-ttu-id="aae04-1265">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="aae04-1265">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1266">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1266">Network</span></span>

* <span data-ttu-id="aae04-1267">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-1267">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-1268">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-1268">Profile</span></span>

* <span data-ttu-id="aae04-1269">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1269">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="aae04-1270">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="aae04-1270">ServiceFabric</span></span>

* <span data-ttu-id="aae04-1271">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="aae04-1271">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="aae04-1272">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="aae04-1272">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1273">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1273">Storage</span></span>

* <span data-ttu-id="aae04-1274">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1274">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="aae04-1275">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1275">July 30, 2019</span></span>

<span data-ttu-id="aae04-1276">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="aae04-1276">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1277">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1277">ACR</span></span>

* <span data-ttu-id="aae04-1278">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="aae04-1278">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="aae04-1279">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="aae04-1279">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1280">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1280">Appservice</span></span>

* <span data-ttu-id="aae04-1281">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="aae04-1281">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="aae04-1282">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="aae04-1282">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="aae04-1283">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="aae04-1283">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1284">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1284">Network</span></span>

* <span data-ttu-id="aae04-1285">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="aae04-1285">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="aae04-1286">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="aae04-1286">Fixes #9604.</span></span> <span data-ttu-id="aae04-1287">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="aae04-1287">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="aae04-1288">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="aae04-1288">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1289">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1289">RBAC</span></span>

* <span data-ttu-id="aae04-1290">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1290">Added `user update` command</span></span>
* <span data-ttu-id="aae04-1291">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-1291">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="aae04-1292">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="aae04-1292">Use replacement argument `--id`</span></span>
* <span data-ttu-id="aae04-1293">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-1293">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1294">SQL</span></span>

* <span data-ttu-id="aae04-1295">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="aae04-1295">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1296">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1296">Storage</span></span>

* <span data-ttu-id="aae04-1297">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="aae04-1297">Added `storage remove` command</span></span>
* <span data-ttu-id="aae04-1298">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1298">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1299">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1299">VM</span></span>

* <span data-ttu-id="aae04-1300">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="aae04-1300">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="aae04-1301">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1301">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="aae04-1302">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1302">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="aae04-1303">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="aae04-1303">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="aae04-1304">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1304">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="aae04-1305">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1305">July 16, 2019</span></span>

<span data-ttu-id="aae04-1306">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="aae04-1306">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1307">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1307">Appservice</span></span>

* <span data-ttu-id="aae04-1308">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="aae04-1308">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="aae04-1309">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-1309">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="aae04-1310">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1310">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1311">Core</span></span>

* <span data-ttu-id="aae04-1312">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="aae04-1312">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1313">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1313">Batch</span></span>

* <span data-ttu-id="aae04-1314">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="aae04-1314">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="aae04-1315">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="aae04-1315">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="aae04-1316">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1316">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="aae04-1317">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="aae04-1317">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aae04-1318">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-1318">Eventhubs</span></span>

* <span data-ttu-id="aae04-1319">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1319">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-1320">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1320">RDBMS</span></span>

* <span data-ttu-id="aae04-1321">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="aae04-1321">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="aae04-1322">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1322">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="aae04-1323">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="aae04-1323">Relay</span></span>

* <span data-ttu-id="aae04-1324">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="aae04-1324">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="aae04-1325">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1325">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="aae04-1326">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-1326">Servicebus</span></span>

* <span data-ttu-id="aae04-1327">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1327">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1328">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1328">Storage</span></span>

* <span data-ttu-id="aae04-1329">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1329">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="aae04-1330">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="aae04-1330">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="aae04-1331">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1331">July 2, 2019</span></span>

<span data-ttu-id="aae04-1332">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="aae04-1332">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1333">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1333">Core</span></span>

* <span data-ttu-id="aae04-1334">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="aae04-1334">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="aae04-1335">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="aae04-1335">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="aae04-1336">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="aae04-1336">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1337">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1337">ACR</span></span>

* <span data-ttu-id="aae04-1338">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="aae04-1338">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1339">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1339">Appservice</span></span>

* <span data-ttu-id="aae04-1340">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-1340">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="aae04-1341">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="aae04-1341">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="aae04-1342">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="aae04-1342">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="aae04-1343">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="aae04-1343">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-1344">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-1344">Cosmos DB</span></span>

* <span data-ttu-id="aae04-1345">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="aae04-1345">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="aae04-1346">DLS</span><span class="sxs-lookup"><span data-stu-id="aae04-1346">DLS</span></span>

* <span data-ttu-id="aae04-1347">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="aae04-1347">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="aae04-1348">Comentários</span><span class="sxs-lookup"><span data-stu-id="aae04-1348">Feedback</span></span>

* <span data-ttu-id="aae04-1349">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="aae04-1349">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1350">HDInsight</span></span>

* <span data-ttu-id="aae04-1351">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="aae04-1351">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="aae04-1352">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="aae04-1352">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="aae04-1353">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="aae04-1353">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="aae04-1354">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="aae04-1354">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="aae04-1355">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="aae04-1355">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="aae04-1356">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1356">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="aae04-1357">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="aae04-1357">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="aae04-1358">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="aae04-1358">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="aae04-1359">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1359">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="aae04-1360">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-1360">Managed Services</span></span>

* <span data-ttu-id="aae04-1361">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-1361">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-1362">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-1362">Profile</span></span>
* <span data-ttu-id="aae04-1363">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="aae04-1363">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1364">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1364">RBAC</span></span>

* <span data-ttu-id="aae04-1365">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="aae04-1365">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="aae04-1366">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="aae04-1366">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="aae04-1367">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="aae04-1367">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="aae04-1368">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-1368">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-1369">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1369">RDBMS</span></span>

* <span data-ttu-id="aae04-1370">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1370">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1371">SQL</span></span>

* <span data-ttu-id="aae04-1372">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-1372">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1373">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1373">Storage</span></span>

* <span data-ttu-id="aae04-1374">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="aae04-1374">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="aae04-1375">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="aae04-1375">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="aae04-1376">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1376">VM</span></span>

* <span data-ttu-id="aae04-1377">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-1377">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="aae04-1378">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1378">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="aae04-1379">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1379">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="aae04-1380">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="aae04-1380">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="aae04-1381">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1381">June 18, 2019</span></span>

<span data-ttu-id="aae04-1382">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="aae04-1382">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1383">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1383">Core</span></span>

<span data-ttu-id="aae04-1384">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="aae04-1384">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="aae04-1385">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="aae04-1385">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="aae04-1386">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="aae04-1386">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="aae04-1387">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="aae04-1387">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="aae04-1388">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="aae04-1388">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="aae04-1389">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="aae04-1389">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="aae04-1390">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="aae04-1390">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1391">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1391">ACR</span></span>
* <span data-ttu-id="aae04-1392">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="aae04-1392">Added 'acr check-health' command</span></span>
* <span data-ttu-id="aae04-1393">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="aae04-1393">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1394">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1394">ACS</span></span>
* <span data-ttu-id="aae04-1395">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-1395">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1396">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1396">AMS</span></span>
* <span data-ttu-id="aae04-1397">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="aae04-1397">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1398">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1398">AppService</span></span>
* <span data-ttu-id="aae04-1399">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="aae04-1399">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="aae04-1400">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aae04-1400">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="aae04-1401">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="aae04-1401">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="aae04-1402">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1402">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="aae04-1403">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="aae04-1403">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="aae04-1404">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="aae04-1404">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1405">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1405">Batch</span></span>
* <span data-ttu-id="aae04-1406">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="aae04-1406">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-1407">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aae04-1407">BatchAI</span></span>
* <span data-ttu-id="aae04-1408">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="aae04-1408">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1409">BotService</span><span class="sxs-lookup"><span data-stu-id="aae04-1409">BotService</span></span>
* <span data-ttu-id="aae04-1410">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="aae04-1410">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1411">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1411">CosmosDB</span></span>
* <span data-ttu-id="aae04-1412">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="aae04-1412">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="aae04-1413">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="aae04-1413">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="aae04-1414">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="aae04-1414">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="aae04-1415">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-1415">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aae04-1416">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aae04-1416">EventGrid</span></span>
* <span data-ttu-id="aae04-1417">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="aae04-1417">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="aae04-1418">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="aae04-1418">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="aae04-1419">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="aae04-1419">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="aae04-1420">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="aae04-1420">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="aae04-1421">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1421">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1422">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1422">HDInsight</span></span>
* <span data-ttu-id="aae04-1423">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1423">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1424">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1424">IoT</span></span>
* <span data-ttu-id="aae04-1425">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="aae04-1425">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="aae04-1426">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="aae04-1426">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1427">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1427">Network</span></span>
* <span data-ttu-id="aae04-1428">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="aae04-1428">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="aae04-1429">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="aae04-1429">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="aae04-1430">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="aae04-1430">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="aae04-1431">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="aae04-1431">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1432">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1432">Resource</span></span>
* <span data-ttu-id="aae04-1433">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="aae04-1433">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="aae04-1434">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="aae04-1434">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="aae04-1435">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aae04-1435">ServiceBus</span></span>
* <span data-ttu-id="aae04-1436">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="aae04-1436">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1437">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1437">SQL</span></span>
* <span data-ttu-id="aae04-1438">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="aae04-1438">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="aae04-1439">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="aae04-1439">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="aae04-1440">SQLVm</span><span class="sxs-lookup"><span data-stu-id="aae04-1440">SQLVm</span></span>
* <span data-ttu-id="aae04-1441">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="aae04-1441">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="aae04-1442">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1442">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1443">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1443">Storage</span></span>
* <span data-ttu-id="aae04-1444">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="aae04-1444">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="aae04-1445">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-1445">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1446">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1446">VM</span></span>
* <span data-ttu-id="aae04-1447">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1447">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="aae04-1448">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1448">June 4, 2019</span></span>

<span data-ttu-id="aae04-1449">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="aae04-1449">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1450">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1450">Core</span></span>
* <span data-ttu-id="aae04-1451">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="aae04-1451">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1452">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1452">ACR</span></span>
* <span data-ttu-id="aae04-1453">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="aae04-1453">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1454">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1454">ACS</span></span>
* <span data-ttu-id="aae04-1455">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1455">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="aae04-1456">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-1456">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1457">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1457">Batch</span></span>
* <span data-ttu-id="aae04-1458">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="aae04-1458">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1459">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1459">IoT</span></span>
* <span data-ttu-id="aae04-1460">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="aae04-1460">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1461">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1461">Network</span></span>
* <span data-ttu-id="aae04-1462">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="aae04-1462">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="aae04-1463">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1463">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="aae04-1464">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1464">Resource</span></span>
* <span data-ttu-id="aae04-1465">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="aae04-1465">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1466">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1466">Role</span></span>
* <span data-ttu-id="aae04-1467">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="aae04-1467">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-1468">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1468">Compute</span></span>
* <span data-ttu-id="aae04-1469">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="aae04-1469">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="aae04-1470">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1470">May 21, 2019</span></span>

<span data-ttu-id="aae04-1471">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="aae04-1471">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1472">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1472">Core</span></span>
* <span data-ttu-id="aae04-1473">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="aae04-1473">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="aae04-1474">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1474">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="aae04-1475">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="aae04-1475">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1476">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1476">ACR</span></span>
* <span data-ttu-id="aae04-1477">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="aae04-1477">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1478">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1478">ACS</span></span>
* <span data-ttu-id="aae04-1479">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="aae04-1479">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1480">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1480">AppService</span></span>
* <span data-ttu-id="aae04-1481">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="aae04-1481">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="aae04-1482">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="aae04-1482">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="aae04-1483">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="aae04-1483">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="aae04-1484">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="aae04-1484">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="aae04-1485">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1485">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="aae04-1486">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="aae04-1486">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="aae04-1487">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-1487">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1488">BotService</span><span class="sxs-lookup"><span data-stu-id="aae04-1488">BotService</span></span>
* <span data-ttu-id="aae04-1489">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-1489">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="aae04-1490">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="aae04-1490">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-1491">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-1491">Consumption</span></span>
* <span data-ttu-id="aae04-1492">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-1492">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1493">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1493">IoT</span></span>
* <span data-ttu-id="aae04-1494">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="aae04-1494">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1495">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1495">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="aae04-1497">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="aae04-1497">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="aae04-1498">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="aae04-1498">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-1499">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1499">RDBMS</span></span>
* <span data-ttu-id="aae04-1500">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="aae04-1500">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-1501">RBAC</span><span class="sxs-lookup"><span data-stu-id="aae04-1501">RBAC</span></span>
* <span data-ttu-id="aae04-1502">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="aae04-1502">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1503">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1503">Storage</span></span>
* <span data-ttu-id="aae04-1504">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="aae04-1504">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="aae04-1505">Computação</span><span class="sxs-lookup"><span data-stu-id="aae04-1505">Compute</span></span>
* <span data-ttu-id="aae04-1506">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1506">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="aae04-1507">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="aae04-1507">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="aae04-1508">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="aae04-1508">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="aae04-1509">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="aae04-1509">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="aae04-1510">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1510">May 6, 2019</span></span>

<span data-ttu-id="aae04-1511">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="aae04-1511">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1512">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1512">ACS</span></span>
* <span data-ttu-id="aae04-1513">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="aae04-1513">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="aae04-1514">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="aae04-1514">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="aae04-1515">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1515">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="aae04-1516">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1516">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1517">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1517">Appservice</span></span>
* <span data-ttu-id="aae04-1518">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-1518">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="aae04-1519">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="aae04-1519">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="aae04-1520">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1520">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="aae04-1521">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="aae04-1521">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="aae04-1522">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1522">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="aae04-1523">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="aae04-1523">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="aae04-1524">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-1524">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="aae04-1525">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="aae04-1525">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="aae04-1526">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-1526">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="aae04-1527">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="aae04-1527">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1528">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1528">Batch</span></span>
* <span data-ttu-id="aae04-1529">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="aae04-1529">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1530">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1530">Botservice</span></span>
* <span data-ttu-id="aae04-1531">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="aae04-1531">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="aae04-1532">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="aae04-1532">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="aae04-1533">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="aae04-1533">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="aae04-1534">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="aae04-1534">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="aae04-1535">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="aae04-1535">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="aae04-1536">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="aae04-1536">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="aae04-1537">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1537">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="aae04-1538">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="aae04-1538">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="aae04-1539">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="aae04-1539">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="aae04-1540">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="aae04-1540">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="aae04-1541">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1541">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="aae04-1542">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="aae04-1542">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="aae04-1543">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="aae04-1543">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="aae04-1544">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="aae04-1544">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="aae04-1545">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-1545">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="aae04-1546">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1546">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="aae04-1547">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1547">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="aae04-1548">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="aae04-1548">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="aae04-1549">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="aae04-1549">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="aae04-1550">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="aae04-1550">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="aae04-1551">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="aae04-1551">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="aae04-1552">Configurar</span><span class="sxs-lookup"><span data-stu-id="aae04-1552">Configure</span></span>
* <span data-ttu-id="aae04-1553">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="aae04-1553">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aae04-1554">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-1554">Eventhubs</span></span>
* <span data-ttu-id="aae04-1555">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1555">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="aae04-1556">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1556">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1557">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1557">Network</span></span>
* <span data-ttu-id="aae04-1558">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1558">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="aae04-1559">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="aae04-1559">Policy Insights</span></span>
* <span data-ttu-id="aae04-1560">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1560">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1561">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1561">Role</span></span>
* <span data-ttu-id="aae04-1562">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1562">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="aae04-1563">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-1563">Service Bus</span></span>
* <span data-ttu-id="aae04-1564">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1564">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="aae04-1565">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1565">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="aae04-1566">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="aae04-1566">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1567">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1567">SQL</span></span>
* <span data-ttu-id="aae04-1568">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1568">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1569">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1569">VM</span></span>
* <span data-ttu-id="aae04-1570">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-1570">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="aae04-1571">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-1571">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="aae04-1572">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-1572">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="aae04-1573">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="aae04-1573">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="aae04-1574">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="aae04-1574">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="aae04-1575">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1575">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="aae04-1576">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1576">April 23, 2019</span></span>

<span data-ttu-id="aae04-1577">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="aae04-1577">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1578">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1578">ACS</span></span>
* <span data-ttu-id="aae04-1579">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="aae04-1579">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="aae04-1580">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="aae04-1580">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1581">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1581">AMS</span></span>
* <span data-ttu-id="aae04-1582">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1582">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1583">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1583">AppService</span></span>
* <span data-ttu-id="aae04-1584">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="aae04-1584">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="aae04-1585">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="aae04-1585">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="aae04-1586">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="aae04-1586">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="aae04-1587">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="aae04-1587">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="aae04-1588">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="aae04-1588">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="aae04-1589">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-1589">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="aae04-1590">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="aae04-1590">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="aae04-1591">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="aae04-1591">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="aae04-1592">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="aae04-1592">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="aae04-1593">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-1593">Deployment Manager</span></span>
* <span data-ttu-id="aae04-1594">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="aae04-1594">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="aae04-1595">Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-1595">Lab</span></span>
* <span data-ttu-id="aae04-1596">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-1596">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1597">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1597">Network</span></span>
* <span data-ttu-id="aae04-1598">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="aae04-1598">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1599">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1599">Resource</span></span>
* <span data-ttu-id="aae04-1600">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="aae04-1600">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="aae04-1601">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="aae04-1601">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="aae04-1602">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="aae04-1602">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="aae04-1603">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="aae04-1603">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1604">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1604">SQL</span></span>
* <span data-ttu-id="aae04-1605">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="aae04-1605">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="aae04-1606">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1606">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="aae04-1607">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1607">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="aae04-1608">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-1608">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1609">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1609">Storage</span></span>
* <span data-ttu-id="aae04-1610">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="aae04-1610">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1611">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1611">VM</span></span>
* <span data-ttu-id="aae04-1612">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1612">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="aae04-1613">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="aae04-1613">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="aae04-1614">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="aae04-1614">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="aae04-1615">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1615">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1616">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1616">Core</span></span>
* <span data-ttu-id="aae04-1617">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="aae04-1617">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1618">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1618">ACR</span></span>
* <span data-ttu-id="aae04-1619">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="aae04-1619">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1620">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1620">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="aae04-1623">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1623">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="aae04-1624">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1624">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1625">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1625">AppService</span></span>
* <span data-ttu-id="aae04-1626">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1626">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="aae04-1627">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="aae04-1627">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="aae04-1628">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1628">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="aae04-1629">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="aae04-1629">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="aae04-1630">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-1630">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="aae04-1631">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="aae04-1631">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="aae04-1632">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="aae04-1632">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-1633">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-1633">CDN</span></span>
* <span data-ttu-id="aae04-1634">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="aae04-1634">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="aae04-1635">Comentários</span><span class="sxs-lookup"><span data-stu-id="aae04-1635">Feedback</span></span>
* <span data-ttu-id="aae04-1636">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="aae04-1636">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="aae04-1637">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="aae04-1637">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="aae04-1638">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="aae04-1638">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1639">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1639">Monitor</span></span>
* <span data-ttu-id="aae04-1640">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1640">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="aae04-1641">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1641">Network</span></span>
* <span data-ttu-id="aae04-1642">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="aae04-1642">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="aae04-1643">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-1643">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="aae04-1644">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="aae04-1644">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="aae04-1645">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1645">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="aae04-1646">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="aae04-1646">PrivateDNS</span></span>
* <span data-ttu-id="aae04-1647">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="aae04-1647">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1648">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1648">Resource</span></span>
* <span data-ttu-id="aae04-1649">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="aae04-1649">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1650">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1650">Role</span></span>
* <span data-ttu-id="aae04-1651">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="aae04-1651">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="aae04-1652">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="aae04-1652">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1653">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1653">SQL</span></span>
* <span data-ttu-id="aae04-1654">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="aae04-1654">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1655">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1655">Storage</span></span>
* <span data-ttu-id="aae04-1656">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-1656">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="aae04-1657">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="aae04-1657">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="aae04-1658">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="aae04-1658">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="aae04-1659">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="aae04-1659">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="aae04-1660">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1660">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="aae04-1661">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1661">Core</span></span>
* <span data-ttu-id="aae04-1662">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="aae04-1662">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="aae04-1663">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="aae04-1663">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="aae04-1664">Nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-1664">Cloud</span></span>
* <span data-ttu-id="aae04-1665">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="aae04-1665">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1666">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1666">ACR</span></span>
* <span data-ttu-id="aae04-1667">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="aae04-1667">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="aae04-1668">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1668">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="aae04-1669">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="aae04-1669">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="aae04-1670">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="aae04-1670">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1671">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1671">AppService</span></span>
* <span data-ttu-id="aae04-1672">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="aae04-1672">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="aae04-1673">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="aae04-1673">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="aae04-1674">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="aae04-1674">BOT Service</span></span>
* <span data-ttu-id="aae04-1675">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="aae04-1675">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="aae04-1676">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="aae04-1676">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="aae04-1677">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="aae04-1677">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="aae04-1678">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="aae04-1678">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-1679">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-1679">CDN</span></span>
* <span data-ttu-id="aae04-1680">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1680">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="aae04-1682">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="aae04-1682">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="aae04-1683">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-1683">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1684">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="aae04-1684">Cosmosdb</span></span>
* <span data-ttu-id="aae04-1685">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="aae04-1685">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="aae04-1686">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-1686">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-1687">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1687">Interactive</span></span>
* <span data-ttu-id="aae04-1688">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="aae04-1688">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1689">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1689">Monitor</span></span>
* <span data-ttu-id="aae04-1690">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1690">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1691">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1691">Network</span></span>
* <span data-ttu-id="aae04-1692">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="aae04-1692">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-1693">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-1693">Profile</span></span>
* <span data-ttu-id="aae04-1694">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="aae04-1694">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="aae04-1695">Postgres</span><span class="sxs-lookup"><span data-stu-id="aae04-1695">Postgres</span></span> 
* <span data-ttu-id="aae04-1696">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="aae04-1696">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="aae04-1697">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="aae04-1697">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1698">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1698">Resource</span></span>
* <span data-ttu-id="aae04-1699">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1699">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="aae04-1700">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="aae04-1700">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="aae04-1701">Grafo</span><span class="sxs-lookup"><span data-stu-id="aae04-1701">Graph</span></span>
* <span data-ttu-id="aae04-1702">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="aae04-1702">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="aae04-1703">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="aae04-1703">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="aae04-1704">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="aae04-1704">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="aae04-1705">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-1705">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="aae04-1706">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-1706">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1707">armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1707">storage</span></span>
* <span data-ttu-id="aae04-1708">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1708">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="aae04-1709">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="aae04-1709">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="aae04-1710">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="aae04-1710">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="aae04-1711">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="aae04-1711">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1712">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1712">VM</span></span>
* <span data-ttu-id="aae04-1713">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1713">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="aae04-1714">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1714">March 12, 2019</span></span>

<span data-ttu-id="aae04-1715">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="aae04-1715">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1716">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1716">Core</span></span>

* <span data-ttu-id="aae04-1717">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="aae04-1717">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1718">ACR</span></span>

* <span data-ttu-id="aae04-1719">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="aae04-1719">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1720">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1720">ACS</span></span>

* <span data-ttu-id="aae04-1721">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="aae04-1721">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="aae04-1722">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1722">AppService</span></span>

* <span data-ttu-id="aae04-1723">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="aae04-1723">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="aae04-1724">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1724">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="aae04-1725">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="aae04-1725">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="aae04-1726">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="aae04-1726">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1727">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1727">Botservice</span></span>

* <span data-ttu-id="aae04-1728">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="aae04-1728">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="aae04-1729">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="aae04-1729">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="aae04-1730">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1730">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="aae04-1731">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="aae04-1731">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="aae04-1732">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-1732">Container</span></span>

* <span data-ttu-id="aae04-1733">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1733">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="aae04-1734">EventHub</span><span class="sxs-lookup"><span data-stu-id="aae04-1734">EventHub</span></span>

* <span data-ttu-id="aae04-1735">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="aae04-1735">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="aae04-1736">Localizar</span><span class="sxs-lookup"><span data-stu-id="aae04-1736">Find</span></span>

* <span data-ttu-id="aae04-1737">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="aae04-1737">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1738">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1738">HDInsight</span></span>

* <span data-ttu-id="aae04-1739">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="aae04-1739">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1740">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1740">Network</span></span>

* <span data-ttu-id="aae04-1741">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="aae04-1741">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-1742">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aae04-1742">Rdbms</span></span>

* <span data-ttu-id="aae04-1743">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="aae04-1743">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1744">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1744">Role</span></span>

* <span data-ttu-id="aae04-1745">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="aae04-1745">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="aae04-1746">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="aae04-1746">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aae04-1747">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-1747">Service Fabric</span></span>

* <span data-ttu-id="aae04-1748">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="aae04-1748">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="aae04-1749">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1749">February 26, 2019</span></span>

<span data-ttu-id="aae04-1750">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="aae04-1750">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1751">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1751">Core</span></span>

* <span data-ttu-id="aae04-1752">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="aae04-1752">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1753">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1753">ACR</span></span>

* <span data-ttu-id="aae04-1754">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1754">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="aae04-1755">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-1755">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1756">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1756">ACS</span></span>

* <span data-ttu-id="aae04-1757">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="aae04-1757">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1758">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1758">AppService</span></span>

* <span data-ttu-id="aae04-1759">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="aae04-1759">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-1760">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-1760">Batch</span></span>
* <span data-ttu-id="aae04-1761">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1761">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="aae04-1762">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="aae04-1762">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="aae04-1763">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1763">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="aae04-1764">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="aae04-1764">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="aae04-1765">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="aae04-1765">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="aae04-1766">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-1766">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1767">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1767">CosmosDB</span></span>

* <span data-ttu-id="aae04-1768">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-1768">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="aae04-1769">Kusto</span><span class="sxs-lookup"><span data-stu-id="aae04-1769">Kusto</span></span>

* <span data-ttu-id="aae04-1770">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="aae04-1770">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1771">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1771">Network</span></span>

* <span data-ttu-id="aae04-1772">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1772">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="aae04-1773">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="aae04-1773">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="aae04-1774">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-1774">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="aae04-1775">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1775">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="aae04-1776">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1776">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="aae04-1777">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1777">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="aae04-1778">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="aae04-1778">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1779">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1779">Resource</span></span>

* <span data-ttu-id="aae04-1780">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-1780">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="aae04-1781">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1781">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="aae04-1782">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1782">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="aae04-1783">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1783">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="aae04-1784">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-1784">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1785">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1785">Role</span></span>

* <span data-ttu-id="aae04-1786">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1786">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1787">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1787">VM</span></span>

* <span data-ttu-id="aae04-1788">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="aae04-1788">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="aae04-1789">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1789">February 12, 2019</span></span>

<span data-ttu-id="aae04-1790">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="aae04-1790">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1791">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1791">Core</span></span>

* <span data-ttu-id="aae04-1792">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="aae04-1792">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="aae04-1793">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="aae04-1793">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1794">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1794">ACR</span></span>
* <span data-ttu-id="aae04-1795">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1795">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="aae04-1796">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="aae04-1796">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1797">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1797">ACS</span></span>
* <span data-ttu-id="aae04-1798">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-1798">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="aae04-1799">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="aae04-1799">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="aae04-1800">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-1800">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1801">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1801">AMS</span></span>
* <span data-ttu-id="aae04-1802">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-1802">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="aae04-1803">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-1803">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1804">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1804">Appservice</span></span>
* <span data-ttu-id="aae04-1805">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1805">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="aae04-1806">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="aae04-1806">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="aae04-1807">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1807">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="aae04-1808">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="aae04-1808">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="aae04-1809">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="aae04-1809">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1810">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1810">Botservice</span></span>
* <span data-ttu-id="aae04-1811">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="aae04-1811">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="aae04-1812">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="aae04-1812">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="aae04-1813">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1813">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="aae04-1814">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="aae04-1814">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="aae04-1815">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="aae04-1815">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="aae04-1816">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="aae04-1816">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="aae04-1817">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1817">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="aae04-1818">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="aae04-1818">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="aae04-1819">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="aae04-1819">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="aae04-1820">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="aae04-1820">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-1821">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-1821">Key Vault</span></span>
* <span data-ttu-id="aae04-1822">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="aae04-1822">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1823">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1823">Monitor</span></span>
* <span data-ttu-id="aae04-1824">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="aae04-1824">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1825">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1825">Network</span></span>
* <span data-ttu-id="aae04-1826">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="aae04-1826">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="aae04-1827">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-1827">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="aae04-1828">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-1828">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="aae04-1829">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1829">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="aae04-1830">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="aae04-1830">Policy Insights</span></span>
* <span data-ttu-id="aae04-1831">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-1831">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-1832">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1832">RDBMS</span></span>
* <span data-ttu-id="aae04-1833">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="aae04-1833">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-1834">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-1834">Redis</span></span>
* <span data-ttu-id="aae04-1835">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="aae04-1835">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="aae04-1836">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="aae04-1836">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="aae04-1837">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="aae04-1837">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="aae04-1838">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-1838">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="aae04-1839">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="aae04-1839">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="aae04-1840">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="aae04-1840">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="aae04-1841">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="aae04-1841">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1842">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1842">Role</span></span>
* <span data-ttu-id="aae04-1843">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="aae04-1843">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="aae04-1844">SQL VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1844">SQL VM</span></span>
* <span data-ttu-id="aae04-1845">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="aae04-1845">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1846">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1846">VM</span></span>
* <span data-ttu-id="aae04-1847">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="aae04-1847">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="aae04-1848">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1848">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="aae04-1849">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="aae04-1849">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="aae04-1850">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="aae04-1850">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="aae04-1851">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1851">January 31, 2019</span></span>

<span data-ttu-id="aae04-1852">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="aae04-1852">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="aae04-1853">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-1853">Core</span></span>

* <span data-ttu-id="aae04-1854">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="aae04-1854">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="aae04-1855">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1855">January 28, 2019</span></span>

<span data-ttu-id="aae04-1856">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="aae04-1856">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1857">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1857">ACR</span></span>
* <span data-ttu-id="aae04-1858">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="aae04-1858">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1859">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1859">ACS</span></span>
* <span data-ttu-id="aae04-1860">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="aae04-1860">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="aae04-1861">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-1861">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="aae04-1862">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="aae04-1862">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-1863">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-1863">AMS</span></span>
* <span data-ttu-id="aae04-1864">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="aae04-1864">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="aae04-1865">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="aae04-1865">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1866">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1866">Appservice</span></span>
* <span data-ttu-id="aae04-1867">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1867">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="aae04-1868">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="aae04-1868">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="aae04-1869">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="aae04-1869">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="aae04-1870">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-1870">Container</span></span>
* <span data-ttu-id="aae04-1871">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="aae04-1871">Added `container start` command</span></span>
* <span data-ttu-id="aae04-1872">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-1872">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aae04-1873">EventGrid</span><span class="sxs-lookup"><span data-stu-id="aae04-1873">EventGrid</span></span>
* <span data-ttu-id="aae04-1874">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1874">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="aae04-1875">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="aae04-1875">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="aae04-1876">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-1876">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="aae04-1877">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="aae04-1877">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="aae04-1878">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-1878">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1879">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1879">HDInsight</span></span>
* <span data-ttu-id="aae04-1880">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="aae04-1880">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="aae04-1881">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="aae04-1881">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="aae04-1882">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1882">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="aae04-1883">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1883">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="aae04-1884">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="aae04-1884">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="aae04-1885">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="aae04-1885">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-1886">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-1886">IoT</span></span>
* <span data-ttu-id="aae04-1887">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="aae04-1887">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="aae04-1888">Kusto</span><span class="sxs-lookup"><span data-stu-id="aae04-1888">Kusto</span></span>
* <span data-ttu-id="aae04-1889">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-1889">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-1890">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-1890">Monitor</span></span>
* <span data-ttu-id="aae04-1891">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-1891">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-1892">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-1892">Profile</span></span>
* <span data-ttu-id="aae04-1893">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="aae04-1893">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1894">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1894">Network</span></span>
* <span data-ttu-id="aae04-1895">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="aae04-1895">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="aae04-1896">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="aae04-1896">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-1897">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-1897">Resource</span></span>
* <span data-ttu-id="aae04-1898">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1898">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="aae04-1899">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1899">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="aae04-1900">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1900">SQL Virtual Machine</span></span>
* <span data-ttu-id="aae04-1901">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-1901">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1902">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1902">Storage</span></span>
* <span data-ttu-id="aae04-1903">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="aae04-1903">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="aae04-1904">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="aae04-1904">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1905">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1905">VM</span></span>
* <span data-ttu-id="aae04-1906">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="aae04-1906">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="aae04-1907">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="aae04-1907">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="aae04-1908">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="aae04-1908">January 15, 2019</span></span>

<span data-ttu-id="aae04-1909">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="aae04-1909">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-1910">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1910">ACR</span></span>
* <span data-ttu-id="aae04-1911">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="aae04-1911">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="aae04-1912">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-1912">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="aae04-1913">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="aae04-1913">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="aae04-1914">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1914">ACS</span></span>
* <span data-ttu-id="aae04-1915">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="aae04-1915">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1916">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1916">Appservice</span></span>
* <span data-ttu-id="aae04-1917">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="aae04-1917">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="aae04-1918">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-1918">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="aae04-1919">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="aae04-1919">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="aae04-1920">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="aae04-1920">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1921">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1921">Botservice</span></span>
* <span data-ttu-id="aae04-1922">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1922">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="aae04-1923">Configurar</span><span class="sxs-lookup"><span data-stu-id="aae04-1923">Configure</span></span>
* <span data-ttu-id="aae04-1924">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="aae04-1924">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1925">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1925">CosmosDB</span></span>
* <span data-ttu-id="aae04-1926">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="aae04-1926">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-1927">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-1927">HDInsight</span></span>
* <span data-ttu-id="aae04-1928">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="aae04-1928">Added commands for managing applications</span></span>
* <span data-ttu-id="aae04-1929">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="aae04-1929">Added commands for managing script actions</span></span>
* <span data-ttu-id="aae04-1930">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="aae04-1930">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="aae04-1931">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="aae04-1931">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="aae04-1932">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="aae04-1932">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1933">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1933">Network</span></span>
* <span data-ttu-id="aae04-1934">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1934">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="aae04-1935">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="aae04-1935">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="aae04-1936">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1936">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="aae04-1937">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="aae04-1937">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1938">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1938">Role</span></span>
* <span data-ttu-id="aae04-1939">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="aae04-1939">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="aae04-1940">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-1940">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="aae04-1941">Segurança</span><span class="sxs-lookup"><span data-stu-id="aae04-1941">Security</span></span>
* <span data-ttu-id="aae04-1942">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-1942">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-1943">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-1943">Storage</span></span>
* <span data-ttu-id="aae04-1944">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="aae04-1944">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="aae04-1945">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="aae04-1945">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="aae04-1946">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="aae04-1946">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="aae04-1947">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="aae04-1947">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="aae04-1948">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="aae04-1948">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1949">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1949">VM</span></span>
* <span data-ttu-id="aae04-1950">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="aae04-1950">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="aae04-1951">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1951">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="aae04-1952">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="aae04-1952">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="aae04-1953">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="aae04-1953">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="aae04-1954">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-1954">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="aae04-1955">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="aae04-1955">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="aae04-1956">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-1956">December 20, 2018</span></span>

<span data-ttu-id="aae04-1957">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="aae04-1957">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="aae04-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1958">Appservice</span></span>
* <span data-ttu-id="aae04-1959">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="aae04-1959">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="aae04-1960">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="aae04-1960">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="aae04-1961">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-1961">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="aae04-1962">IoT Central</span><span class="sxs-lookup"><span data-stu-id="aae04-1962">IoTCentral</span></span>
* <span data-ttu-id="aae04-1963">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="aae04-1963">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="aae04-1964">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-1964">Role</span></span>
* <span data-ttu-id="aae04-1965">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-1965">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-1966">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-1966">SQL</span></span>
* <span data-ttu-id="aae04-1967">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="aae04-1967">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-1968">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-1968">VM</span></span>
* <span data-ttu-id="aae04-1969">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1969">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="aae04-1970">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-1970">December 18, 2018</span></span>

<span data-ttu-id="aae04-1971">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="aae04-1971">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="aae04-1972">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-1972">ACR</span></span>
* <span data-ttu-id="aae04-1973">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="aae04-1973">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="aae04-1974">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="aae04-1974">Condensed the table layout for task list</span></span>
* <span data-ttu-id="aae04-1975">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="aae04-1975">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-1976">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-1976">ACS</span></span>
* <span data-ttu-id="aae04-1977">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="aae04-1977">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="aae04-1978">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-1978">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="aae04-1979">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="aae04-1979">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="aae04-1980">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-1980">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="aae04-1981">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-1981">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="aae04-1982">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="aae04-1982">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-1983">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-1983">Appservice</span></span>
* <span data-ttu-id="aae04-1984">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="aae04-1984">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="aae04-1985">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="aae04-1985">Botservice</span></span>
* <span data-ttu-id="aae04-1986">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="aae04-1986">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="aae04-1987">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="aae04-1987">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="aae04-1988">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="aae04-1988">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="aae04-1989">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="aae04-1989">Reduced Kudu network calls</span></span>
* <span data-ttu-id="aae04-1990">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="aae04-1990">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-1991">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-1991">Consumption</span></span>
* <span data-ttu-id="aae04-1992">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="aae04-1992">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-1993">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-1993">CosmosDB</span></span>
* <span data-ttu-id="aae04-1994">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="aae04-1994">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="aae04-1995">Mapas</span><span class="sxs-lookup"><span data-stu-id="aae04-1995">Maps</span></span>
* <span data-ttu-id="aae04-1996">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-1996">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-1997">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-1997">Network</span></span>
* <span data-ttu-id="aae04-1998">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="aae04-1998">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="aae04-1999">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-1999">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2000">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2000">Resource</span></span>
* <span data-ttu-id="aae04-2001">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2001">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="aae04-2002">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-2002">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2003">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2003">Storage</span></span>
*  <span data-ttu-id="aae04-2004">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2004">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2005">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2005">VM</span></span>
* <span data-ttu-id="aae04-2006">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="aae04-2006">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="aae04-2007">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2007">December 4, 2018</span></span>

<span data-ttu-id="aae04-2008">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="aae04-2008">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="aae04-2009">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2009">Core</span></span>
* <span data-ttu-id="aae04-2010">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="aae04-2010">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="aae04-2011">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2011">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2012">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2012">Appservice</span></span>
* <span data-ttu-id="aae04-2013">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2013">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="aae04-2014">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="aae04-2014">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2015">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2015">Network</span></span>
* <span data-ttu-id="aae04-2016">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="aae04-2016">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2017">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2017">Role</span></span>
* <span data-ttu-id="aae04-2018">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="aae04-2018">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="aae04-2019">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2019">VM</span></span>
* <span data-ttu-id="aae04-2020">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-2020">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="aae04-2021">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="aae04-2021">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="aae04-2022">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="aae04-2022">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="aae04-2023">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-2023">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="aae04-2024">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2024">November 20, 2018</span></span>

<span data-ttu-id="aae04-2025">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="aae04-2025">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="aae04-2026">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2026">Core</span></span>
* <span data-ttu-id="aae04-2027">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="aae04-2027">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2028">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2028">ACR</span></span>
* <span data-ttu-id="aae04-2029">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="aae04-2029">Added context token to task step</span></span>
* <span data-ttu-id="aae04-2030">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="aae04-2030">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="aae04-2031">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="aae04-2031">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2032">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2032">Appservice</span></span>
* <span data-ttu-id="aae04-2033">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="aae04-2033">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="aae04-2034">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="aae04-2034">Updated the default `node_version`.</span></span> <span data-ttu-id="aae04-2035">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="aae04-2035">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="aae04-2036">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2036">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="aae04-2037">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="aae04-2037">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="aae04-2038">Iot Central</span><span class="sxs-lookup"><span data-stu-id="aae04-2038">IotCentral</span></span>
* <span data-ttu-id="aae04-2039">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="aae04-2039">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-2040">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-2040">KeyVault</span></span>
* <span data-ttu-id="aae04-2041">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="aae04-2041">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2042">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2042">Network</span></span>
* <span data-ttu-id="aae04-2043">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="aae04-2043">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="aae04-2044">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="aae04-2044">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="aae04-2045">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2045">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="aae04-2046">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-2046">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2047">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aae04-2047">Rdbms</span></span>
* <span data-ttu-id="aae04-2048">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-2048">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="aae04-2049">Rbac</span><span class="sxs-lookup"><span data-stu-id="aae04-2049">Rbac</span></span>
* <span data-ttu-id="aae04-2050">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2050">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="aae04-2051">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2051">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="aae04-2052">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2052">Storage</span></span>
* <span data-ttu-id="aae04-2053">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2053">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="aae04-2054">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="aae04-2054">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="aae04-2055">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="aae04-2055">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="aae04-2056">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2056">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2057">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2057">VM</span></span>
* <span data-ttu-id="aae04-2058">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2058">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="aae04-2059">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="aae04-2059">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="aae04-2060">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="aae04-2060">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="aae04-2061">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="aae04-2061">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="aae04-2062">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2062">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="aae04-2063">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-2063">Added `snapshot wait` command</span></span>
* <span data-ttu-id="aae04-2064">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-2064">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="aae04-2065">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2065">November 6, 2018</span></span>

<span data-ttu-id="aae04-2066">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="aae04-2066">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2067">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2067">Core</span></span>
* <span data-ttu-id="aae04-2068">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="aae04-2068">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2069">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2069">ACR</span></span>
* <span data-ttu-id="aae04-2070">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="aae04-2070">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="aae04-2071">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="aae04-2071">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2072">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2072">ACS</span></span>
* <span data-ttu-id="aae04-2073">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2073">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="aae04-2074">Supervisor</span><span class="sxs-lookup"><span data-stu-id="aae04-2074">Advisor</span></span>
* <span data-ttu-id="aae04-2075">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="aae04-2075">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-2076">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2076">AMS</span></span>
* <span data-ttu-id="aae04-2077">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="aae04-2077">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="aae04-2078">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="aae04-2078">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="aae04-2079">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2079">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="aae04-2080">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="aae04-2080">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="aae04-2081">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="aae04-2081">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="aae04-2082">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="aae04-2082">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="aae04-2083">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="aae04-2083">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="aae04-2084">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="aae04-2084">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="aae04-2085">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="aae04-2085">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="aae04-2086">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="aae04-2086">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="aae04-2087">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-2087">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="aae04-2088">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2088">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="aae04-2089">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="aae04-2089">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="aae04-2090">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="aae04-2090">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="aae04-2091">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2091">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="aae04-2092">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="aae04-2092">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="aae04-2093">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="aae04-2093">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2094">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2094">AppService</span></span>
* <span data-ttu-id="aae04-2095">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="aae04-2095">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="aae04-2096">Configurar</span><span class="sxs-lookup"><span data-stu-id="aae04-2096">Configure</span></span>
* <span data-ttu-id="aae04-2097">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="aae04-2097">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2098">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2098">Container</span></span>
* <span data-ttu-id="aae04-2099">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="aae04-2099">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="aae04-2100">EventHub</span><span class="sxs-lookup"><span data-stu-id="aae04-2100">EventHub</span></span>
* <span data-ttu-id="aae04-2101">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2101">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2102">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2102">Interactive</span></span>
* <span data-ttu-id="aae04-2103">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="aae04-2103">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-2104">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-2104">Monitor</span></span>
* <span data-ttu-id="aae04-2105">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2105">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2106">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2106">Network</span></span>
* <span data-ttu-id="aae04-2107">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="aae04-2107">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="aae04-2108">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="aae04-2108">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="aae04-2109">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2109">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="aae04-2110">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-2110">Profile</span></span>
* <span data-ttu-id="aae04-2111">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="aae04-2111">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2112">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2112">RDBMS</span></span>
* <span data-ttu-id="aae04-2113">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="aae04-2113">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2114">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2114">Resource</span></span>
* <span data-ttu-id="aae04-2115">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="aae04-2115">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2116">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2116">Role</span></span>
* <span data-ttu-id="aae04-2117">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="aae04-2117">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="aae04-2118">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2118">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="aae04-2119">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="aae04-2119">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2120">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2120">Storage</span></span>
* <span data-ttu-id="aae04-2121">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="aae04-2121">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2122">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2122">VM</span></span>
* <span data-ttu-id="aae04-2123">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-2123">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="aae04-2124">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-2124">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="aae04-2125">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="aae04-2125">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="aae04-2126">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="aae04-2126">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="aae04-2127">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="aae04-2127">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="aae04-2128">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="aae04-2128">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="aae04-2129">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2129">October 23, 2018</span></span>

<span data-ttu-id="aae04-2130">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="aae04-2130">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2131">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2131">Core</span></span>
* <span data-ttu-id="aae04-2132">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="aae04-2132">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="aae04-2133">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="aae04-2133">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2134">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2134">ACR</span></span>
* <span data-ttu-id="aae04-2135">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="aae04-2135">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-2136">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-2136">CDN</span></span>
* <span data-ttu-id="aae04-2137">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="aae04-2137">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="aae04-2138">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2138">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2139">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2139">Container</span></span>
* <span data-ttu-id="aae04-2140">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="aae04-2140">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="aae04-2141">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-2141">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="aae04-2142">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-2142">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="aae04-2143">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-2143">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="aae04-2144">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="aae04-2144">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="aae04-2145">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="aae04-2145">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="aae04-2146">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2146">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-2147">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-2147">CosmosDB</span></span>
* <span data-ttu-id="aae04-2148">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2148">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2149">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2149">Interactive</span></span>
* <span data-ttu-id="aae04-2150">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="aae04-2150">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="aae04-2151">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2151">IoT Central</span></span>
* <span data-ttu-id="aae04-2152">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="aae04-2152">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="aae04-2153">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="aae04-2153">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-2154">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-2154">Monitor</span></span>
* <span data-ttu-id="aae04-2155">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="aae04-2155">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="aae04-2156">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2156">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="aae04-2157">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="aae04-2157">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="aae04-2158">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-2158">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="aae04-2159">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="aae04-2159">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="aae04-2160">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2160">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="aae04-2161">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="aae04-2161">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="aae04-2162">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="aae04-2162">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="aae04-2163">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-2163">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="aae04-2164">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2164">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2165">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2165">Network</span></span>
* <span data-ttu-id="aae04-2166">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="aae04-2166">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="aae04-2167">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="aae04-2167">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="aae04-2168">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="aae04-2168">ServiceBus</span></span>
* <span data-ttu-id="aae04-2169">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2169">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2170">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2170">SQL</span></span>
* <span data-ttu-id="aae04-2171">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="aae04-2171">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2172">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2172">Storage</span></span>
* <span data-ttu-id="aae04-2173">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="aae04-2173">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="aae04-2174">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="aae04-2174">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2175">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2175">VM</span></span>
* <span data-ttu-id="aae04-2176">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2176">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="aae04-2177">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2177">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="aae04-2178">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2178">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="aae04-2179">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2179">October 16, 2018</span></span>

<span data-ttu-id="aae04-2180">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="aae04-2180">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2181">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2181">VM</span></span>
* <span data-ttu-id="aae04-2182">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="aae04-2182">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="aae04-2183">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2183">October 9, 2018</span></span>

<span data-ttu-id="aae04-2184">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="aae04-2184">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2185">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2185">Core</span></span>
* <span data-ttu-id="aae04-2186">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="aae04-2186">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2187">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2187">ACR</span></span>
* <span data-ttu-id="aae04-2188">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="aae04-2188">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2189">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2189">ACS</span></span>
* <span data-ttu-id="aae04-2190">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="aae04-2190">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="aae04-2191">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="aae04-2191">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="aae04-2192">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="aae04-2192">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="aae04-2193">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2193">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2194">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2194">Container</span></span>
* <span data-ttu-id="aae04-2195">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="aae04-2195">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="aae04-2196">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-2196">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="aae04-2197">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="aae04-2197">Event Hub</span></span>
* <span data-ttu-id="aae04-2198">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2198">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="aae04-2199">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="aae04-2199">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="aae04-2200">Extensões</span><span class="sxs-lookup"><span data-stu-id="aae04-2200">Extensions</span></span>
* <span data-ttu-id="aae04-2201">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="aae04-2201">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="aae04-2202">HDInsight</span><span class="sxs-lookup"><span data-stu-id="aae04-2202">HDInsight</span></span>
* <span data-ttu-id="aae04-2203">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2203">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-2204">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2204">IoT</span></span>
* <span data-ttu-id="aae04-2205">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2205">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-2206">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-2206">KeyVault</span></span>
* <span data-ttu-id="aae04-2207">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="aae04-2207">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2208">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2208">Network</span></span>
* <span data-ttu-id="aae04-2209">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="aae04-2209">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="aae04-2210">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="aae04-2210">See #6052</span></span>
* <span data-ttu-id="aae04-2211">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2211">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="aae04-2212">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="aae04-2212">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="aae04-2213">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="aae04-2213">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="aae04-2214">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="aae04-2214">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="aae04-2215">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="aae04-2215">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="aae04-2216">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2216">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2217">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2217">Role</span></span>
* <span data-ttu-id="aae04-2218">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="aae04-2218">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="aae04-2219">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="aae04-2219">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="aae04-2220">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="aae04-2220">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="aae04-2221">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="aae04-2221">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="aae04-2222">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2222">Service Bus</span></span>
* <span data-ttu-id="aae04-2223">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="aae04-2223">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2224">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2224">VM</span></span>
* <span data-ttu-id="aae04-2225">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="aae04-2225">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="aae04-2226">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2226">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="aae04-2227">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="aae04-2227">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="aae04-2228">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="aae04-2228">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="aae04-2229">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="aae04-2229">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="aae04-2230">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="aae04-2230">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="aae04-2231">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2231">September 21, 2018</span></span>

<span data-ttu-id="aae04-2232">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="aae04-2232">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2233">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2233">ACR</span></span>
* <span data-ttu-id="aae04-2234">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2234">Added ACR Task commands</span></span>
* <span data-ttu-id="aae04-2235">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="aae04-2235">Added quick run command</span></span>
* <span data-ttu-id="aae04-2236">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2236">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="aae04-2237">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2237">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="aae04-2238">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="aae04-2238">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="aae04-2239">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="aae04-2239">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2240">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2240">ACS</span></span>
* <span data-ttu-id="aae04-2241">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-2241">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="aae04-2242">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="aae04-2242">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2243">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2243">AppService</span></span>

* <span data-ttu-id="aae04-2244">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="aae04-2244">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="aae04-2245">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="aae04-2245">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="aae04-2246">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="aae04-2246">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="aae04-2247">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="aae04-2247">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-2248">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2248">Batch</span></span>
* <span data-ttu-id="aae04-2249">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="aae04-2249">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="aae04-2250">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="aae04-2250">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="aae04-2251">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2251">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="aae04-2252">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="aae04-2252">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aae04-2253">Lote AI</span><span class="sxs-lookup"><span data-stu-id="aae04-2253">Batch AI</span></span> 
* <span data-ttu-id="aae04-2254">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2254">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aae04-2255">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2255">Cognitive Services</span></span>
* <span data-ttu-id="aae04-2256">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="aae04-2256">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="aae04-2257">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="aae04-2257">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="aae04-2258">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="aae04-2258">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="aae04-2259">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2259">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="aae04-2260">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2260">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="aae04-2261">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="aae04-2261">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2262">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2262">Container</span></span>
* <span data-ttu-id="aae04-2263">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="aae04-2263">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="aae04-2264">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2264">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="aae04-2265">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="aae04-2265">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="aae04-2266">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-2266">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="aae04-2267">DataLake</span><span class="sxs-lookup"><span data-stu-id="aae04-2267">Datalake</span></span>
* <span data-ttu-id="aae04-2268">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="aae04-2268">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="aae04-2269">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2269">Interactive Shell</span></span>
* <span data-ttu-id="aae04-2270">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2270">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="aae04-2271">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2271">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-2272">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2272">IoT</span></span>
* <span data-ttu-id="aae04-2273">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2273">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-2274">Key Vault</span><span class="sxs-lookup"><span data-stu-id="aae04-2274">Key Vault</span></span>
* <span data-ttu-id="aae04-2275">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="aae04-2275">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2276">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2276">Network</span></span>
* <span data-ttu-id="aae04-2277">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="aae04-2277">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="aae04-2278">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2278">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="aae04-2279">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="aae04-2279">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="aae04-2280">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="aae04-2280">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="aae04-2281">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2281">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="aae04-2282">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2282">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="aae04-2283">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="aae04-2283">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="aae04-2284">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="aae04-2284">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="aae04-2285">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="aae04-2285">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="aae04-2286">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="aae04-2286">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="aae04-2287">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="aae04-2287">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="aae04-2288">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="aae04-2288">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="aae04-2289">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="aae04-2289">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="aae04-2290">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="aae04-2290">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="aae04-2291">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="aae04-2291">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="aae04-2292">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="aae04-2292">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="aae04-2293">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2293">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="aae04-2294">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="aae04-2294">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2295">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2295">RDBMS</span></span>
* <span data-ttu-id="aae04-2296">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="aae04-2296">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="aae04-2297">Reserva</span><span class="sxs-lookup"><span data-stu-id="aae04-2297">Reservation</span></span>
* <span data-ttu-id="aae04-2298">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="aae04-2298">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="aae04-2299">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="aae04-2299">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="aae04-2300">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2300">Manage App</span></span>
* <span data-ttu-id="aae04-2301">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="aae04-2301">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="aae04-2302">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="aae04-2302">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2303">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2303">Role</span></span>
* <span data-ttu-id="aae04-2304">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="aae04-2304">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="aae04-2305">SignalR</span><span class="sxs-lookup"><span data-stu-id="aae04-2305">SignalR</span></span>
* <span data-ttu-id="aae04-2306">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="aae04-2306">First release</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2307">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2307">Storage</span></span>
* <span data-ttu-id="aae04-2308">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="aae04-2308">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="aae04-2309">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="aae04-2309">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2310">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2310">VM</span></span>
* <span data-ttu-id="aae04-2311">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="aae04-2311">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="aae04-2312">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="aae04-2312">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="aae04-2313">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2313">August 28, 2018</span></span>

<span data-ttu-id="aae04-2314">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="aae04-2314">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2315">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2315">Core</span></span>

* <span data-ttu-id="aae04-2316">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="aae04-2316">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="aae04-2317">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="aae04-2317">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2318">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2318">ACR</span></span>

* <span data-ttu-id="aae04-2319">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-2319">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="aae04-2320">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="aae04-2320">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2321">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2321">ACS</span></span>

* <span data-ttu-id="aae04-2322">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="aae04-2322">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="aae04-2323">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-2323">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2324">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2324">AppService</span></span>

* <span data-ttu-id="aae04-2325">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="aae04-2325">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="aae04-2326">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2326">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="aae04-2327">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2327">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-2328">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-2328">Backup</span></span>

* <span data-ttu-id="aae04-2329">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2329">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="aae04-2330">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="aae04-2330">Bot Service</span></span>

* <span data-ttu-id="aae04-2331">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2331">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aae04-2332">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2332">Cognitive Services</span></span>

* <span data-ttu-id="aae04-2333">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="aae04-2333">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-2334">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2334">IoT</span></span>

* <span data-ttu-id="aae04-2335">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="aae04-2335">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-2336">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-2336">Monitor</span></span>

* <span data-ttu-id="aae04-2337">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="aae04-2337">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="aae04-2338">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2338">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2339">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2339">Network</span></span>

* <span data-ttu-id="aae04-2340">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2340">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2341">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2341">Resource</span></span>

* <span data-ttu-id="aae04-2342">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2342">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2343">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2343">Storage</span></span>

* <span data-ttu-id="aae04-2344">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2344">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2345">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2345">VM</span></span>

* <span data-ttu-id="aae04-2346">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2346">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="aae04-2347">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2347">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="aae04-2348">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2348">Auguest 14, 2018</span></span>

<span data-ttu-id="aae04-2349">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="aae04-2349">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2350">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2350">Core</span></span>

* <span data-ttu-id="aae04-2351">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="aae04-2351">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="aae04-2352">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="aae04-2352">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="aae04-2353">Telemetria</span><span class="sxs-lookup"><span data-stu-id="aae04-2353">Telemetry</span></span>

* <span data-ttu-id="aae04-2354">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="aae04-2354">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2355">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2355">ACR</span></span>

* <span data-ttu-id="aae04-2356">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-2356">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="aae04-2357">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2357">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2358">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2358">ACS</span></span>

* <span data-ttu-id="aae04-2359">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-2359">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="aae04-2360">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2360">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="aae04-2361">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="aae04-2361">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="aae04-2362">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="aae04-2362">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="aae04-2363">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="aae04-2363">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="aae04-2364">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2364">AppService</span></span>

* <span data-ttu-id="aae04-2365">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="aae04-2365">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="aae04-2366">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="aae04-2366">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-2367">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aae04-2367">BatchAI</span></span>

* <span data-ttu-id="aae04-2368">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="aae04-2368">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="aae04-2369">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2369">Container</span></span>

* <span data-ttu-id="aae04-2370">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2370">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="aae04-2371">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2371">IoT</span></span>

* <span data-ttu-id="aae04-2372">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="aae04-2372">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="aae04-2373">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="aae04-2373">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="aae04-2374">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-2374">Iot Central</span></span>

* <span data-ttu-id="aae04-2375">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="aae04-2375">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-2376">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-2376">KeyVault</span></span>


* <span data-ttu-id="aae04-2377">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="aae04-2377">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="aae04-2378">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2378">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="aae04-2379">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="aae04-2379">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="aae04-2380">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="aae04-2380">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="aae04-2381">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="aae04-2381">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="aae04-2382">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="aae04-2382">Relay</span></span>

* <span data-ttu-id="aae04-2383">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2383">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2384">Sql</span><span class="sxs-lookup"><span data-stu-id="aae04-2384">Sql</span></span>

* <span data-ttu-id="aae04-2385">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="aae04-2385">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2386">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2386">Storage</span></span>

* <span data-ttu-id="aae04-2387">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="aae04-2387">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="aae04-2388">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="aae04-2388">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="aae04-2389">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="aae04-2389">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="aae04-2390">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="aae04-2390">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="aae04-2391">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2391">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2392">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2392">VM</span></span>

* <span data-ttu-id="aae04-2393">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="aae04-2393">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="aae04-2394">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2394">July 31, 2018</span></span>

<span data-ttu-id="aae04-2395">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="aae04-2395">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2396">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2396">ACR</span></span>

* <span data-ttu-id="aae04-2397">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2397">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="aae04-2398">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="aae04-2398">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2399">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2399">ACS</span></span>

* <span data-ttu-id="aae04-2400">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="aae04-2400">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-2401">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2401">Batch</span></span>

* <span data-ttu-id="aae04-2402">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="aae04-2402">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2403">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2403">Container</span></span>

* <span data-ttu-id="aae04-2404">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2404">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2405">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2405">Network</span></span>

* <span data-ttu-id="aae04-2406">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="aae04-2406">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="aae04-2407">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2407">Resource</span></span>

* <span data-ttu-id="aae04-2408">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="aae04-2408">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="aae04-2409">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="aae04-2409">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2410">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2410">Role</span></span>

* <span data-ttu-id="aae04-2411">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="aae04-2411">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="aae04-2412">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-2412">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="aae04-2413">Search</span><span class="sxs-lookup"><span data-stu-id="aae04-2413">Search</span></span>

* <span data-ttu-id="aae04-2414">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="aae04-2414">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="aae04-2415">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2415">Service Bus</span></span>

* <span data-ttu-id="aae04-2416">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="aae04-2416">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="aae04-2417">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2417">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="aae04-2418">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="aae04-2418">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="aae04-2419">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="aae04-2419">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2420">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2420">Storage</span></span>

* <span data-ttu-id="aae04-2421">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="aae04-2421">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="aae04-2422">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2422">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2423">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2423">VM</span></span>

* <span data-ttu-id="aae04-2424">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2424">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="aae04-2425">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="aae04-2425">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="aae04-2426">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2426">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="aae04-2427">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="aae04-2427">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="aae04-2428">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2428">July 18, 2018</span></span>

<span data-ttu-id="aae04-2429">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="aae04-2429">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2430">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2430">Core</span></span>

* <span data-ttu-id="aae04-2431">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="aae04-2431">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="aae04-2432">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="aae04-2432">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="aae04-2433">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="aae04-2433">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2434">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2434">ACR</span></span>

* <span data-ttu-id="aae04-2435">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="aae04-2435">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="aae04-2436">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="aae04-2436">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="aae04-2437">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2437">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="aae04-2438">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-2438">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2439">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2439">ACS</span></span>

* <span data-ttu-id="aae04-2440">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="aae04-2440">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2441">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2441">AppService</span></span>

* <span data-ttu-id="aae04-2442">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="aae04-2442">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-2443">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2443">Batch</span></span>

* <span data-ttu-id="aae04-2444">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aae04-2444">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="aae04-2445">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-2445">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aae04-2446">Lote AI</span><span class="sxs-lookup"><span data-stu-id="aae04-2446">Batch AI</span></span>

* <span data-ttu-id="aae04-2447">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="aae04-2447">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2448">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2448">Container</span></span>

* <span data-ttu-id="aae04-2449">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="aae04-2449">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="aae04-2450">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="aae04-2450">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2451">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2451">Network</span></span>

* <span data-ttu-id="aae04-2452">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2452">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="aae04-2453">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-2453">Added `network nic wait`</span></span>
* <span data-ttu-id="aae04-2454">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2454">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="aae04-2455">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2455">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="aae04-2456">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2456">Resource</span></span>

* <span data-ttu-id="aae04-2457">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-2457">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="aae04-2458">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-2458">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="aae04-2459">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-2459">Added `deployment wait` command</span></span>
* <span data-ttu-id="aae04-2460">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="aae04-2460">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2461">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2461">SQL</span></span>

* <span data-ttu-id="aae04-2462">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2462">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="aae04-2463">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="aae04-2463">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="aae04-2464">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="aae04-2464">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2465">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2465">Storage</span></span>

* <span data-ttu-id="aae04-2466">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="aae04-2466">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2467">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2467">VM</span></span>

* <span data-ttu-id="aae04-2468">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2468">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="aae04-2469">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2469">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="aae04-2470">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="aae04-2470">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="aae04-2471">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2471">July 3, 2018</span></span>

<span data-ttu-id="aae04-2472">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="aae04-2472">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-2473">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-2473">AKS</span></span>

* <span data-ttu-id="aae04-2474">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2474">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="aae04-2475">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2475">July 3, 2018</span></span>

<span data-ttu-id="aae04-2476">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="aae04-2476">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2477">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2477">Core</span></span>

* <span data-ttu-id="aae04-2478">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2478">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2479">ACR</span></span>

* <span data-ttu-id="aae04-2480">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-2480">Added polling build status</span></span>
* <span data-ttu-id="aae04-2481">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-2481">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="aae04-2482">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="aae04-2482">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2483">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2483">ACS</span></span>

* <span data-ttu-id="aae04-2484">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2484">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="aae04-2485">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="aae04-2485">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="aae04-2486">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2486">Updated options for `aks browse` command.</span></span> <span data-ttu-id="aae04-2487">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-2487">Added `--listen-port` support</span></span>
* <span data-ttu-id="aae04-2488">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2488">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="aae04-2489">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="aae04-2489">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="aae04-2490">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="aae04-2490">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2491">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2491">AppService</span></span>

* <span data-ttu-id="aae04-2492">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="aae04-2492">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="aae04-2493">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="aae04-2493">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-2494">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-2494">Backup</span></span>

* <span data-ttu-id="aae04-2495">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="aae04-2495">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-2496">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aae04-2496">BatchAI</span></span>

* <span data-ttu-id="aae04-2497">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2497">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="aae04-2498">Nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-2498">Cloud</span></span>

* <span data-ttu-id="aae04-2499">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-2499">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2500">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2500">Container</span></span>

* <span data-ttu-id="aae04-2501">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="aae04-2501">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="aae04-2502">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-2502">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="aae04-2503">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="aae04-2503">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2504">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2504">Extension</span></span>

* <span data-ttu-id="aae04-2505">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-2505">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2506">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2506">Network</span></span>

* <span data-ttu-id="aae04-2507">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="aae04-2507">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2508">Rdbms</span><span class="sxs-lookup"><span data-stu-id="aae04-2508">Rdbms</span></span>

* <span data-ttu-id="aae04-2509">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-2509">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2510">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2510">Resource</span></span>

* <span data-ttu-id="aae04-2511">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-2511">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2512">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2512">VM</span></span>

* <span data-ttu-id="aae04-2513">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="aae04-2513">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="aae04-2514">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2514">June 25, 2018</span></span>

<span data-ttu-id="aae04-2515">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="aae04-2515">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="aae04-2516">CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-2516">CLI</span></span>

* <span data-ttu-id="aae04-2517">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2517">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="aae04-2518">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2518">June 19, 2018</span></span>

<span data-ttu-id="aae04-2519">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="aae04-2519">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2520">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2520">Core</span></span>

* <span data-ttu-id="aae04-2521">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2521">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2522">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2522">ACR</span></span>

* <span data-ttu-id="aae04-2523">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="aae04-2523">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="aae04-2524">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="aae04-2524">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2525">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2525">ACS</span></span>

* <span data-ttu-id="aae04-2526">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="aae04-2526">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="aae04-2527">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="aae04-2527">Added `--update` support</span></span>
* <span data-ttu-id="aae04-2528">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="aae04-2528">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="aae04-2529">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-2529">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="aae04-2530">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-2530">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="aae04-2531">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="aae04-2531">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="aae04-2532">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="aae04-2532">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="aae04-2533">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="aae04-2533">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2534">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2534">AppService</span></span>

* <span data-ttu-id="aae04-2535">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="aae04-2535">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="aae04-2536">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="aae04-2536">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-2537">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2537">Batch</span></span>

* <span data-ttu-id="aae04-2538">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="aae04-2538">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aae04-2539">Lote AI</span><span class="sxs-lookup"><span data-stu-id="aae04-2539">Batch AI</span></span>

* <span data-ttu-id="aae04-2540">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="aae04-2540">Added support for workspaces.</span></span> <span data-ttu-id="aae04-2541">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="aae04-2541">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="aae04-2542">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="aae04-2542">Added support for experiments.</span></span> <span data-ttu-id="aae04-2543">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="aae04-2543">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="aae04-2544">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="aae04-2544">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="aae04-2545">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2545">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="aae04-2546">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="aae04-2546">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="aae04-2547">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="aae04-2547">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="aae04-2548">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="aae04-2548">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="aae04-2549">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="aae04-2549">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="aae04-2550">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2550">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="aae04-2551">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="aae04-2551">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="aae04-2552">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2552">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="aae04-2553">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="aae04-2553">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="aae04-2554">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="aae04-2554">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="aae04-2555">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="aae04-2555">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="aae04-2556">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2556">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="aae04-2557">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="aae04-2557">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="aae04-2558">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="aae04-2558">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="aae04-2559">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="aae04-2559">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="aae04-2560">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="aae04-2560">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="aae04-2561">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="aae04-2561">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="aae04-2562">Mapas</span><span class="sxs-lookup"><span data-stu-id="aae04-2562">Maps</span></span>

* <span data-ttu-id="aae04-2563">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="aae04-2563">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2564">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2564">Network</span></span>

* <span data-ttu-id="aae04-2565">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="aae04-2565">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="aae04-2566">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="aae04-2566">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="aae04-2567">#6502</span><span class="sxs-lookup"><span data-stu-id="aae04-2567">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="aae04-2568">Reservas</span><span class="sxs-lookup"><span data-stu-id="aae04-2568">Reservations</span></span>

* <span data-ttu-id="aae04-2569">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2569">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="aae04-2570">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2570">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="aae04-2571">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="aae04-2571">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="aae04-2572">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="aae04-2572">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="aae04-2573">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="aae04-2573">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="aae04-2574">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2574">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2575">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2575">Role</span></span>

* <span data-ttu-id="aae04-2576">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="aae04-2576">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2577">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2577">SQL</span></span>

* <span data-ttu-id="aae04-2578">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2578">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2579">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2579">Storage</span></span>

* <span data-ttu-id="aae04-2580">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="aae04-2580">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2581">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2581">VM</span></span>

* <span data-ttu-id="aae04-2582">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2582">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="aae04-2583">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="aae04-2583">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="aae04-2584">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="aae04-2584">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="aae04-2585">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2585">June 13, 2018</span></span>

<span data-ttu-id="aae04-2586">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="aae04-2586">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2587">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2587">Core</span></span>

* <span data-ttu-id="aae04-2588">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="aae04-2588">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="aae04-2589">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2589">June 13, 2018</span></span>

<span data-ttu-id="aae04-2590">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="aae04-2590">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-2591">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-2591">AKS</span></span>

* <span data-ttu-id="aae04-2592">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2592">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="aae04-2593">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="aae04-2593">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="aae04-2594">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2594">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="aae04-2595">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2595">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="aae04-2596">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2596">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2597">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2597">AppService</span></span>

* <span data-ttu-id="aae04-2598">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="aae04-2598">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="aae04-2599">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2599">June 5, 2018</span></span>

<span data-ttu-id="aae04-2600">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="aae04-2600">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2601">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2601">Interactive</span></span>

* <span data-ttu-id="aae04-2602">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2602">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="aae04-2603">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2603">June 5, 2018</span></span>

<span data-ttu-id="aae04-2604">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="aae04-2604">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2605">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2605">Core</span></span>

* <span data-ttu-id="aae04-2606">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="aae04-2606">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="aae04-2607">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="aae04-2607">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2608">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2608">ACR</span></span>

* <span data-ttu-id="aae04-2609">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="aae04-2609">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="aae04-2610">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="aae04-2610">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="aae04-2611">AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-2611">AKS</span></span>

* <span data-ttu-id="aae04-2612">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="aae04-2612">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-2613">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2613">Batch</span></span>

* <span data-ttu-id="aae04-2614">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="aae04-2614">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-2615">IOT</span><span class="sxs-lookup"><span data-stu-id="aae04-2615">IOT</span></span>

* <span data-ttu-id="aae04-2616">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="aae04-2616">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2617">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2617">Network</span></span>

* <span data-ttu-id="aae04-2618">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="aae04-2618">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="aae04-2619">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="aae04-2619">Policy Insights</span></span>

* <span data-ttu-id="aae04-2620">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2620">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="aae04-2621">ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-2621">ARM</span></span>

* <span data-ttu-id="aae04-2622">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="aae04-2622">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2623">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2623">SQL</span></span>

* <span data-ttu-id="aae04-2624">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="aae04-2624">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="aae04-2625">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="aae04-2625">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="aae04-2626">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2626">Storage</span></span>

* <span data-ttu-id="aae04-2627">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="aae04-2627">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2628">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2628">VM</span></span>

* <span data-ttu-id="aae04-2629">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="aae04-2629">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="aae04-2630">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2630">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="aae04-2631">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2631">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="aae04-2632">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2632">May 22, 2018</span></span>

<span data-ttu-id="aae04-2633">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="aae04-2633">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2634">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2634">Core</span></span>

* <span data-ttu-id="aae04-2635">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2635">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2636">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2636">ACS</span></span>

* <span data-ttu-id="aae04-2637">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-2637">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="aae04-2638">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-2638">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2639">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2639">AppService</span></span>

* <span data-ttu-id="aae04-2640">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="aae04-2640">Improved generic update commands</span></span>
* <span data-ttu-id="aae04-2641">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="aae04-2641">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2642">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2642">Container</span></span>

* <span data-ttu-id="aae04-2643">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="aae04-2643">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="aae04-2644">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2644">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2645">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2645">Extension</span></span>

* <span data-ttu-id="aae04-2646">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="aae04-2646">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2647">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2647">Interactive</span></span>

* <span data-ttu-id="aae04-2648">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="aae04-2648">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="aae04-2649">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="aae04-2649">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-2650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-2650">KeyVault</span></span>

* <span data-ttu-id="aae04-2651">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="aae04-2651">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2652">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2652">Network</span></span>

* <span data-ttu-id="aae04-2653">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="aae04-2653">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="aae04-2654">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="aae04-2654">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2655">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2655">SQL</span></span>

* <span data-ttu-id="aae04-2656">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="aae04-2656">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="aae04-2657">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="aae04-2657">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="aae04-2658">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="aae04-2658">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="aae04-2659">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aae04-2659">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="aae04-2660">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="aae04-2660">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="aae04-2661">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2661">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="aae04-2662">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="aae04-2662">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="aae04-2663">`edition`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2663">`edition`.</span></span> <span data-ttu-id="aae04-2664">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="aae04-2664">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="aae04-2665">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2665">`elasticPoolName`.</span></span> <span data-ttu-id="aae04-2666">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="aae04-2666">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="aae04-2667">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="aae04-2667">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="aae04-2668">`edition`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2668">`edition`.</span></span> <span data-ttu-id="aae04-2669">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="aae04-2669">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="aae04-2670">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2670">`dtu`.</span></span> <span data-ttu-id="aae04-2671">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="aae04-2671">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="aae04-2672">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2672">`databaseDtuMin`.</span></span> <span data-ttu-id="aae04-2673">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="aae04-2673">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="aae04-2674">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2674">`databaseDtuMax`.</span></span> <span data-ttu-id="aae04-2675">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="aae04-2675">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="aae04-2676">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2676">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="aae04-2677">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2677">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2678">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2678">Storage</span></span>

* <span data-ttu-id="aae04-2679">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-2679">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="aae04-2680">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-2680">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2681">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2681">VM</span></span>

* <span data-ttu-id="aae04-2682">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2682">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="aae04-2683">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="aae04-2683">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="aae04-2684">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="aae04-2684">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="aae04-2685">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="aae04-2685">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="aae04-2686">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2686">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="aae04-2687">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2687">May 7, 2018</span></span>

<span data-ttu-id="aae04-2688">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="aae04-2688">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2689">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2689">Core</span></span>

* <span data-ttu-id="aae04-2690">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="aae04-2690">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="aae04-2691">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="aae04-2691">Added limited support for positional arguments</span></span>
* <span data-ttu-id="aae04-2692">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2692">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="aae04-2693">#5591</span><span class="sxs-lookup"><span data-stu-id="aae04-2693">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="aae04-2694">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2694">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="aae04-2695">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="aae04-2695">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="aae04-2696">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2696">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="aae04-2697">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="aae04-2697">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="aae04-2698">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="aae04-2698">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2699">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2699">ACR</span></span>

* <span data-ttu-id="aae04-2700">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2700">Added ACR Build commands</span></span>
* <span data-ttu-id="aae04-2701">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="aae04-2701">Improved resource not found error messages</span></span>
* <span data-ttu-id="aae04-2702">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="aae04-2702">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="aae04-2703">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="aae04-2703">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="aae04-2704">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="aae04-2704">Improved repository commands error messages</span></span>
* <span data-ttu-id="aae04-2705">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2705">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2706">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2706">ACS</span></span>

* <span data-ttu-id="aae04-2707">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-2707">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="aae04-2708">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="aae04-2708">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="aae04-2709">AMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2709">AMS</span></span>

* <span data-ttu-id="aae04-2710">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-2710">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2711">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2711">Appservice</span></span>

* <span data-ttu-id="aae04-2712">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-2712">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="aae04-2713">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2713">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="aae04-2714">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="aae04-2714">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="aae04-2715">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="aae04-2715">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="aae04-2716">Lote AI</span><span class="sxs-lookup"><span data-stu-id="aae04-2716">Batch AI</span></span>

* <span data-ttu-id="aae04-2717">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-2717">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aae04-2718">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2718">Cognitive Services</span></span>

* <span data-ttu-id="aae04-2719">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="aae04-2719">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-2720">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-2720">Consumption</span></span>

* <span data-ttu-id="aae04-2721">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2721">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2722">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2722">Container</span></span>

* <span data-ttu-id="aae04-2723">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-2723">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="aae04-2724">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-2724">Cosmos DB</span></span>

* <span data-ttu-id="aae04-2725">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="aae04-2725">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="aae04-2726">DMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2726">DMS</span></span>

* <span data-ttu-id="aae04-2727">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-2727">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2728">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2728">Extension</span></span>

* <span data-ttu-id="aae04-2729">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="aae04-2729">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2730">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2730">Interactive</span></span>

* <span data-ttu-id="aae04-2731">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="aae04-2731">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="aae04-2732">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="aae04-2732">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="aae04-2733">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-2733">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="aae04-2734">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="aae04-2734">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="aae04-2735">Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-2735">Lab</span></span>

* <span data-ttu-id="aae04-2736">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="aae04-2736">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2737">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2737">Network</span></span>

* <span data-ttu-id="aae04-2738">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="aae04-2738">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="aae04-2739">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-2739">Profile</span></span>

* <span data-ttu-id="aae04-2740">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="aae04-2740">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="aae04-2741">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="aae04-2741">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="aae04-2742">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="aae04-2742">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-2743">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-2743">Redis</span></span>

* <span data-ttu-id="aae04-2744">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2744">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="aae04-2745">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="aae04-2745">Deprecated `redis list-all`.</span></span> <span data-ttu-id="aae04-2746">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2746">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="aae04-2747">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="aae04-2747">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="aae04-2748">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2748">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2749">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2749">Role</span></span>

* <span data-ttu-id="aae04-2750">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="aae04-2750">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2751">Storage</span></span>

* <span data-ttu-id="aae04-2752">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2752">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="aae04-2753">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="aae04-2753">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="aae04-2754">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="aae04-2754">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="aae04-2755">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="aae04-2755">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="aae04-2756">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="aae04-2756">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2757">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2757">VM</span></span>

* <span data-ttu-id="aae04-2758">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="aae04-2758">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="aae04-2759">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-2759">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="aae04-2760">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="aae04-2760">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="aae04-2761">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="aae04-2761">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="aae04-2762">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="aae04-2762">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="aae04-2763">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="aae04-2763">Added write accelerator support</span></span>
* <span data-ttu-id="aae04-2764">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="aae04-2764">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="aae04-2765">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="aae04-2765">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="aae04-2766">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="aae04-2766">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="aae04-2767">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2767">April 10, 2018</span></span>

<span data-ttu-id="aae04-2768">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="aae04-2768">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2769">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2769">ACR</span></span>

* <span data-ttu-id="aae04-2770">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="aae04-2770">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2771">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2771">ACS</span></span>

* <span data-ttu-id="aae04-2772">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="aae04-2772">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2773">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2773">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="aae04-2775">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="aae04-2775">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-2776">BatchAI</span><span class="sxs-lookup"><span data-stu-id="aae04-2776">BatchAI</span></span>

* <span data-ttu-id="aae04-2777">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="aae04-2777">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="aae04-2778">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-2778">Job level mounting</span></span>
  - <span data-ttu-id="aae04-2779">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="aae04-2779">Environment variables with secret values</span></span>
  - <span data-ttu-id="aae04-2780">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="aae04-2780">Performance counters settings</span></span>
  - <span data-ttu-id="aae04-2781">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-2781">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="aae04-2782">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="aae04-2782">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="aae04-2783">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="aae04-2783">Usage and limits reporting</span></span>
  - <span data-ttu-id="aae04-2784">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="aae04-2784">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="aae04-2785">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2785">Support for custom images</span></span>
  - <span data-ttu-id="aae04-2786">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="aae04-2786">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="aae04-2787">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-2787">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="aae04-2788">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="aae04-2788">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="aae04-2789">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="aae04-2789">National clouds are supported</span></span>
* <span data-ttu-id="aae04-2790">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="aae04-2790">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="aae04-2791">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="aae04-2791">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="aae04-2792">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-2792">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="aae04-2793">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="aae04-2793">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="aae04-2794">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="aae04-2794">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="aae04-2795">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="aae04-2795">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="aae04-2796">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2796">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="aae04-2797">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="aae04-2797">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="aae04-2798">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="aae04-2798">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="aae04-2799">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2799">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="aae04-2800">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="aae04-2800">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="aae04-2801">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="aae04-2801">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="aae04-2802">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2802">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="aae04-2803">Cobrança</span><span class="sxs-lookup"><span data-stu-id="aae04-2803">Billing</span></span>

* <span data-ttu-id="aae04-2804">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="aae04-2804">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-2805">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-2805">Consumption</span></span>

* <span data-ttu-id="aae04-2806">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="aae04-2806">Added `marketplace` commands</span></span>
* <span data-ttu-id="aae04-2807">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="aae04-2807">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="aae04-2808">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="aae04-2808">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="aae04-2809">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="aae04-2809">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="aae04-2810">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="aae04-2810">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="aae04-2811">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="aae04-2811">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2812">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2812">Container</span></span>

* <span data-ttu-id="aae04-2813">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="aae04-2813">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="aae04-2814">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="aae04-2814">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2815">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2815">Extension</span></span>

* <span data-ttu-id="aae04-2816">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="aae04-2816">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2817">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2817">Interactive</span></span>

* <span data-ttu-id="aae04-2818">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="aae04-2818">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="aae04-2819">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="aae04-2819">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="aae04-2820">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="aae04-2820">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2821">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2821">Network</span></span>

* <span data-ttu-id="aae04-2822">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="aae04-2822">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="aae04-2823">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2823">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="aae04-2824">#4910</span><span class="sxs-lookup"><span data-stu-id="aae04-2824">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="aae04-2825">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="aae04-2825">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="aae04-2826">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="aae04-2826">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="aae04-2827">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2827">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="aae04-2828">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2828">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="aae04-2829">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="aae04-2829">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-2830">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-2830">Profile</span></span>

* <span data-ttu-id="aae04-2831">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2831">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="aae04-2832">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="aae04-2832">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2833">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2833">RDBMS</span></span>

* <span data-ttu-id="aae04-2834">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="aae04-2834">Added `georestore` command</span></span>
* <span data-ttu-id="aae04-2835">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2835">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2836">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2836">Resource</span></span>

* <span data-ttu-id="aae04-2837">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2837">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="aae04-2838">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2838">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2839">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2839">SQL</span></span>

* <span data-ttu-id="aae04-2840">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="aae04-2840">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2841">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2841">Storage</span></span>

* <span data-ttu-id="aae04-2842">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2842">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2843">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2843">VM</span></span>

* <span data-ttu-id="aae04-2844">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2844">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="aae04-2845">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2845">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="aae04-2847">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2847">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="aae04-2848">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="aae04-2848">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="aae04-2849">#5718</span><span class="sxs-lookup"><span data-stu-id="aae04-2849">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="aae04-2850">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="aae04-2850">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="aae04-2851">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2851">March 27, 2018</span></span>

<span data-ttu-id="aae04-2852">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="aae04-2852">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2853">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2853">Core</span></span>

* <span data-ttu-id="aae04-2854">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="aae04-2854">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2855">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2855">ACS</span></span>

* <span data-ttu-id="aae04-2856">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aae04-2856">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2857">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2857">Appservice</span></span>

* <span data-ttu-id="aae04-2858">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2858">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="aae04-2859">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2859">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-2860">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-2860">Backup</span></span>

* <span data-ttu-id="aae04-2861">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2861">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="aae04-2862">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-2862">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="aae04-2863">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="aae04-2863">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="aae04-2864">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2864">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2865">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2865">Container</span></span>

* <span data-ttu-id="aae04-2866">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="aae04-2866">Added `container exec` command.</span></span> <span data-ttu-id="aae04-2867">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="aae04-2867">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="aae04-2868">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2868">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2869">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2869">Extension</span></span>

* <span data-ttu-id="aae04-2870">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-2870">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="aae04-2871">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="aae04-2871">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="aae04-2872">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2872">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2873">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2873">Interactive</span></span>

* <span data-ttu-id="aae04-2874">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2874">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="aae04-2875">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="aae04-2875">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="aae04-2876">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-2876">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="aae04-2877">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="aae04-2877">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="aae04-2878">Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-2878">Lab</span></span>

* <span data-ttu-id="aae04-2879">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="aae04-2879">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-2880">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-2880">Monitor</span></span>

* <span data-ttu-id="aae04-2881">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="aae04-2881">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="aae04-2882">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="aae04-2882">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="aae04-2883">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="aae04-2883">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2884">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2884">Network</span></span>

* <span data-ttu-id="aae04-2885">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="aae04-2885">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-2886">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-2886">Profile</span></span>

* <span data-ttu-id="aae04-2887">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="aae04-2887">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2888">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2888">RDBMS</span></span>

* <span data-ttu-id="aae04-2889">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="aae04-2889">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2890">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2890">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="aae04-2892">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2892">Role</span></span>

* <span data-ttu-id="aae04-2893">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2893">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="aae04-2894">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="aae04-2894">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="aae04-2895">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2895">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="aae04-2896">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2896">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="aae04-2897">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="aae04-2897">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2898">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2898">Storage</span></span>

* <span data-ttu-id="aae04-2899">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="aae04-2899">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="aae04-2900">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="aae04-2900">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2901">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2901">VM</span></span>

* <span data-ttu-id="aae04-2902">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="aae04-2902">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="aae04-2903">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2903">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="aae04-2904">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="aae04-2904">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="aae04-2905">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="aae04-2905">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="aae04-2906">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2906">March 13, 2018</span></span>

<span data-ttu-id="aae04-2907">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="aae04-2907">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-2908">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-2908">ACR</span></span>

* <span data-ttu-id="aae04-2909">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-2909">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="aae04-2910">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-2910">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="aae04-2911">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="aae04-2911">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2912">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2912">ACS</span></span>

* <span data-ttu-id="aae04-2913">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="aae04-2913">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="aae04-2914">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="aae04-2914">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="aae04-2915">Supervisor</span><span class="sxs-lookup"><span data-stu-id="aae04-2915">Advisor</span></span>

* <span data-ttu-id="aae04-2916">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2916">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="aae04-2917">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="aae04-2917">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="aae04-2918">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="aae04-2918">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="aae04-2919">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="aae04-2919">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="aae04-2920">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="aae04-2920">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2921">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2921">Appservice</span></span>

* <span data-ttu-id="aae04-2922">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="aae04-2922">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="aae04-2923">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-2923">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="aae04-2924">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-2924">Eventhubs</span></span>

* <span data-ttu-id="aae04-2925">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2925">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-2926">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-2926">Extension</span></span>

* <span data-ttu-id="aae04-2927">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="aae04-2927">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-2928">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-2928">Interactive</span></span>

* <span data-ttu-id="aae04-2929">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="aae04-2929">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="aae04-2930">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="aae04-2930">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="aae04-2931">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="aae04-2931">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="aae04-2932">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="aae04-2932">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-2933">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-2933">Monitor</span></span>

* <span data-ttu-id="aae04-2934">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2934">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="aae04-2935">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="aae04-2935">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="aae04-2936">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="aae04-2936">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="aae04-2937">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-2937">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2938">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2938">Network</span></span>

* <span data-ttu-id="aae04-2939">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2939">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="aae04-2940">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="aae04-2940">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="aae04-2941">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-2941">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="aae04-2942">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="aae04-2942">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-2943">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-2943">Profile</span></span>

* <span data-ttu-id="aae04-2944">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="aae04-2944">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="aae04-2945">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="aae04-2945">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-2946">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-2946">RDBMS</span></span>

* <span data-ttu-id="aae04-2947">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="aae04-2947">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="aae04-2948">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2948">Service Bus</span></span>

* <span data-ttu-id="aae04-2949">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-2949">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2950">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2950">Storage</span></span>

* <span data-ttu-id="aae04-2951">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-2951">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="aae04-2952">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="aae04-2952">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2953">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2953">VM</span></span>

* <span data-ttu-id="aae04-2954">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="aae04-2954">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="aae04-2955">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2955">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="aae04-2956">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="aae04-2956">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="aae04-2957">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="aae04-2957">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="aae04-2958">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2958">February 27, 2018</span></span>

<span data-ttu-id="aae04-2959">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="aae04-2959">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2960">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2960">Core</span></span>

* <span data-ttu-id="aae04-2961">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="aae04-2961">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="aae04-2962">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="aae04-2962">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="aae04-2963">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="aae04-2963">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2964">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2964">ACS</span></span>

* <span data-ttu-id="aae04-2965">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-2965">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="aae04-2966">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="aae04-2966">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="aae04-2967">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="aae04-2967">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="aae04-2968">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="aae04-2968">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-2969">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-2969">Appservice</span></span>

* <span data-ttu-id="aae04-2970">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="aae04-2970">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="aae04-2971">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="aae04-2971">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="aae04-2972">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2972">Cognitive Services</span></span>

* <span data-ttu-id="aae04-2973">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-2973">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-2974">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-2974">Consumption</span></span>

* <span data-ttu-id="aae04-2975">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="aae04-2975">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="aae04-2976">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="aae04-2976">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="aae04-2977">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-2977">Container</span></span>

* <span data-ttu-id="aae04-2978">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="aae04-2978">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="aae04-2979">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-2979">Network</span></span>

* <span data-ttu-id="aae04-2980">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="aae04-2980">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-2981">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-2981">Resource</span></span>

* <span data-ttu-id="aae04-2982">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="aae04-2982">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="aae04-2983">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-2983">Role</span></span>

* <span data-ttu-id="aae04-2984">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-2984">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-2985">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-2985">SQL</span></span>

* <span data-ttu-id="aae04-2986">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="aae04-2986">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-2987">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-2987">Storage</span></span>

* <span data-ttu-id="aae04-2988">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="aae04-2988">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-2989">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-2989">VM</span></span>

* <span data-ttu-id="aae04-2990">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-2990">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="aae04-2991">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-2991">February 13, 2018</span></span>

<span data-ttu-id="aae04-2992">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="aae04-2992">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="aae04-2993">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-2993">Core</span></span>

* <span data-ttu-id="aae04-2994">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="aae04-2994">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-2995">ACS</span></span>

* <span data-ttu-id="aae04-2996">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="aae04-2996">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="aae04-2997">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="aae04-2997">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="aae04-2998">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-2998">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="aae04-2999">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-2999">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="aae04-3000">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="aae04-3000">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="aae04-3001">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="aae04-3001">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="aae04-3002">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-3002">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="aae04-3003">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="aae04-3003">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3004">Appservice</span></span>

* <span data-ttu-id="aae04-3005">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="aae04-3005">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="aae04-3006">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="aae04-3006">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-3007">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-3007">CDN</span></span>

* <span data-ttu-id="aae04-3008">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3008">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="aae04-3009">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3009">Container</span></span>

* <span data-ttu-id="aae04-3010">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="aae04-3010">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="aae04-3011">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3011">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-3012">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3012">CosmosDB</span></span>

* <span data-ttu-id="aae04-3013">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="aae04-3013">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-3014">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-3014">Extension</span></span>

* <span data-ttu-id="aae04-3015">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3015">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="aae04-3016">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3016">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="aae04-3017">Comentários</span><span class="sxs-lookup"><span data-stu-id="aae04-3017">Feedback</span></span>

* <span data-ttu-id="aae04-3018">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="aae04-3018">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-3019">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3019">Interactive</span></span>

* <span data-ttu-id="aae04-3020">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="aae04-3020">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="aae04-3021">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="aae04-3021">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-3022">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3022">IoT</span></span>

* <span data-ttu-id="aae04-3023">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="aae04-3023">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="aae04-3024">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="aae04-3024">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="aae04-3025">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3025">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="aae04-3026">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="aae04-3026">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3027">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3027">Monitor</span></span>

* <span data-ttu-id="aae04-3028">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3028">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3029">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3029">Network</span></span>

* <span data-ttu-id="aae04-3030">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="aae04-3030">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="aae04-3031">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3031">Profile</span></span>

* <span data-ttu-id="aae04-3032">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3032">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3033">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3033">Resource</span></span>

* <span data-ttu-id="aae04-3034">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3034">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="aae04-3035">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-3035">Role</span></span>

* <span data-ttu-id="aae04-3036">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3036">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3037">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3037">SQL</span></span>

* <span data-ttu-id="aae04-3038">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="aae04-3038">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="aae04-3039">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="aae04-3039">Added `sql db rename`</span></span>
* <span data-ttu-id="aae04-3040">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="aae04-3040">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3041">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3041">Storage</span></span>

* <span data-ttu-id="aae04-3042">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="aae04-3042">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3043">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3043">VM</span></span>

* <span data-ttu-id="aae04-3044">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="aae04-3044">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="aae04-3045">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="aae04-3045">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="aae04-3046">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="aae04-3046">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="aae04-3047">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-3047">January 31, 2018</span></span>

<span data-ttu-id="aae04-3048">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="aae04-3048">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="aae04-3049">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3049">Core</span></span>

* <span data-ttu-id="aae04-3050">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="aae04-3050">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="aae04-3051">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="aae04-3051">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="aae04-3052">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="aae04-3052">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="aae04-3053">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="aae04-3053">Use `--verbose` to see</span></span>
* <span data-ttu-id="aae04-3054">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="aae04-3054">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3055">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3055">ACS</span></span>

* <span data-ttu-id="aae04-3056">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="aae04-3056">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="aae04-3057">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="aae04-3057">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3058">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3058">Appservice</span></span>

* <span data-ttu-id="aae04-3059">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="aae04-3059">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="aae04-3060">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="aae04-3060">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-3061">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-3061">CDN</span></span>

* <span data-ttu-id="aae04-3062">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3062">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-3063">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3063">CosmosDB</span></span>

* <span data-ttu-id="aae04-3064">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="aae04-3064">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-3065">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3065">Interactive</span></span>

* <span data-ttu-id="aae04-3066">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="aae04-3066">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3067">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3067">Network</span></span>

* <span data-ttu-id="aae04-3068">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3068">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="aae04-3069">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="aae04-3069">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="aae04-3070">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3070">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="aae04-3071">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3071">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="aae04-3072">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="aae04-3072">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="aae04-3073">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="aae04-3073">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="aae04-3074">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3074">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="aae04-3075">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="aae04-3075">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="aae04-3076">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="aae04-3076">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="aae04-3077">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="aae04-3077">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3078">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3078">Profile</span></span>

* <span data-ttu-id="aae04-3079">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="aae04-3079">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3080">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3080">Resource</span></span>

* <span data-ttu-id="aae04-3081">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="aae04-3081">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3082">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3082">Storage</span></span>

* <span data-ttu-id="aae04-3083">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="aae04-3083">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="aae04-3084">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="aae04-3084">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="aae04-3085">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-3085">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="aae04-3086">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3086">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="aae04-3087">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="aae04-3087">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3088">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3088">VM</span></span>

* <span data-ttu-id="aae04-3089">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="aae04-3089">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="aae04-3090">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="aae04-3090">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="aae04-3091">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="aae04-3091">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="aae04-3092">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3092">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="aae04-3093">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="aae04-3093">January 17, 2018</span></span>

<span data-ttu-id="aae04-3094">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="aae04-3094">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-3095">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3095">ACR</span></span>

* <span data-ttu-id="aae04-3096">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-3096">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="aae04-3097">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="aae04-3097">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3098">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3098">ACS</span></span>

* <span data-ttu-id="aae04-3099">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="aae04-3099">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="aae04-3100">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="aae04-3100">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3101">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3101">Appservice</span></span>

* <span data-ttu-id="aae04-3102">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="aae04-3102">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="aae04-3103">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="aae04-3103">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="aae04-3104">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="aae04-3104">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-3105">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-3105">Backup</span></span>

* <span data-ttu-id="aae04-3106">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="aae04-3106">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="aae04-3107">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="aae04-3107">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="aae04-3108">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-3108">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="aae04-3109">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="aae04-3109">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="aae04-3110">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-3110">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-3111">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3111">Batch</span></span>

* <span data-ttu-id="aae04-3112">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="aae04-3112">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="aae04-3113">Nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-3113">Cloud</span></span>

* <span data-ttu-id="aae04-3114">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-3114">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-3115">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-3115">Consumption</span></span>

* <span data-ttu-id="aae04-3116">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="aae04-3116">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="aae04-3117">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-3117">Event Grid</span></span>

* <span data-ttu-id="aae04-3118">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="aae04-3118">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="aae04-3119">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="aae04-3119">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="aae04-3120">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="aae04-3120">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="aae04-3121">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="aae04-3121">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="aae04-3122">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3122">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="aae04-3123">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3123">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="aae04-3124">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="aae04-3124">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="aae04-3125">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="aae04-3125">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-3126">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3126">Interactive</span></span>

* <span data-ttu-id="aae04-3127">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="aae04-3127">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="aae04-3128">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="aae04-3128">Fixed errors on startup</span></span>
* <span data-ttu-id="aae04-3129">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3129">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-3130">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3130">IoT</span></span>

* <span data-ttu-id="aae04-3131">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="aae04-3131">Added support for device provisioning service</span></span>
* <span data-ttu-id="aae04-3132">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="aae04-3132">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="aae04-3133">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3133">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3134">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3134">Monitor</span></span>

* <span data-ttu-id="aae04-3135">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="aae04-3135">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="aae04-3136">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3136">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="aae04-3137">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="aae04-3137">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3138">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3138">Network</span></span>

* <span data-ttu-id="aae04-3139">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3139">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="aae04-3140">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3140">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3141">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3141">Profile</span></span>

* <span data-ttu-id="aae04-3142">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-3142">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="aae04-3143">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-3143">Role</span></span>

* <span data-ttu-id="aae04-3144">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="aae04-3144">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aae04-3145">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-3145">Service Fabric</span></span>

* <span data-ttu-id="aae04-3146">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="aae04-3146">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="aae04-3147">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="aae04-3147">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3148">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3148">VM</span></span>

* <span data-ttu-id="aae04-3149">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="aae04-3149">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="aae04-3150">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="aae04-3150">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="aae04-3151">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="aae04-3151">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="aae04-3152">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="aae04-3152">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="aae04-3153">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="aae04-3153">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="aae04-3154">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3154">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="aae04-3155">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3155">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="aae04-3156">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="aae04-3156">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="aae04-3157">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3157">December 19, 2017</span></span>

<span data-ttu-id="aae04-3158">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="aae04-3158">Version 2.0.23</span></span>

* <span data-ttu-id="aae04-3159">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="aae04-3159">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="aae04-3160">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3160">Container</span></span>

* <span data-ttu-id="aae04-3161">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3161">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3162">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3162">Network</span></span>

* <span data-ttu-id="aae04-3163">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3163">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="aae04-3164">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3164">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3165">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3165">Storage</span></span>

* <span data-ttu-id="aae04-3166">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="aae04-3166">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3167">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3167">VM</span></span>

* <span data-ttu-id="aae04-3168">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="aae04-3168">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="aae04-3169">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3169">December 5, 2017</span></span>

<span data-ttu-id="aae04-3170">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="aae04-3170">Version 2.0.22</span></span>

* <span data-ttu-id="aae04-3171">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="aae04-3171">Removed `az component` commands.</span></span> <span data-ttu-id="aae04-3172">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="aae04-3172">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="aae04-3173">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3173">Core</span></span>
* <span data-ttu-id="aae04-3174">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="aae04-3174">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="aae04-3175">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3175">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3176">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3176">ACS</span></span>

* <span data-ttu-id="aae04-3177">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-3177">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="aae04-3178">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3178">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="aae04-3179">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="aae04-3179">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="aae04-3180">Supervisor</span><span class="sxs-lookup"><span data-stu-id="aae04-3180">Advisor</span></span>

* <span data-ttu-id="aae04-3181">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-3181">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3182">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3182">Appservice</span></span>

* <span data-ttu-id="aae04-3183">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="aae04-3183">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="aae04-3184">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="aae04-3184">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="aae04-3185">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="aae04-3185">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="aae04-3186">Consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-3186">Consumption</span></span>

* <span data-ttu-id="aae04-3187">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3187">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="aae04-3188">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3188">Container</span></span>

* <span data-ttu-id="aae04-3189">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-3189">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3190">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3190">Monitor</span></span>

* <span data-ttu-id="aae04-3191">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="aae04-3191">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3192">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3192">Resource</span></span>

* <span data-ttu-id="aae04-3193">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3193">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="aae04-3194">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-3194">Role</span></span>

* <span data-ttu-id="aae04-3195">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="aae04-3195">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="aae04-3196">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="aae04-3196">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="aae04-3197">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="aae04-3197">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3198">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3198">SQL</span></span>

* <span data-ttu-id="aae04-3199">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-3199">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="aae04-3200">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-3200">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3201">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3201">VM</span></span>

* <span data-ttu-id="aae04-3202">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="aae04-3202">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="aae04-3203">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3203">November 14, 2017</span></span>

<span data-ttu-id="aae04-3204">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="aae04-3204">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-3205">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3205">ACR</span></span>

* <span data-ttu-id="aae04-3206">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="aae04-3206">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="aae04-3207">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3207">ACS</span></span>

* <span data-ttu-id="aae04-3208">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="aae04-3208">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="aae04-3209">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3209">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="aae04-3210">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="aae04-3210">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="aae04-3211">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-3211">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="aae04-3212">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="aae04-3212">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3213">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3213">Appservice</span></span>

* <span data-ttu-id="aae04-3214">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="aae04-3214">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="aae04-3215">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="aae04-3215">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="aae04-3216">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="aae04-3216">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="aae04-3217">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="aae04-3217">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="aae04-3218">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-3218">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="aae04-3219">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="aae04-3219">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-3220">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3220">Batch</span></span>

* <span data-ttu-id="aae04-3221">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="aae04-3221">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-3222">Batchai</span><span class="sxs-lookup"><span data-stu-id="aae04-3222">Batchai</span></span>

* <span data-ttu-id="aae04-3223">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3223">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="aae04-3224">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3224">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="aae04-3225">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="aae04-3225">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="aae04-3226">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3226">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="aae04-3227">Nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-3227">Cloud</span></span>

* <span data-ttu-id="aae04-3228">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="aae04-3228">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="aae04-3229">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3229">Container</span></span>

* <span data-ttu-id="aae04-3230">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="aae04-3230">Added support to open multiple ports</span></span>
* <span data-ttu-id="aae04-3231">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="aae04-3231">Added container group restart policy</span></span>
* <span data-ttu-id="aae04-3232">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="aae04-3232">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="aae04-3233">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="aae04-3233">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aae04-3234">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-3234">Data Lake Analytics</span></span>

* <span data-ttu-id="aae04-3235">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="aae04-3235">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aae04-3236">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3236">Data Lake Store</span></span>

* <span data-ttu-id="aae04-3237">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="aae04-3237">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-3238">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-3238">Extension</span></span>

* <span data-ttu-id="aae04-3239">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="aae04-3239">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="aae04-3240">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="aae04-3240">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-3241">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3241">IoT</span></span>

* <span data-ttu-id="aae04-3242">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="aae04-3242">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3243">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3243">Monitor</span></span>

* <span data-ttu-id="aae04-3244">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="aae04-3244">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3245">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3245">Network</span></span>

* <span data-ttu-id="aae04-3246">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="aae04-3246">Added support for CAA DNS records</span></span>
* <span data-ttu-id="aae04-3247">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3247">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="aae04-3248">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="aae04-3248">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="aae04-3249">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="aae04-3249">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="aae04-3250">Reservas</span><span class="sxs-lookup"><span data-stu-id="aae04-3250">Reservations</span></span>

* <span data-ttu-id="aae04-3251">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-3251">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3252">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3252">Resource</span></span>

* <span data-ttu-id="aae04-3253">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3253">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3254">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3254">SQL</span></span>

* <span data-ttu-id="aae04-3255">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3255">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3256">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3256">Storage</span></span>

* <span data-ttu-id="aae04-3257">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-3257">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="aae04-3258">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="aae04-3258">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="aae04-3259">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="aae04-3259">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="aae04-3260">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="aae04-3260">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="aae04-3261">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3261">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="aae04-3262">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="aae04-3262">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="aae04-3263">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3263">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3264">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3264">VM</span></span>

* <span data-ttu-id="aae04-3265">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="aae04-3265">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="aae04-3266">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="aae04-3266">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="aae04-3267">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-3267">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="aae04-3268">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="aae04-3268">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="aae04-3269">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="aae04-3269">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="aae04-3270">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3270">October 24, 2017</span></span>

<span data-ttu-id="aae04-3271">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="aae04-3271">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="aae04-3272">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3272">Core</span></span>

* <span data-ttu-id="aae04-3273">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="aae04-3273">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-3274">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3274">ACR</span></span>

* <span data-ttu-id="aae04-3275">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="aae04-3275">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="aae04-3276">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="aae04-3276">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="aae04-3277">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="aae04-3277">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3278">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3278">ACS</span></span>

* <span data-ttu-id="aae04-3279">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="aae04-3279">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="aae04-3280">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="aae04-3280">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3281">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3281">Appservice</span></span>

* <span data-ttu-id="aae04-3282">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="aae04-3282">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="aae04-3283">Componente</span><span class="sxs-lookup"><span data-stu-id="aae04-3283">Component</span></span>

* <span data-ttu-id="aae04-3284">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="aae04-3284">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3285">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3285">Monitor</span></span>

* <span data-ttu-id="aae04-3286">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="aae04-3286">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3287">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3287">Resource</span></span>

* <span data-ttu-id="aae04-3288">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="aae04-3288">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="aae04-3289">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="aae04-3289">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3290">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3290">VM</span></span>

* <span data-ttu-id="aae04-3291">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3291">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="aae04-3292">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3292">October 9, 2017</span></span>

<span data-ttu-id="aae04-3293">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="aae04-3293">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="aae04-3294">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3294">Core</span></span>

* <span data-ttu-id="aae04-3295">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="aae04-3295">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3296">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3296">Appservice</span></span>

* <span data-ttu-id="aae04-3297">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3297">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-3298">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3298">Batch</span></span>

* <span data-ttu-id="aae04-3299">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-3299">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="aae04-3300">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="aae04-3300">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="aae04-3301">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3301">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="aae04-3302">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="aae04-3302">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="aae04-3303">Batchai</span><span class="sxs-lookup"><span data-stu-id="aae04-3303">Batchai</span></span>

* <span data-ttu-id="aae04-3304">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3304">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-3305">Keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-3305">Keyvault</span></span>

* <span data-ttu-id="aae04-3306">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="aae04-3306">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="aae04-3307">(#4448)</span><span class="sxs-lookup"><span data-stu-id="aae04-3307">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="aae04-3308">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3308">Network</span></span>

* <span data-ttu-id="aae04-3309">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="aae04-3309">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="aae04-3310">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="aae04-3310">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3311">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3311">Resource</span></span>

* <span data-ttu-id="aae04-3312">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="aae04-3312">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="aae04-3313">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-3313">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="aae04-3314">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="aae04-3314">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="aae04-3315">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3315">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3316">Sql</span><span class="sxs-lookup"><span data-stu-id="aae04-3316">Sql</span></span>

* <span data-ttu-id="aae04-3317">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="aae04-3317">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="aae04-3318">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="aae04-3318">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="aae04-3319">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="aae04-3319">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3320">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3320">Storage</span></span>

* <span data-ttu-id="aae04-3321">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="aae04-3321">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3322">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3322">Vm</span></span>

* <span data-ttu-id="aae04-3323">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="aae04-3323">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="aae04-3324">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3324">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="aae04-3325">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="aae04-3325">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="aae04-3326">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3326">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="aae04-3327">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3327">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="aae04-3328">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3328">September 22, 2017</span></span>

<span data-ttu-id="aae04-3329">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="aae04-3329">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3330">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3330">Resource</span></span>

* <span data-ttu-id="aae04-3331">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="aae04-3331">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="aae04-3332">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="aae04-3332">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="aae04-3333">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3333">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="aae04-3334">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="aae04-3334">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3335">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3335">Network</span></span>

* <span data-ttu-id="aae04-3336">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="aae04-3336">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="aae04-3337">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="aae04-3337">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="aae04-3338">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3338">Added `asg` application security group commands</span></span>
* <span data-ttu-id="aae04-3339">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3339">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="aae04-3340">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3340">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="aae04-3341">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3341">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="aae04-3342">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3342">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3343">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3343">Storage</span></span>

* <span data-ttu-id="aae04-3344">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="aae04-3344">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="aae04-3345">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-3345">Eventgrid</span></span>

* <span data-ttu-id="aae04-3346">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="aae04-3346">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3347">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3347">SQL</span></span>

* <span data-ttu-id="aae04-3348">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="aae04-3348">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="aae04-3349">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="aae04-3349">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="aae04-3350">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3350">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-3351">Keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-3351">Keyvault</span></span>

* <span data-ttu-id="aae04-3352">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="aae04-3352">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3353">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3353">VM</span></span>

* <span data-ttu-id="aae04-3354">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3354">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="aae04-3355">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="aae04-3355">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="aae04-3356">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3356">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="aae04-3357">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="aae04-3357">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="aae04-3358">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="aae04-3358">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="aae04-3359">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="aae04-3359">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3360">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3360">ACS</span></span>

* <span data-ttu-id="aae04-3361">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3361">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3362">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3362">Appservice</span></span>

* <span data-ttu-id="aae04-3363">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3363">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="aae04-3364">Backup</span><span class="sxs-lookup"><span data-stu-id="aae04-3364">Backup</span></span>

* <span data-ttu-id="aae04-3365">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-3365">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="aae04-3366">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3366">September 11, 2017</span></span>

<span data-ttu-id="aae04-3367">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="aae04-3367">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="aae04-3368">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3368">Core</span></span>

* <span data-ttu-id="aae04-3369">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="aae04-3369">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="aae04-3370">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="aae04-3370">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3371">Acs</span><span class="sxs-lookup"><span data-stu-id="aae04-3371">Acs</span></span>

* <span data-ttu-id="aae04-3372">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="aae04-3372">Added `acs list-locations` command</span></span>
* <span data-ttu-id="aae04-3373">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="aae04-3373">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3374">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3374">Appservice</span></span>

* <span data-ttu-id="aae04-3375">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3375">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-3376">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-3376">CDN</span></span>

* <span data-ttu-id="aae04-3377">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3377">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="aae04-3378">Extensão</span><span class="sxs-lookup"><span data-stu-id="aae04-3378">Extension</span></span>

* <span data-ttu-id="aae04-3379">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-3379">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-3380">Keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-3380">Keyvault</span></span>

* <span data-ttu-id="aae04-3381">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-3381">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3382">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3382">Network</span></span>

* <span data-ttu-id="aae04-3383">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="aae04-3383">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="aae04-3384">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3384">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="aae04-3385">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3385">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="aae04-3386">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3386">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="aae04-3387">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3387">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3388">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3388">Resource</span></span>

* <span data-ttu-id="aae04-3389">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3389">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="aae04-3390">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3390">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="aae04-3391">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="aae04-3391">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="aae04-3392">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="aae04-3392">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3393">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3393">SQL</span></span>

* <span data-ttu-id="aae04-3394">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="aae04-3394">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3395">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3395">VM</span></span>

* <span data-ttu-id="aae04-3396">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="aae04-3396">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="aae04-3397">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="aae04-3397">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="aae04-3398">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3398">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="aae04-3399">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-3399">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="aae04-3400">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="aae04-3400">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="aae04-3401">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3401">August 31, 2017</span></span>

<span data-ttu-id="aae04-3402">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="aae04-3402">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-3403">Keyvault</span><span class="sxs-lookup"><span data-stu-id="aae04-3403">Keyvault</span></span>

* <span data-ttu-id="aae04-3404">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="aae04-3404">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="aae04-3405">Sf</span><span class="sxs-lookup"><span data-stu-id="aae04-3405">Sf</span></span>

* <span data-ttu-id="aae04-3406">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="aae04-3406">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3407">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3407">Storage</span></span>

* <span data-ttu-id="aae04-3408">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="aae04-3408">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="aae04-3409">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="aae04-3409">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="aae04-3410">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3410">August 28, 2017</span></span>

<span data-ttu-id="aae04-3411">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="aae04-3411">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="aae04-3412">CLI</span><span class="sxs-lookup"><span data-stu-id="aae04-3412">CLI</span></span>

* <span data-ttu-id="aae04-3413">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="aae04-3413">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3414">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3414">ACS</span></span>

* <span data-ttu-id="aae04-3415">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="aae04-3415">Corrected preview regions</span></span>
* <span data-ttu-id="aae04-3416">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="aae04-3416">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="aae04-3417">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="aae04-3417">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3418">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3418">Appservice</span></span>

* <span data-ttu-id="aae04-3419">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3419">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="aae04-3420">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-3420">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="aae04-3421">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3421">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="aae04-3422">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3422">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="aae04-3423">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3423">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-3424">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3424">IoT</span></span>

* <span data-ttu-id="aae04-3425">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="aae04-3425">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3426">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3426">Network</span></span>

* <span data-ttu-id="aae04-3427">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="aae04-3427">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="aae04-3428">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3428">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="aae04-3429">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="aae04-3429">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="aae04-3430">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3430">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="aae04-3431">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3431">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3432">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3432">Profile</span></span>

* <span data-ttu-id="aae04-3433">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="aae04-3433">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aae04-3434">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-3434">Service Fabric</span></span>

* <span data-ttu-id="aae04-3435">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="aae04-3435">Preview release</span></span>
* <span data-ttu-id="aae04-3436">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="aae04-3436">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="aae04-3437">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="aae04-3437">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="aae04-3438">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="aae04-3438">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3439">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3439">Storage</span></span>

* <span data-ttu-id="aae04-3440">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="aae04-3440">Enabled setting blob tier</span></span>
* <span data-ttu-id="aae04-3441">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="aae04-3441">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="aae04-3442">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="aae04-3442">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="aae04-3443">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="aae04-3443">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="aae04-3444">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3444">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="aae04-3445">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="aae04-3445">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3446">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3446">VM</span></span>

* <span data-ttu-id="aae04-3447">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="aae04-3447">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="aae04-3448">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-3448">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="aae04-3449">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3449">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="aae04-3450">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="aae04-3450">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="aae04-3451">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="aae04-3451">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="aae04-3452">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3452">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="aae04-3453">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3453">August 15, 2017</span></span>

<span data-ttu-id="aae04-3454">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="aae04-3454">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3455">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3455">ACS</span></span>

* <span data-ttu-id="aae04-3456">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="aae04-3456">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3457">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3457">Appservice</span></span>

* <span data-ttu-id="aae04-3458">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="aae04-3458">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="aae04-3459">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-3459">Event Grid</span></span>

* <span data-ttu-id="aae04-3460">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="aae04-3460">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="aae04-3461">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3461">August 11, 2017</span></span>

<span data-ttu-id="aae04-3462">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="aae04-3462">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3463">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3463">ACS</span></span>

* <span data-ttu-id="aae04-3464">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="aae04-3464">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-3465">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3465">Batch</span></span>

* <span data-ttu-id="aae04-3466">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="aae04-3466">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="aae04-3467">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-3467">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="aae04-3468">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3468">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="aae04-3469">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="aae04-3469">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="aae04-3470">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="aae04-3470">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="aae04-3471">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="aae04-3471">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="aae04-3472">Componente</span><span class="sxs-lookup"><span data-stu-id="aae04-3472">Component</span></span>

* <span data-ttu-id="aae04-3473">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="aae04-3473">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="aae04-3474">Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3474">Container</span></span>

* <span data-ttu-id="aae04-3475">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="aae04-3475">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="aae04-3476">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3476">Data Lake Store</span></span>

* <span data-ttu-id="aae04-3477">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3477">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="aae04-3478">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="aae04-3478">Event Grid</span></span>

* <span data-ttu-id="aae04-3479">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="aae04-3479">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3480">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3480">Network</span></span>

* <span data-ttu-id="aae04-3481">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="aae04-3481">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="aae04-3482">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="aae04-3482">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="aae04-3483">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="aae04-3483">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="aae04-3484">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="aae04-3484">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3485">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3485">Profile</span></span>

* <span data-ttu-id="aae04-3486">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="aae04-3486">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3487">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3487">Storage</span></span>

* <span data-ttu-id="aae04-3488">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="aae04-3488">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3489">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3489">VM</span></span>

* <span data-ttu-id="aae04-3490">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="aae04-3490">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="aae04-3491">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="aae04-3491">Exposed `list-skus` command</span></span>
* <span data-ttu-id="aae04-3492">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="aae04-3492">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="aae04-3493">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="aae04-3493">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="aae04-3494">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-3494">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="aae04-3495">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3495">July 28, 2017</span></span>

<span data-ttu-id="aae04-3496">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="aae04-3496">Version 2.0.12</span></span>

* <span data-ttu-id="aae04-3497">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3497">Added container commands</span></span>
* <span data-ttu-id="aae04-3498">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="aae04-3498">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="aae04-3499">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3499">Core</span></span>

* <span data-ttu-id="aae04-3500">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="aae04-3500">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="aae04-3501">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="aae04-3501">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="aae04-3502">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="aae04-3502">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="aae04-3503">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="aae04-3503">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="aae04-3504">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="aae04-3504">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="aae04-3505">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="aae04-3505">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="aae04-3506">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="aae04-3506">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="aae04-3507">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="aae04-3507">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="aae04-3508">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="aae04-3508">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="aae04-3509">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="aae04-3509">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="aae04-3510">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="aae04-3510">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="aae04-3511">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="aae04-3511">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="aae04-3512">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-3512">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="aae04-3513">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="aae04-3513">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="aae04-3514">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="aae04-3514">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="aae04-3515">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="aae04-3515">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="aae04-3516">ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3516">ACR</span></span>

* <span data-ttu-id="aae04-3517">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-3517">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="aae04-3518">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="aae04-3518">Support SKU update for managed registries</span></span>
* <span data-ttu-id="aae04-3519">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="aae04-3519">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="aae04-3520">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3520">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="aae04-3521">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3521">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="aae04-3522">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="aae04-3522">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3523">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3523">ACS</span></span>

* <span data-ttu-id="aae04-3524">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="aae04-3524">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3525">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3525">Appservice</span></span>

* <span data-ttu-id="aae04-3526">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="aae04-3526">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="aae04-3527">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="aae04-3527">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="aae04-3528">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="aae04-3528">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="aae04-3529">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="aae04-3529">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="aae04-3530">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="aae04-3530">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="aae04-3531">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="aae04-3531">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="aae04-3532">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="aae04-3532">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="aae04-3533">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="aae04-3533">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="aae04-3534">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="aae04-3534">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="aae04-3535">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="aae04-3535">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="aae04-3536">Lote</span><span class="sxs-lookup"><span data-stu-id="aae04-3536">Batch</span></span>

* <span data-ttu-id="aae04-3537">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="aae04-3537">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="aae04-3538">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="aae04-3538">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="aae04-3539">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="aae04-3539">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="aae04-3540">CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-3540">CDN</span></span>

* <span data-ttu-id="aae04-3541">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="aae04-3541">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="aae04-3542">Nuvem</span><span class="sxs-lookup"><span data-stu-id="aae04-3542">Cloud</span></span>

* <span data-ttu-id="aae04-3543">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="aae04-3543">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="aae04-3544">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="aae04-3544">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="aae04-3545">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="aae04-3545">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="aae04-3546">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="aae04-3546">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="aae04-3547">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="aae04-3547">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-3548">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3548">CosmosDB</span></span>

* <span data-ttu-id="aae04-3549">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="aae04-3549">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="aae04-3550">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="aae04-3550">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aae04-3551">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-3551">Data Lake Analytics</span></span>

* <span data-ttu-id="aae04-3552">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="aae04-3552">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="aae04-3553">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3553">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="aae04-3554">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="aae04-3554">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aae04-3555">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3555">Data Lake Store</span></span>

* <span data-ttu-id="aae04-3556">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3556">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="aae04-3557">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="aae04-3557">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="aae04-3558">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="aae04-3558">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="aae04-3559">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3559">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="aae04-3560">Interativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3560">Interactive</span></span>

* <span data-ttu-id="aae04-3561">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="aae04-3561">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="aae04-3562">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="aae04-3562">Increased test coverage</span></span>
* <span data-ttu-id="aae04-3563">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="aae04-3563">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="aae04-3564">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="aae04-3564">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="aae04-3565">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="aae04-3565">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="aae04-3566">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="aae04-3566">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="aae04-3567">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="aae04-3567">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="aae04-3568">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="aae04-3568">Added `--progress` flag</span></span>
* <span data-ttu-id="aae04-3569">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="aae04-3569">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="aae04-3570">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="aae04-3570">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="aae04-3571">IoT</span><span class="sxs-lookup"><span data-stu-id="aae04-3571">IoT</span></span>

* <span data-ttu-id="aae04-3572">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="aae04-3572">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="aae04-3573">(#3934)</span><span class="sxs-lookup"><span data-stu-id="aae04-3573">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="aae04-3574">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="aae04-3574">Key vault</span></span>

* <span data-ttu-id="aae04-3575">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="aae04-3575">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="aae04-3576">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="aae04-3576">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="aae04-3577">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="aae04-3577">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="aae04-3578">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="aae04-3578">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="aae04-3579">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="aae04-3579">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="aae04-3580">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="aae04-3580">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="aae04-3581">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="aae04-3581">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="aae04-3582">(#3307)</span><span class="sxs-lookup"><span data-stu-id="aae04-3582">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="aae04-3583">Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3583">Lab</span></span>

* <span data-ttu-id="aae04-3584">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="aae04-3584">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="aae04-3585">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3585">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3586">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3586">Monitor</span></span>

* <span data-ttu-id="aae04-3587">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="aae04-3587">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="aae04-3588">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="aae04-3588">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="aae04-3589">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="aae04-3589">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="aae04-3590">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="aae04-3590">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="aae04-3591">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="aae04-3591">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="aae04-3592">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="aae04-3592">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="aae04-3593">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="aae04-3593">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="aae04-3594">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="aae04-3594">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="aae04-3595">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="aae04-3595">`location` no longer required</span></span>
  * <span data-ttu-id="aae04-3596">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="aae04-3596">Add name and ID support for target</span></span>
  * <span data-ttu-id="aae04-3597">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-3597">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="aae04-3598">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="aae04-3598">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="aae04-3599">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="aae04-3599">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="aae04-3600">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="aae04-3600">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="aae04-3601">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="aae04-3601">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="aae04-3602">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3602">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3603">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3603">Network</span></span>

* <span data-ttu-id="aae04-3604">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="aae04-3604">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="aae04-3605">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3605">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="aae04-3606">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="aae04-3606">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="aae04-3607">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="aae04-3607">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="aae04-3608">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3608">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="aae04-3609">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="aae04-3609">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="aae04-3610">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3610">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="aae04-3611">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="aae04-3611">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="aae04-3612">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="aae04-3612">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="aae04-3613">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="aae04-3613">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="aae04-3614">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3614">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="aae04-3615">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="aae04-3615">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="aae04-3616">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="aae04-3616">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="aae04-3617">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3617">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="aae04-3618">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3618">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="aae04-3619">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3619">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="aae04-3620">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="aae04-3620">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="aae04-3621">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="aae04-3621">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="aae04-3622">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3622">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="aae04-3623">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3623">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="aae04-3624">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3624">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="aae04-3625">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="aae04-3625">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="aae04-3626">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="aae04-3626">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="aae04-3627">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="aae04-3627">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="aae04-3628">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="aae04-3628">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="aae04-3629">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="aae04-3629">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="aae04-3630">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="aae04-3630">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3631">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3631">Profile</span></span>

* <span data-ttu-id="aae04-3632">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="aae04-3632">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="aae04-3633">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="aae04-3633">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="aae04-3634">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="aae04-3634">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="aae04-3635">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="aae04-3635">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="aae04-3636">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="aae04-3636">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="aae04-3637">RDBMS</span><span class="sxs-lookup"><span data-stu-id="aae04-3637">RDBMS</span></span>

* <span data-ttu-id="aae04-3638">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="aae04-3638">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="aae04-3639">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="aae04-3639">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="aae04-3640">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="aae04-3640">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="aae04-3641">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="aae04-3641">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3642">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3642">Resource</span></span>

* <span data-ttu-id="aae04-3643">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3643">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="aae04-3644">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="aae04-3644">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="aae04-3645">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="aae04-3645">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="aae04-3646">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="aae04-3646">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="aae04-3647">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="aae04-3647">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="aae04-3648">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="aae04-3648">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="aae04-3649">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="aae04-3649">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="aae04-3650">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="aae04-3650">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="aae04-3651">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-3651">Role</span></span>

* <span data-ttu-id="aae04-3652">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="aae04-3652">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="aae04-3653">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="aae04-3653">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="aae04-3654">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="aae04-3654">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="aae04-3655">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="aae04-3655">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="aae04-3656">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="aae04-3656">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="aae04-3657">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-3657">Service Fabric</span></span>
* <span data-ttu-id="aae04-3658">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="aae04-3658">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="aae04-3659">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="aae04-3659">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="aae04-3660">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="aae04-3660">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3661">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3661">SQL</span></span>

* <span data-ttu-id="aae04-3662">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="aae04-3662">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="aae04-3663">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="aae04-3663">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="aae04-3664">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="aae04-3664">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3665">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3665">Storage</span></span>

* <span data-ttu-id="aae04-3666">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="aae04-3666">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="aae04-3667">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="aae04-3667">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="aae04-3668">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="aae04-3668">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="aae04-3669">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="aae04-3669">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="aae04-3670">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="aae04-3670">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="aae04-3671">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="aae04-3671">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3672">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3672">VM</span></span>

* <span data-ttu-id="aae04-3673">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="aae04-3673">Support configuring nsg</span></span>
* <span data-ttu-id="aae04-3674">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3674">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="aae04-3675">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="aae04-3675">Support managed service identities</span></span>
* <span data-ttu-id="aae04-3676">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="aae04-3676">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="aae04-3677">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="aae04-3677">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="aae04-3678">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3678">May 10, 2017</span></span>

<span data-ttu-id="aae04-3679">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="aae04-3679">Version 2.0.6</span></span>

* <span data-ttu-id="aae04-3680">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3680">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="aae04-3681">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="aae04-3681">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="aae04-3682">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3682">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="aae04-3683">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="aae04-3683">Include Cognitive Services module</span></span>
* <span data-ttu-id="aae04-3684">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="aae04-3684">Include Service Fabric module</span></span>
* <span data-ttu-id="aae04-3685">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="aae04-3685">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="aae04-3686">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="aae04-3686">Add support for CDN commands</span></span>
* <span data-ttu-id="aae04-3687">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="aae04-3687">Remove Container module</span></span>
* <span data-ttu-id="aae04-3688">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="aae04-3688">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="aae04-3689">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="aae04-3689">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="aae04-3690">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3690">Core</span></span>

* <span data-ttu-id="aae04-3691">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="aae04-3691">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="aae04-3692">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="aae04-3692">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="aae04-3693">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="aae04-3693">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="aae04-3694">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="aae04-3694">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="aae04-3695">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="aae04-3695">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="aae04-3696">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="aae04-3696">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="aae04-3697">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="aae04-3697">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="aae04-3698">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="aae04-3698">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="aae04-3699">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="aae04-3699">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="aae04-3700">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="aae04-3700">core: Improved performance</span></span>
* <span data-ttu-id="aae04-3701">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="aae04-3701">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="aae04-3702">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="aae04-3702">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3703">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3703">ACS</span></span>

* <span data-ttu-id="aae04-3704">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aae04-3704">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="aae04-3705">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="aae04-3705">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="aae04-3706">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="aae04-3706">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="aae04-3707">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="aae04-3707">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3708">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3708">AppService</span></span>

* <span data-ttu-id="aae04-3709">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="aae04-3709">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="aae04-3710">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="aae04-3710">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="aae04-3711">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="aae04-3711">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="aae04-3712">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="aae04-3712">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="aae04-3713">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="aae04-3713">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="aae04-3714">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="aae04-3714">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="aae04-3715">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="aae04-3715">support slot swap with preview</span></span>
* <span data-ttu-id="aae04-3716">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="aae04-3716">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="aae04-3717">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="aae04-3717">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="aae04-3718">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3718">CosmosDB</span></span>

* <span data-ttu-id="aae04-3719">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3719">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="aae04-3720">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="aae04-3720">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="aae04-3721">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="aae04-3721">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="aae04-3722">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="aae04-3722">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="aae04-3723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-3723">Data Lake Analytics</span></span>

* <span data-ttu-id="aae04-3724">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="aae04-3724">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="aae04-3725">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="aae04-3725">Add support for new catalog item type: package.</span></span> <span data-ttu-id="aae04-3726">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="aae04-3726">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="aae04-3727">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="aae04-3727">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="aae04-3728">Tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-3728">Table</span></span>
  * <span data-ttu-id="aae04-3729">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-3729">Table valued function</span></span>
  * <span data-ttu-id="aae04-3730">Visualizar</span><span class="sxs-lookup"><span data-stu-id="aae04-3730">View</span></span>
  * <span data-ttu-id="aae04-3731">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="aae04-3731">Table Statistics.</span></span> <span data-ttu-id="aae04-3732">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="aae04-3732">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="aae04-3733">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3733">Data Lake Store</span></span>

* <span data-ttu-id="aae04-3734">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="aae04-3734">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="aae04-3735">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="aae04-3735">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="aae04-3736">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="aae04-3736">missed help for access show.</span></span> <span data-ttu-id="aae04-3737">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="aae04-3737">adding it.</span></span> <span data-ttu-id="aae04-3738">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="aae04-3738">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="aae04-3739">Localizar</span><span class="sxs-lookup"><span data-stu-id="aae04-3739">Find</span></span>

* <span data-ttu-id="aae04-3740">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="aae04-3740">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="aae04-3741">KeyVault</span><span class="sxs-lookup"><span data-stu-id="aae04-3741">KeyVault</span></span>

* <span data-ttu-id="aae04-3742">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="aae04-3742">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="aae04-3743">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="aae04-3743">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="aae04-3744">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="aae04-3744">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="aae04-3745">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="aae04-3745">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="aae04-3746">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="aae04-3746">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="aae04-3747">Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3747">Lab</span></span>

* <span data-ttu-id="aae04-3748">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3748">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="aae04-3749">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3749">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="aae04-3750">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3750">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="aae04-3751">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3751">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="aae04-3752">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="aae04-3752">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="aae04-3753">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="aae04-3753">Monitor</span></span>

* <span data-ttu-id="aae04-3754">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="aae04-3754">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="aae04-3755">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="aae04-3755">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="aae04-3756">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3756">Network</span></span>

* <span data-ttu-id="aae04-3757">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="aae04-3757">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="aae04-3758">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3758">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="aae04-3759">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3759">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="aae04-3760">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aae04-3760">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="aae04-3761">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="aae04-3761">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="aae04-3762">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="aae04-3762">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="aae04-3763">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="aae04-3763">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="aae04-3764">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="aae04-3764">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="aae04-3765">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="aae04-3765">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="aae04-3766">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="aae04-3766">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="aae04-3767">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="aae04-3767">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="aae04-3768">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3768">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="aae04-3769">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3769">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="aae04-3770">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="aae04-3770">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="aae04-3771">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="aae04-3771">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="aae04-3772">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="aae04-3772">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="aae04-3773">Perfil</span><span class="sxs-lookup"><span data-stu-id="aae04-3773">Profile</span></span>

* <span data-ttu-id="aae04-3774">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="aae04-3774">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="aae04-3775">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="aae04-3775">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="aae04-3776">Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-3776">Redis</span></span>

* <span data-ttu-id="aae04-3777">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="aae04-3777">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="aae04-3778">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="aae04-3778">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="aae04-3779">Recurso</span><span class="sxs-lookup"><span data-stu-id="aae04-3779">Resource</span></span>

* <span data-ttu-id="aae04-3780">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="aae04-3780">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="aae04-3781">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="aae04-3781">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="aae04-3782">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="aae04-3782">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="aae04-3783">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="aae04-3783">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="aae04-3784">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="aae04-3784">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="aae04-3785">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="aae04-3785">Add docs for az lock update.</span></span> <span data-ttu-id="aae04-3786">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="aae04-3786">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="aae04-3787">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="aae04-3787">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="aae04-3788">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="aae04-3788">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="aae04-3789">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="aae04-3789">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="aae04-3790">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="aae04-3790">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="aae04-3791">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="aae04-3791">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="aae04-3792">Função</span><span class="sxs-lookup"><span data-stu-id="aae04-3792">Role</span></span>

* <span data-ttu-id="aae04-3793">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="aae04-3793">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="aae04-3794">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="aae04-3794">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="aae04-3795">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="aae04-3795">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="aae04-3796">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="aae04-3796">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="aae04-3797">SQL</span><span class="sxs-lookup"><span data-stu-id="aae04-3797">SQL</span></span>

* <span data-ttu-id="aae04-3798">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="aae04-3798">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="aae04-3799">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="aae04-3799">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="aae04-3800">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3800">Storage</span></span>

* <span data-ttu-id="aae04-3801">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="aae04-3801">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="aae04-3802">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="aae04-3802">Add support for incremental blob copy</span></span>
* <span data-ttu-id="aae04-3803">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="aae04-3803">Add support for large block blob upload</span></span>
* <span data-ttu-id="aae04-3804">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="aae04-3804">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3805">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3805">VM</span></span>

* <span data-ttu-id="aae04-3806">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="aae04-3806">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="aae04-3807">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="aae04-3807">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="aae04-3808">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="aae04-3808">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="aae04-3809">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="aae04-3809">az vm/vmss disk</span></span>
  3. <span data-ttu-id="aae04-3810">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="aae04-3810">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="aae04-3811">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="aae04-3811">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="aae04-3812">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="aae04-3812">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="aae04-3813">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3813">April 3, 2017</span></span>

<span data-ttu-id="aae04-3814">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="aae04-3814">Version 2.0.2</span></span>

<span data-ttu-id="aae04-3815">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="aae04-3815">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="aae04-3816">Núcleo</span><span class="sxs-lookup"><span data-stu-id="aae04-3816">Core</span></span>

* <span data-ttu-id="aae04-3817">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-3817">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="aae04-3818">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="aae04-3818">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="aae04-3819">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="aae04-3819">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="aae04-3820">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="aae04-3820">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="aae04-3821">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="aae04-3821">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="aae04-3822">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="aae04-3822">Add prompting for missing template parameters.</span></span> <span data-ttu-id="aae04-3823">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="aae04-3823">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="aae04-3824">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="aae04-3824">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="aae04-3825">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="aae04-3825">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="aae04-3826">ACS</span><span class="sxs-lookup"><span data-stu-id="aae04-3826">ACS</span></span>

* <span data-ttu-id="aae04-3827">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="aae04-3827">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="aae04-3828">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="aae04-3828">Add support for ssh key password prompting.</span></span> <span data-ttu-id="aae04-3829">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="aae04-3829">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="aae04-3830">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="aae04-3830">Add support for windows clusters.</span></span> <span data-ttu-id="aae04-3831">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="aae04-3831">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="aae04-3832">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="aae04-3832">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="aae04-3833">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="aae04-3833">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="aae04-3834">AppService</span><span class="sxs-lookup"><span data-stu-id="aae04-3834">AppService</span></span>

* <span data-ttu-id="aae04-3835">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="aae04-3835">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="aae04-3836">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="aae04-3836">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="aae04-3837">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="aae04-3837">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="aae04-3838">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="aae04-3838">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="aae04-3839">DataLake</span><span class="sxs-lookup"><span data-stu-id="aae04-3839">DataLake</span></span>

* <span data-ttu-id="aae04-3840">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="aae04-3840">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="aae04-3841">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="aae04-3841">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="aae04-3842">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="aae04-3842">DocuemntDB</span></span>

* <span data-ttu-id="aae04-3843">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="aae04-3843">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="aae04-3844">VM</span><span class="sxs-lookup"><span data-stu-id="aae04-3844">VM</span></span>

* <span data-ttu-id="aae04-3845">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="aae04-3845">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="aae04-3846">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="aae04-3846">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="aae04-3847">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="aae04-3847">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="aae04-3848">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="aae04-3848">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="aae04-3849">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="aae04-3849">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="aae04-3850">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="aae04-3850">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="aae04-3851">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="aae04-3851">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="aae04-3852">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="aae04-3852">February 27, 2017</span></span>

<span data-ttu-id="aae04-3853">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="aae04-3853">Version 2.0.0</span></span>

<span data-ttu-id="aae04-3854">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="aae04-3854">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="aae04-3855">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="aae04-3855">Container Service (acs)</span></span>
- <span data-ttu-id="aae04-3856">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="aae04-3856">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="aae04-3857">Rede</span><span class="sxs-lookup"><span data-stu-id="aae04-3857">Networking</span></span>
- <span data-ttu-id="aae04-3858">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="aae04-3858">Storage</span></span>

<span data-ttu-id="aae04-3859">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="aae04-3859">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="aae04-3860">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-3860">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="aae04-3861">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="aae04-3861">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="aae04-3862">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="aae04-3862">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="aae04-3863">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="aae04-3863">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="aae04-3864">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="aae04-3864">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="aae04-3865">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="aae04-3865">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="aae04-3866">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="aae04-3866">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="aae04-3867">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="aae04-3867">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="aae04-3868">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="aae04-3868">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="aae04-3869">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="aae04-3869">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="aae04-3870">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="aae04-3870">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="aae04-3871">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="aae04-3871">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="aae04-3872">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="aae04-3872">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="aae04-3873">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="aae04-3873">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="aae04-3874">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="aae04-3874">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="aae04-3875">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="aae04-3875">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="aae04-3876">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.</span><span class="sxs-lookup"><span data-stu-id="aae04-3876">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="aae04-3877">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="aae04-3877">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="aae04-3878">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="aae04-3878">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
