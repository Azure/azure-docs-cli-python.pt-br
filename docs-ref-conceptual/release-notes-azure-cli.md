---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 07/16/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8f134b28c3c2c288a0a0faa0fcb64c109cb1970
ms.sourcegitcommit: c473377d1c08ac4efd2480bf852c30dbf1044a57
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2020
ms.locfileid: "86415303"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="beb0e-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="beb0e-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="beb0e-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="july-16-2020"></a><span data-ttu-id="beb0e-105">16 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-105">July 16, 2020</span></span>

<span data-ttu-id="beb0e-106">Versão 2.9.1</span><span class="sxs-lookup"><span data-stu-id="beb0e-106">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-107">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-107">AKS</span></span>

* <span data-ttu-id="beb0e-108">Remove a configuração explícita de VMSS no comando de exemplo do Windows, pois ele agora é padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-108">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-109">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-109">IoT</span></span>

* <span data-ttu-id="beb0e-110">[ALTERAÇÃO DA FALHA] `az iot pnp`: Remove comandos de versão prévia do IoT PNP da CLI principal</span><span class="sxs-lookup"><span data-stu-id="beb0e-110">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="beb0e-111">REST</span><span class="sxs-lookup"><span data-stu-id="beb0e-111">REST</span></span>

* <span data-ttu-id="beb0e-112">Correção nº14152: `az rest`: aceita URLs do ARM sem a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-112">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-113">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-113">Storage</span></span>

* <span data-ttu-id="beb0e-114">Correção nº 14138: torna algumas permissões opcionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-114">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="beb0e-115">14 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-115">July 14, 2020</span></span>

<span data-ttu-id="beb0e-116">Versão 2.9.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-116">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-117">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-117">ACR</span></span>

* <span data-ttu-id="beb0e-118">Manipular o link do artefato de log do Registro para os logs de fluxo</span><span class="sxs-lookup"><span data-stu-id="beb0e-118">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="beb0e-119">Substituir comandos helm2</span><span class="sxs-lookup"><span data-stu-id="beb0e-119">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-120">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-120">AKS</span></span>

* <span data-ttu-id="beb0e-121">`az aks create`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="beb0e-121">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="beb0e-122">`az aks update`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="beb0e-122">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="beb0e-123">APIM</span><span class="sxs-lookup"><span data-stu-id="beb0e-123">APIM</span></span>

* <span data-ttu-id="beb0e-124">Comandos az apim api gerais adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-124">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-125">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-125">AppConfig</span></span>

* <span data-ttu-id="beb0e-126">Adicionar exemplo para usar --fields na revisão do appconfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-126">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-127">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-127">AppService</span></span>

* <span data-ttu-id="beb0e-128">`az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-128">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="beb0e-129">Suporte à API de pilhas adicionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-129">Added Stacks API Support.</span></span>
* <span data-ttu-id="beb0e-130">Correção nº 14208 falha na criação de um aplicativo com vários contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-130">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="beb0e-131">Corrige az webapp create – usa pilhas de runtime embutidas em código</span><span class="sxs-lookup"><span data-stu-id="beb0e-131">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-132">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-132">ARM</span></span>

* <span data-ttu-id="beb0e-133">`az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="beb0e-133">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-134">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-134">Compute</span></span>

* <span data-ttu-id="beb0e-135">Avançar os discos de versão 2020-05-01, computação 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-135">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="beb0e-136">Criptografia dupla do conjunto de criptografia de disco</span><span class="sxs-lookup"><span data-stu-id="beb0e-136">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="beb0e-137">`az vmss update`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="beb0e-137">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="beb0e-138">`az sig image-version create`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="beb0e-138">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="beb0e-139">vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-139">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="beb0e-140">Adicionar operação de remoção simulada para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-140">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-141">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-141">CosmosDB</span></span>

* <span data-ttu-id="beb0e-142">Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="beb0e-142">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="beb0e-143">EventGrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-143">EventGrid</span></span>

* <span data-ttu-id="beb0e-144">Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="beb0e-144">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="beb0e-145">Localizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-145">Find</span></span>

* <span data-ttu-id="beb0e-146">Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada</span><span class="sxs-lookup"><span data-stu-id="beb0e-146">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-147">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-147">HDInsight</span></span>

* <span data-ttu-id="beb0e-148">Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-148">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-149">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-149">Monitor</span></span>

* <span data-ttu-id="beb0e-150">Remover sinalizador de visualização para comandos no workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-150">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="beb0e-151">`az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-151">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="beb0e-152">`az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica</span><span class="sxs-lookup"><span data-stu-id="beb0e-152">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="beb0e-153">`az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-153">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-154">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-154">Network</span></span>

* <span data-ttu-id="beb0e-155">`az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="beb0e-155">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="beb0e-156">Avançar azure-mgmt-network para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-156">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="beb0e-157">`az network express-route gateway connection`: dá suporte à configuração de roteamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-157">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="beb0e-158">`az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.</span><span class="sxs-lookup"><span data-stu-id="beb0e-158">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="beb0e-159">Recurso de link privado de suporte do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-159">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="beb0e-160">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="beb0e-160">PolicyInsights</span></span>

* <span data-ttu-id="beb0e-161">`az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política</span><span class="sxs-lookup"><span data-stu-id="beb0e-161">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="beb0e-162">`az policy state list`: expõe versões de entidades de política em cada registro de conformidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-162">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-163">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-163">Profile</span></span>

* <span data-ttu-id="beb0e-164">`az account get-access-token`: Mostra expiresOn para Identidade Gerenciada</span><span class="sxs-lookup"><span data-stu-id="beb0e-164">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-165">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-165">RDBMS</span></span>

* <span data-ttu-id="beb0e-166">Dar suporte à versão mínima do TLS</span><span class="sxs-lookup"><span data-stu-id="beb0e-166">Support Minimum TLS version</span></span>
* <span data-ttu-id="beb0e-167">Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-167">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="beb0e-168">Segurança</span><span class="sxs-lookup"><span data-stu-id="beb0e-168">Security</span></span>

* <span data-ttu-id="beb0e-169">Adicionar comandos allowed_connections</span><span class="sxs-lookup"><span data-stu-id="beb0e-169">Add allowed_connections commands</span></span>
* <span data-ttu-id="beb0e-170">Adicionar comandos hardeningss da rede adaptável</span><span class="sxs-lookup"><span data-stu-id="beb0e-170">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="beb0e-171">Adicionar comandos adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="beb0e-171">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="beb0e-172">Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-172">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="beb0e-173">Adicionar CLI de conformidade regulatória</span><span class="sxs-lookup"><span data-stu-id="beb0e-173">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="beb0e-174">SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-174">SignalR</span></span>

* <span data-ttu-id="beb0e-175">Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream</span><span class="sxs-lookup"><span data-stu-id="beb0e-175">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-176">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-176">SQL</span></span>

* <span data-ttu-id="beb0e-177">`az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-177">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="beb0e-178">`az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário</span><span class="sxs-lookup"><span data-stu-id="beb0e-178">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-179">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-179">Storage</span></span>

* <span data-ttu-id="beb0e-180">`az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-180">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="beb0e-181">`az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-181">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="beb0e-182">Remover credencial de token de check-in</span><span class="sxs-lookup"><span data-stu-id="beb0e-182">Remove check in token credential</span></span>
* <span data-ttu-id="beb0e-183">Corrigir o nome da conta de armazenamento em exemplos</span><span class="sxs-lookup"><span data-stu-id="beb0e-183">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="beb0e-184">Webapp</span><span class="sxs-lookup"><span data-stu-id="beb0e-184">Webapp</span></span>

* <span data-ttu-id="beb0e-185">Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log</span><span class="sxs-lookup"><span data-stu-id="beb0e-185">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="beb0e-186">Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet</span><span class="sxs-lookup"><span data-stu-id="beb0e-186">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="beb0e-187">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-187">June 23, 2020</span></span>

<span data-ttu-id="beb0e-188">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-188">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-189">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-189">ACR</span></span>

* <span data-ttu-id="beb0e-190">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="beb0e-190">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="beb0e-191">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="beb0e-191">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-192">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-192">ACS</span></span>

* <span data-ttu-id="beb0e-193">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="beb0e-193">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-194">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-194">AKS</span></span>

* <span data-ttu-id="beb0e-195">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="beb0e-195">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="beb0e-196">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="beb0e-196">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="beb0e-197">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="beb0e-197">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="beb0e-198">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="beb0e-198">Fix typo in az aks update command</span></span>
* <span data-ttu-id="beb0e-199">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="beb0e-199">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="beb0e-200">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-200">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-201">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-201">AMS</span></span>

* <span data-ttu-id="beb0e-202">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="beb0e-202">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-203">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-203">AppService</span></span>

* <span data-ttu-id="beb0e-204">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="beb0e-204">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="beb0e-205">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="beb0e-205">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="beb0e-206">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-206">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="beb0e-207">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="beb0e-207">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="beb0e-208">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="beb0e-208">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="beb0e-209">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="beb0e-209">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="beb0e-210">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-210">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="beb0e-211">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="beb0e-211">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="beb0e-212">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-212">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="beb0e-213">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="beb0e-213">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="beb0e-214">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="beb0e-214">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-215">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-215">ARM</span></span>

* <span data-ttu-id="beb0e-216">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="beb0e-216">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="beb0e-217">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="beb0e-217">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="beb0e-218">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="beb0e-218">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="beb0e-219">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="beb0e-219">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="beb0e-220">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="beb0e-220">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="beb0e-221">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="beb0e-221">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="beb0e-222">ARO</span><span class="sxs-lookup"><span data-stu-id="beb0e-222">ARO</span></span>

* <span data-ttu-id="beb0e-223">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="beb0e-223">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-224">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-224">Batch</span></span>

* <span data-ttu-id="beb0e-225">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="beb0e-225">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="beb0e-226">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="beb0e-226">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="beb0e-227">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="beb0e-227">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="beb0e-228">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-228">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="beb0e-229">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="beb0e-229">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="beb0e-230">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="beb0e-230">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="beb0e-231">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="beb0e-231">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="beb0e-232">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="beb0e-232">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-233">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-233">CDN</span></span>

* <span data-ttu-id="beb0e-234">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="beb0e-234">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="beb0e-235">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="beb0e-235">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="beb0e-236">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-236">Cognitive Services</span></span>

* <span data-ttu-id="beb0e-237">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-237">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="beb0e-238">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-238">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-239">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-239">Compute</span></span>

* <span data-ttu-id="beb0e-240">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="beb0e-240">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="beb0e-241">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-241">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="beb0e-242">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-242">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="beb0e-243">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="beb0e-243">New command `az image builder cancel`</span></span>
* <span data-ttu-id="beb0e-244">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="beb0e-244">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-245">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-245">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-246">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-246">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="beb0e-247">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="beb0e-247">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="beb0e-248">EventHub</span><span class="sxs-lookup"><span data-stu-id="beb0e-248">EventHub</span></span>

* <span data-ttu-id="beb0e-249">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="beb0e-249">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-250">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-250">Extension</span></span>

* <span data-ttu-id="beb0e-251">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="beb0e-251">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="beb0e-252">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="beb0e-252">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="beb0e-253">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-253">Iot Hub</span></span>

* <span data-ttu-id="beb0e-254">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-254">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-255">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-255">KeyVault</span></span>

* <span data-ttu-id="beb0e-256">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="beb0e-256">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="beb0e-257">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-257">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-258">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-258">Monitor</span></span>

* <span data-ttu-id="beb0e-259">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-259">Support no wait for cluster creation</span></span>
* <span data-ttu-id="beb0e-260">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="beb0e-260">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-261">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-261">Network</span></span>

* <span data-ttu-id="beb0e-262">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-262">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="beb0e-263">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="beb0e-263">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="beb0e-264">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="beb0e-264">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="beb0e-265">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="beb0e-265">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-266">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-266">RBAC</span></span>

* <span data-ttu-id="beb0e-267">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="beb0e-267">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="beb0e-268">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="beb0e-268">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="beb0e-269">Segurança</span><span class="sxs-lookup"><span data-stu-id="beb0e-269">Security</span></span>

* <span data-ttu-id="beb0e-270">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="beb0e-270">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-271">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-271">SQL</span></span>

* <span data-ttu-id="beb0e-272">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="beb0e-272">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-273">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-273">Storage</span></span>

* <span data-ttu-id="beb0e-274">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="beb0e-274">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="beb0e-275">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="beb0e-275">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="beb0e-276">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="beb0e-276">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="beb0e-277">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="beb0e-277">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="beb0e-278">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="beb0e-278">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="beb0e-279">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="beb0e-279">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="beb0e-280">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="beb0e-280">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="beb0e-281">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="beb0e-281">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="beb0e-282">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="beb0e-282">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="beb0e-283">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="beb0e-283">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="beb0e-284">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-284">June 02, 2020</span></span>

<span data-ttu-id="beb0e-285">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-285">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-286">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-286">ACR</span></span>

* <span data-ttu-id="beb0e-287">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="beb0e-287">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-288">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-288">AKS</span></span>

* <span data-ttu-id="beb0e-289">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="beb0e-289">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="beb0e-290">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="beb0e-290">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-291">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-291">AppService</span></span>

* <span data-ttu-id="beb0e-292">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-292">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-293">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-293">ARM</span></span>

* <span data-ttu-id="beb0e-294">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="beb0e-294">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="beb0e-295">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="beb0e-295">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="beb0e-296">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-296">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="beb0e-297">ARO</span><span class="sxs-lookup"><span data-stu-id="beb0e-297">ARO</span></span>

* <span data-ttu-id="beb0e-298">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="beb0e-298">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="beb0e-299">EventHub</span><span class="sxs-lookup"><span data-stu-id="beb0e-299">EventHub</span></span>

* <span data-ttu-id="beb0e-300">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="beb0e-300">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-301">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-301">HDInsight</span></span>

* <span data-ttu-id="beb0e-302">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="beb0e-302">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-303">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-303">Monitor</span></span>

* <span data-ttu-id="beb0e-304">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-304">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="beb0e-305">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="beb0e-305">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="beb0e-306">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="beb0e-306">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-307">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-307">Network</span></span>

* <span data-ttu-id="beb0e-308">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="beb0e-308">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="beb0e-309">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="beb0e-309">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="beb0e-310">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-310">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="beb0e-311">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-311">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="beb0e-312">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-312">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-313">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-313">Packaging</span></span>

* <span data-ttu-id="beb0e-314">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="beb0e-314">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-315">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-315">RBAC</span></span>

* <span data-ttu-id="beb0e-316">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="beb0e-316">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-317">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-317">Redis</span></span>

* <span data-ttu-id="beb0e-318">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="beb0e-318">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-319">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-319">Storage</span></span>

* <span data-ttu-id="beb0e-320">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="beb0e-320">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="beb0e-321">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-321">Enable local context for storage account</span></span>
* <span data-ttu-id="beb0e-322">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-322">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="beb0e-323">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-323">May 19, 2020</span></span>

<span data-ttu-id="beb0e-324">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-324">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-325">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-325">ACR</span></span>

* <span data-ttu-id="beb0e-326">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-326">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="beb0e-327">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="beb0e-327">Support disable public network access</span></span>
* <span data-ttu-id="beb0e-328">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="beb0e-328">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="beb0e-329">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="beb0e-329">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-330">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-330">ACS</span></span>

* <span data-ttu-id="beb0e-331">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="beb0e-331">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-332">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-332">AKS</span></span>

* <span data-ttu-id="beb0e-333">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="beb0e-333">Update uptime-sla command help context</span></span>
* <span data-ttu-id="beb0e-334">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="beb0e-334">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="beb0e-335">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-335">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-336">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-336">AMS</span></span>

* <span data-ttu-id="beb0e-337">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="beb0e-337">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="beb0e-338">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="beb0e-338">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-339">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-339">AppConfig</span></span>

* <span data-ttu-id="beb0e-340">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="beb0e-340">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-341">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-341">AppService</span></span>

* <span data-ttu-id="beb0e-342">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="beb0e-342">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="beb0e-343">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="beb0e-343">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="beb0e-344">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-344">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="beb0e-345">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-345">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-346">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-346">ARM</span></span>

* <span data-ttu-id="beb0e-347">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="beb0e-347">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="beb0e-348">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="beb0e-348">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="beb0e-349">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-349">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="beb0e-350">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="beb0e-350">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="beb0e-351">ARO</span><span class="sxs-lookup"><span data-stu-id="beb0e-351">ARO</span></span>

* <span data-ttu-id="beb0e-352">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="beb0e-352">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="beb0e-353">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="beb0e-353">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-354">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-354">Backup</span></span>

* <span data-ttu-id="beb0e-355">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="beb0e-355">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="beb0e-356">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="beb0e-356">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="beb0e-357">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="beb0e-357">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="beb0e-358">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="beb0e-358">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="beb0e-359">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-359">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="beb0e-360">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-360">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="beb0e-361">CI</span><span class="sxs-lookup"><span data-stu-id="beb0e-361">CI</span></span>

* <span data-ttu-id="beb0e-362">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-362">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-363">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-363">Compute</span></span>

* <span data-ttu-id="beb0e-364">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="beb0e-364">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="beb0e-365">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="beb0e-365">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-366">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-366">Core</span></span>

* <span data-ttu-id="beb0e-367">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="beb0e-367">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-368">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-368">Extension</span></span>

* <span data-ttu-id="beb0e-369">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="beb0e-369">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="beb0e-370">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="beb0e-370">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-371">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-371">IoT</span></span>

* <span data-ttu-id="beb0e-372">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-372">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="beb0e-373">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-373">IoT Hub</span></span>

* <span data-ttu-id="beb0e-374">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-374">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="beb0e-375">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="beb0e-375">NetAppFiles</span></span>

* <span data-ttu-id="beb0e-376">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="beb0e-376">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-377">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-377">Network</span></span>

* <span data-ttu-id="beb0e-378">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="beb0e-378">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="beb0e-379">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="beb0e-379">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="beb0e-380">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-380">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="beb0e-381">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="beb0e-381">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="beb0e-382">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="beb0e-382">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="beb0e-383">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="beb0e-383">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="beb0e-384">Saída</span><span class="sxs-lookup"><span data-stu-id="beb0e-384">Output</span></span>

* <span data-ttu-id="beb0e-385">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="beb0e-385">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-386">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-386">Packaging</span></span>

* <span data-ttu-id="beb0e-387">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="beb0e-387">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-388">RBAC</span></span>

* <span data-ttu-id="beb0e-389">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="beb0e-389">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-390">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-390">Storage</span></span>

* <span data-ttu-id="beb0e-391">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-391">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="beb0e-392">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="beb0e-392">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="beb0e-393">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="beb0e-393">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="beb0e-394">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="beb0e-394">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="beb0e-395">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="beb0e-395">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="beb0e-396">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-396">April 30, 2020</span></span>

<span data-ttu-id="beb0e-397">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="beb0e-397">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-398">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-398">ACR</span></span>

* <span data-ttu-id="beb0e-399">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-399">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-400">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-400">Compute</span></span>

* <span data-ttu-id="beb0e-401">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="beb0e-401">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="beb0e-402">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-402">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="beb0e-403">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="beb0e-403">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-404">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-404">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-405">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="beb0e-405">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-406">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-406">Extension</span></span>

* <span data-ttu-id="beb0e-407">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="beb0e-407">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-408">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-408">Packaging</span></span>

* <span data-ttu-id="beb0e-409">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-409">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-410">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-410">SQL</span></span>

* <span data-ttu-id="beb0e-411">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="beb0e-411">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-412">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-412">Storage</span></span>

* <span data-ttu-id="beb0e-413">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-413">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="beb0e-414">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-414">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="beb0e-415">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="beb0e-415">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="beb0e-416">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="beb0e-416">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="beb0e-417">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-417">April 28, 2020</span></span>

<span data-ttu-id="beb0e-418">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-418">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-419">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-419">ACS</span></span>

* <span data-ttu-id="beb0e-420">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="beb0e-420">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="beb0e-421">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="beb0e-421">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="beb0e-422">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="beb0e-422">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="beb0e-423">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-423">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-424">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-424">AKS</span></span>

* <span data-ttu-id="beb0e-425">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-425">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-426">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-426">AppService</span></span>

* <span data-ttu-id="beb0e-427">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="beb0e-427">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-428">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-428">ARM</span></span>

* <span data-ttu-id="beb0e-429">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="beb0e-429">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="beb0e-430">ARO</span><span class="sxs-lookup"><span data-stu-id="beb0e-430">ARO</span></span>

* <span data-ttu-id="beb0e-431">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-431">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="beb0e-432">CI</span><span class="sxs-lookup"><span data-stu-id="beb0e-432">CI</span></span>

* <span data-ttu-id="beb0e-433">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="beb0e-433">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-434">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-434">Compute</span></span>

* <span data-ttu-id="beb0e-435">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-435">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="beb0e-436">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-436">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="beb0e-437">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-437">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-438">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-438">KeyVault</span></span>

* <span data-ttu-id="beb0e-439">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-439">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-440">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-440">Monitor</span></span>

* <span data-ttu-id="beb0e-441">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="beb0e-441">Support LA cluster CMK features</span></span>
* <span data-ttu-id="beb0e-442">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="beb0e-442">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-443">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-443">Network</span></span>

* <span data-ttu-id="beb0e-444">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="beb0e-444">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="beb0e-445">Privatedns</span><span class="sxs-lookup"><span data-stu-id="beb0e-445">Privatedns</span></span>

* <span data-ttu-id="beb0e-446">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="beb0e-446">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="beb0e-447">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-447">April 21, 2020</span></span>

<span data-ttu-id="beb0e-448">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-448">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-449">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-449">ACR</span></span>

* <span data-ttu-id="beb0e-450">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-450">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="beb0e-451">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="beb0e-451">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-452">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-452">AKS</span></span>

* <span data-ttu-id="beb0e-453">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="beb0e-453">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="beb0e-454">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="beb0e-454">Add --uptime-sla</span></span>
* <span data-ttu-id="beb0e-455">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="beb0e-455">Update containerservice package</span></span>
* <span data-ttu-id="beb0e-456">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="beb0e-456">Add node public IP support</span></span>
* <span data-ttu-id="beb0e-457">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-457">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-458">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-458">AppConfig</span></span>

* <span data-ttu-id="beb0e-459">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="beb0e-459">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="beb0e-460">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="beb0e-460">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-461">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-461">AppService</span></span>

* <span data-ttu-id="beb0e-462">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="beb0e-462">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="beb0e-463">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-463">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="beb0e-464">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="beb0e-464">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="beb0e-465">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="beb0e-465">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="beb0e-466">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="beb0e-466">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-467">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-467">ARM</span></span>

* <span data-ttu-id="beb0e-468">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="beb0e-468">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="beb0e-469">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-469">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="beb0e-470">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="beb0e-470">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="beb0e-471">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="beb0e-471">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="beb0e-472">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="beb0e-472">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="beb0e-473">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="beb0e-473">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="beb0e-474">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="beb0e-474">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="beb0e-475">ARO</span><span class="sxs-lookup"><span data-stu-id="beb0e-475">ARO</span></span>

* <span data-ttu-id="beb0e-476">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="beb0e-476">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-477">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-477">Batch</span></span>

* <span data-ttu-id="beb0e-478">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-478">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-479">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-479">Compute</span></span>

* <span data-ttu-id="beb0e-480">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="beb0e-480">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="beb0e-481">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="beb0e-481">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="beb0e-482">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="beb0e-482">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="beb0e-483">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-483">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="beb0e-484">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="beb0e-484">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="beb0e-485">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="beb0e-485">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-486">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-486">CosmosDB</span></span>

* <span data-ttu-id="beb0e-487">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="beb0e-487">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="beb0e-488">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-488">IoT Central</span></span>

* <span data-ttu-id="beb0e-489">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="beb0e-489">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="beb0e-490">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="beb0e-490">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-491">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-491">Monitor</span></span>

* <span data-ttu-id="beb0e-492">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-492">Support private link scenario for monitor</span></span>
* <span data-ttu-id="beb0e-493">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="beb0e-493">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-494">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-494">Network</span></span>

* <span data-ttu-id="beb0e-495">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="beb0e-495">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="beb0e-496">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="beb0e-496">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="beb0e-497">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-497">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="beb0e-498">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="beb0e-498">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-499">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-499">Packaging</span></span>

* <span data-ttu-id="beb0e-500">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="beb0e-500">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-501">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-501">RBAC</span></span>

* <span data-ttu-id="beb0e-502">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="beb0e-502">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-503">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-503">RDBMS</span></span>

* <span data-ttu-id="beb0e-504">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-504">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="beb0e-505">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-505">Service Fabric</span></span>

* <span data-ttu-id="beb0e-506">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="beb0e-506">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="beb0e-507">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="beb0e-507">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-508">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-508">SQL</span></span>

* <span data-ttu-id="beb0e-509">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="beb0e-509">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="beb0e-510">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="beb0e-510">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-511">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-511">Storage</span></span>

* <span data-ttu-id="beb0e-512">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-512">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="beb0e-513">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-513">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="beb0e-514">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="beb0e-514">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="beb0e-515">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="beb0e-515">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="beb0e-516">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-516">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="beb0e-517">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="beb0e-517">Survey</span></span>

* <span data-ttu-id="beb0e-518">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="beb0e-518">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="beb0e-519">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-519">April 01, 2020</span></span>

<span data-ttu-id="beb0e-520">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="beb0e-520">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-521">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-521">ACR</span></span>

* <span data-ttu-id="beb0e-522">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-522">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-523">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-523">Profile</span></span>

* <span data-ttu-id="beb0e-524">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="beb0e-524">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="beb0e-525">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-525">March 31, 2020</span></span>

<span data-ttu-id="beb0e-526">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-526">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-527">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-527">ACR</span></span>

* <span data-ttu-id="beb0e-528">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="beb0e-528">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="beb0e-529">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="beb0e-529">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="beb0e-530">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="beb0e-530">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="beb0e-531">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="beb0e-531">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="beb0e-532">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-532">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="beb0e-533">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="beb0e-533">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="beb0e-534">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-534">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-535">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-535">AKS</span></span>

* <span data-ttu-id="beb0e-536">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="beb0e-536">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="beb0e-537">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-537">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="beb0e-538">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-538">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-539">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-539">AMS</span></span>

* <span data-ttu-id="beb0e-540">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="beb0e-540">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-541">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-541">AppConfig</span></span>

* <span data-ttu-id="beb0e-542">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="beb0e-542">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-543">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-543">AppService</span></span>

* <span data-ttu-id="beb0e-544">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-544">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="beb0e-545">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="beb0e-545">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="beb0e-546">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-546">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-547">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-547">ARM</span></span>

* <span data-ttu-id="beb0e-548">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-548">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="beb0e-549">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-549">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="beb0e-550">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="beb0e-550">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="beb0e-551">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="beb0e-551">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-552">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-552">Backup</span></span>

* <span data-ttu-id="beb0e-553">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="beb0e-553">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="beb0e-554">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="beb0e-554">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="beb0e-555">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="beb0e-555">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-556">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-556">Compute</span></span>

* <span data-ttu-id="beb0e-557">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="beb0e-557">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="beb0e-558">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="beb0e-558">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="beb0e-559">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="beb0e-559">az vm update: Support --workspace</span></span>
* <span data-ttu-id="beb0e-560">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="beb0e-560">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="beb0e-561">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="beb0e-561">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="beb0e-562">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="beb0e-562">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="beb0e-563">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-563">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="beb0e-564">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="beb0e-564">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-565">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-565">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-566">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="beb0e-566">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="beb0e-567">Docker</span><span class="sxs-lookup"><span data-stu-id="beb0e-567">Docker</span></span>

* <span data-ttu-id="beb0e-568">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="beb0e-568">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-569">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-569">Extension</span></span>

* <span data-ttu-id="beb0e-570">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="beb0e-570">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-571">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-571">HDInsight</span></span>

* <span data-ttu-id="beb0e-572">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-572">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="beb0e-573">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="beb0e-573">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-574">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-574">IoT</span></span>

* <span data-ttu-id="beb0e-575">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="beb0e-575">Add codeowner</span></span>
* <span data-ttu-id="beb0e-576">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="beb0e-576">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="beb0e-577">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-577">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="beb0e-578">IoT Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-578">IoTCentral</span></span>

* <span data-ttu-id="beb0e-579">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="beb0e-579">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-580">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-580">KeyVault</span></span>

* <span data-ttu-id="beb0e-581">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-581">Support certificate backup/restore</span></span>
* <span data-ttu-id="beb0e-582">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="beb0e-582">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="beb0e-583">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-583">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="beb0e-584">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="beb0e-584">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="beb0e-585">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="beb0e-585">Lock</span></span>

* <span data-ttu-id="beb0e-586">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-586">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-587">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-587">Monitor</span></span>

* <span data-ttu-id="beb0e-588">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="beb0e-588">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="beb0e-589">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="beb0e-589">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="beb0e-590">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="beb0e-590">NetAppFiles</span></span>

* <span data-ttu-id="beb0e-591">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="beb0e-591">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-592">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-592">Network</span></span>

* <span data-ttu-id="beb0e-593">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="beb0e-593">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="beb0e-594">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="beb0e-594">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="beb0e-595">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-595">support host names in application gateway listener</span></span>
* <span data-ttu-id="beb0e-596">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="beb0e-596">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="beb0e-597">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="beb0e-597">Support vpn gateway generation</span></span>
* <span data-ttu-id="beb0e-598">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="beb0e-598">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-599">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-599">Packaging</span></span>

* <span data-ttu-id="beb0e-600">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="beb0e-600">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-601">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-601">Profile</span></span>

* <span data-ttu-id="beb0e-602">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="beb0e-602">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-603">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-603">RDBMS</span></span>

* <span data-ttu-id="beb0e-604">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-604">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="beb0e-605">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-605">March 10, 2020</span></span>

<span data-ttu-id="beb0e-606">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-606">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-607">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-607">ACR</span></span>

* <span data-ttu-id="beb0e-608">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-608">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="beb0e-609">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="beb0e-609">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="beb0e-610">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="beb0e-610">Add private link and CMK support</span></span>
* <span data-ttu-id="beb0e-611">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="beb0e-611">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-612">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-612">AKS</span></span>

* <span data-ttu-id="beb0e-613">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="beb0e-613">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="beb0e-614">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="beb0e-614">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="beb0e-615">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-615">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="beb0e-616">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-616">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="beb0e-617">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="beb0e-617">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="beb0e-618">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-618">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="beb0e-619">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-619">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="beb0e-620">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="beb0e-620">add missing / in the dashboard url</span></span>
* <span data-ttu-id="beb0e-621">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="beb0e-621">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="beb0e-622">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="beb0e-622">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="beb0e-623">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="beb0e-623">az aks: Add aad session key support</span></span>
* <span data-ttu-id="beb0e-624">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="beb0e-624">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="beb0e-625">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="beb0e-625">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-626">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-626">AppConfig</span></span>

* <span data-ttu-id="beb0e-627">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="beb0e-627">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-628">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-628">AppService</span></span>

* <span data-ttu-id="beb0e-629">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="beb0e-629">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="beb0e-630">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="beb0e-630">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="beb0e-631">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="beb0e-631">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="beb0e-632">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-632">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="beb0e-633">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-633">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="beb0e-634">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="beb0e-634">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-635">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-635">ARM</span></span>

* <span data-ttu-id="beb0e-636">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-636">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="beb0e-637">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-637">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="beb0e-638">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-638">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="beb0e-639">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="beb0e-639">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="beb0e-640">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="beb0e-640">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="beb0e-641">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="beb0e-641">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="beb0e-642">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-642">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="beb0e-643">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="beb0e-643">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="beb0e-644">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="beb0e-644">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="beb0e-645">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="beb0e-645">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-646">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-646">CDN</span></span>

* <span data-ttu-id="beb0e-647">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-647">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-648">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-648">Compute</span></span>

* <span data-ttu-id="beb0e-649">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="beb0e-649">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="beb0e-650">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-650">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="beb0e-651">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="beb0e-651">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="beb0e-652">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="beb0e-652">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="beb0e-653">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="beb0e-653">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-654">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-654">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-655">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="beb0e-655">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="beb0e-656">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="beb0e-656">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-657">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-657">KeyVault</span></span>

* <span data-ttu-id="beb0e-658">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-658">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-659">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-659">Monitor</span></span>

* <span data-ttu-id="beb0e-660">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="beb0e-660">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-661">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-661">Network</span></span>

* <span data-ttu-id="beb0e-662">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="beb0e-662">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="beb0e-663">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="beb0e-663">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="beb0e-664">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-664">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="beb0e-665">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="beb0e-665">az network bastion: support bastion</span></span>
* <span data-ttu-id="beb0e-666">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="beb0e-666">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="beb0e-667">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-667">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="beb0e-668">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-668">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="beb0e-669">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="beb0e-669">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="beb0e-670">Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-670">Policy</span></span>

* <span data-ttu-id="beb0e-671">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="beb0e-671">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-672">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-672">RBAC</span></span>

* <span data-ttu-id="beb0e-673">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="beb0e-673">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-674">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-674">RDBMS</span></span>

* <span data-ttu-id="beb0e-675">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-675">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="beb0e-676">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="beb0e-676">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="beb0e-677">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="beb0e-677">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="beb0e-678">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-678">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="beb0e-679">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-679">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="beb0e-680">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-680">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="beb0e-681">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-681">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="beb0e-682">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-682">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-683">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-683">SQL</span></span>

* <span data-ttu-id="beb0e-684">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="beb0e-684">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="beb0e-685">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="beb0e-685">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="beb0e-686">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="beb0e-686">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="beb0e-687">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-687">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-688">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-688">Storage</span></span>

* <span data-ttu-id="beb0e-689">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="beb0e-689">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="beb0e-690">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="beb0e-690">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="beb0e-691">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-691">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="beb0e-692">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-692">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="beb0e-693">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="beb0e-693">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="beb0e-694">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-694">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="beb0e-695">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-695">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="beb0e-696">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="beb0e-696">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="beb0e-697">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="beb0e-697">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="beb0e-698">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-698">February 18, 2020</span></span>

<span data-ttu-id="beb0e-699">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-699">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-700">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-700">ACR</span></span>

* <span data-ttu-id="beb0e-701">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-701">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="beb0e-702">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="beb0e-702">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="beb0e-703">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="beb0e-703">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-704">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-704">ACS</span></span>

* <span data-ttu-id="beb0e-705">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="beb0e-705">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="beb0e-706">Aladdin</span><span class="sxs-lookup"><span data-stu-id="beb0e-706">Aladdin</span></span>

* <span data-ttu-id="beb0e-707">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-707">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-708">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-708">AMS</span></span>

* <span data-ttu-id="beb0e-709">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="beb0e-709">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-710">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-710">AppConfig</span></span>

* <span data-ttu-id="beb0e-711">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="beb0e-711">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="beb0e-712">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="beb0e-712">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="beb0e-713">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="beb0e-713">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-714">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-714">AppService</span></span>

* <span data-ttu-id="beb0e-715">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="beb0e-715">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="beb0e-716">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="beb0e-716">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="beb0e-717">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="beb0e-717">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-718">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-718">ARM</span></span>

* <span data-ttu-id="beb0e-719">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="beb0e-719">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="beb0e-720">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="beb0e-720">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-721">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-721">Backup</span></span>

* <span data-ttu-id="beb0e-722">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="beb0e-722">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="beb0e-723">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="beb0e-723">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-724">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-724">Compute</span></span>

* <span data-ttu-id="beb0e-725">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="beb0e-725">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="beb0e-726">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="beb0e-726">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="beb0e-727">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="beb0e-727">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="beb0e-728">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-728">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="beb0e-729">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-729">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="beb0e-730">Eventhub</span><span class="sxs-lookup"><span data-stu-id="beb0e-730">Eventhub</span></span>

* <span data-ttu-id="beb0e-731">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-731">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-732">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-732">KeyVault</span></span>

* <span data-ttu-id="beb0e-733">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="beb0e-733">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="beb0e-734">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="beb0e-734">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="beb0e-735">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-735">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-736">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-736">Network</span></span>

* <span data-ttu-id="beb0e-737">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-737">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="beb0e-738">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="beb0e-738">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="beb0e-739">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="beb0e-739">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-740">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-740">Packaging</span></span>

* <span data-ttu-id="beb0e-741">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="beb0e-741">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-742">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-742">Profile</span></span>

* <span data-ttu-id="beb0e-743">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="beb0e-743">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="beb0e-744">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="beb0e-744">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="beb0e-745">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="beb0e-745">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="beb0e-746">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-746">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-747">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-747">Role</span></span>

* <span data-ttu-id="beb0e-748">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="beb0e-748">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-749">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-749">SQL</span></span>

* <span data-ttu-id="beb0e-750">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="beb0e-750">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-751">Storage</span></span>

* <span data-ttu-id="beb0e-752">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="beb0e-752">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="beb0e-753">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-753">February 04, 2020</span></span>

<span data-ttu-id="beb0e-754">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="beb0e-754">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-755">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-755">ACS</span></span>

* <span data-ttu-id="beb0e-756">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="beb0e-756">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="beb0e-757">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-757">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-758">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-758">ACR</span></span>

* <span data-ttu-id="beb0e-759">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="beb0e-759">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="beb0e-760">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="beb0e-760">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="beb0e-761">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="beb0e-761">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-762">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-762">AKS</span></span>

* <span data-ttu-id="beb0e-763">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-763">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-764">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-764">AppConfig</span></span>

* <span data-ttu-id="beb0e-765">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="beb0e-765">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="beb0e-766">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-766">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="beb0e-767">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="beb0e-767">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="beb0e-768">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="beb0e-768">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="beb0e-769">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="beb0e-769">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-770">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-770">AppService</span></span>

* <span data-ttu-id="beb0e-771">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-771">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="beb0e-772">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-772">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-773">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-773">ARM</span></span>

* <span data-ttu-id="beb0e-774">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-774">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="beb0e-775">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="beb0e-775">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="beb0e-776">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="beb0e-776">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="beb0e-777">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-777">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="beb0e-778">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-778">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="beb0e-779">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-779">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="beb0e-780">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-780">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-781">BotService</span><span class="sxs-lookup"><span data-stu-id="beb0e-781">BotService</span></span>

* <span data-ttu-id="beb0e-782">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="beb0e-782">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="beb0e-783">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="beb0e-783">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-784">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-784">CDN</span></span>

* <span data-ttu-id="beb0e-785">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="beb0e-785">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="beb0e-786">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="beb0e-786">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="beb0e-787">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="beb0e-787">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="beb0e-788">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-788">Deployment Manager</span></span>

* <span data-ttu-id="beb0e-789">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-789">Add list operation for all resources.</span></span>
* <span data-ttu-id="beb0e-790">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="beb0e-790">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="beb0e-791">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="beb0e-791">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-792">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-792">IoT</span></span>

* <span data-ttu-id="beb0e-793">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="beb0e-793">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="beb0e-794">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-794">IoT Central</span></span>

* <span data-ttu-id="beb0e-795">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="beb0e-795">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-796">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-796">Key Vault</span></span>

* <span data-ttu-id="beb0e-797">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="beb0e-797">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="beb0e-798">Diversos</span><span class="sxs-lookup"><span data-stu-id="beb0e-798">Misc</span></span>

* <span data-ttu-id="beb0e-799">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="beb0e-799">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-800">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-800">Network</span></span>

* <span data-ttu-id="beb0e-801">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-801">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="beb0e-802">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="beb0e-802">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="beb0e-803">Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-803">Policy</span></span>

* <span data-ttu-id="beb0e-804">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="beb0e-804">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="beb0e-805">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="beb0e-805">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-806">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-806">Profile</span></span>

* <span data-ttu-id="beb0e-807">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-807">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-808">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-808">RBAC</span></span>

* <span data-ttu-id="beb0e-809">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-809">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="beb0e-810">Segurança</span><span class="sxs-lookup"><span data-stu-id="beb0e-810">Security</span></span>

* <span data-ttu-id="beb0e-811">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-811">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-812">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-812">SQL</span></span>

* <span data-ttu-id="beb0e-813">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-813">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="beb0e-814">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="beb0e-814">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="beb0e-815">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="beb0e-815">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="beb0e-816">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="beb0e-816">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="beb0e-817">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="beb0e-817">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="beb0e-818">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="beb0e-818">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-819">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-819">Storage</span></span>

* <span data-ttu-id="beb0e-820">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="beb0e-820">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="beb0e-821">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-821">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="beb0e-822">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="beb0e-822">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="beb0e-823">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="beb0e-823">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="beb0e-824">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="beb0e-824">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="beb0e-825">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="beb0e-825">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="beb0e-826">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-826">ServiceFabric</span></span>

* <span data-ttu-id="beb0e-827">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="beb0e-827">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="beb0e-828">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-828">January 13, 2020</span></span>

<span data-ttu-id="beb0e-829">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="beb0e-829">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-830">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-830">Compute</span></span>

* <span data-ttu-id="beb0e-831">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="beb0e-831">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="beb0e-832">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="beb0e-832">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-833">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-833">Storage</span></span>

* <span data-ttu-id="beb0e-834">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-834">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="beb0e-835">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="beb0e-835">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="beb0e-836">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-836">January 07, 2020</span></span>

<span data-ttu-id="beb0e-837">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="beb0e-837">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-838">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-838">ACR</span></span>

* <span data-ttu-id="beb0e-839">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-839">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="beb0e-840">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-840">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-841">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-841">AppConfig</span></span>

* <span data-ttu-id="beb0e-842">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-842">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="beb0e-843">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-843">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="beb0e-844">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="beb0e-844">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-845">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-845">AppService</span></span>

* <span data-ttu-id="beb0e-846">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="beb0e-846">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="beb0e-847">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="beb0e-847">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="beb0e-848">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="beb0e-848">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-849">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-849">ARM</span></span>

* <span data-ttu-id="beb0e-850">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-850">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-851">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-851">Backup</span></span>

* <span data-ttu-id="beb0e-852">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="beb0e-852">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="beb0e-853">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-853">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="beb0e-854">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="beb0e-854">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-855">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-855">Compute</span></span>

* <span data-ttu-id="beb0e-856">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="beb0e-856">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="beb0e-857">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="beb0e-857">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="beb0e-858">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="beb0e-858">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-859">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-859">HDInsight</span></span>

* <span data-ttu-id="beb0e-860">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="beb0e-860">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="beb0e-861">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-861">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="beb0e-862">Diversos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-862">Misc.</span></span>

* <span data-ttu-id="beb0e-863">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="beb0e-863">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="beb0e-864">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-864">Event Hubs</span></span>

* <span data-ttu-id="beb0e-865">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-865">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="beb0e-866">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-866">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="beb0e-867">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-867">Service Bus</span></span>

* <span data-ttu-id="beb0e-868">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-868">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="beb0e-869">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="beb0e-869">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-870">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-870">RBAC</span></span>

* <span data-ttu-id="beb0e-871">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="beb0e-871">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-872">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-872">Storage</span></span>

* <span data-ttu-id="beb0e-873">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="beb0e-873">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="beb0e-874">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-874">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="beb0e-875">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="beb0e-875">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="beb0e-876">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-876">December 17, 2019</span></span>

<span data-ttu-id="beb0e-877">2.0.78</span><span class="sxs-lookup"><span data-stu-id="beb0e-877">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-878">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-878">ACR</span></span>

* <span data-ttu-id="beb0e-879">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="beb0e-879">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-880">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-880">ACS</span></span>

* <span data-ttu-id="beb0e-881">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-881">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-882">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-882">AMS</span></span>

* <span data-ttu-id="beb0e-883">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="beb0e-883">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-884">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-884">AppConfig</span></span>

* <span data-ttu-id="beb0e-885">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="beb0e-885">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="beb0e-886">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="beb0e-886">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="beb0e-887">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="beb0e-887">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-888">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-888">AppService</span></span>

* <span data-ttu-id="beb0e-889">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="beb0e-889">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="beb0e-890">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="beb0e-890">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="beb0e-891">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-891">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="beb0e-892">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-892">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-893">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-893">ARM</span></span>

* <span data-ttu-id="beb0e-894">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-894">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="beb0e-895">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="beb0e-895">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="beb0e-896">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-896">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-897">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-897">Backup</span></span>

* <span data-ttu-id="beb0e-898">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="beb0e-898">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-899">BotService</span><span class="sxs-lookup"><span data-stu-id="beb0e-899">BotService</span></span>

* <span data-ttu-id="beb0e-900">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-900">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="beb0e-901">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="beb0e-901">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="beb0e-902">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-902">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="beb0e-903">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-903">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="beb0e-904">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-904">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="beb0e-905">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-905">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="beb0e-906">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-906">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="beb0e-907">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-907">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="beb0e-908">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="beb0e-908">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-909">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-909">Compute</span></span>

* <span data-ttu-id="beb0e-910">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-910">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="beb0e-911">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-911">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="beb0e-912">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-912">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="beb0e-913">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="beb0e-913">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="beb0e-914">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="beb0e-914">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="beb0e-915">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="beb0e-915">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-916">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-916">Core</span></span>

* <span data-ttu-id="beb0e-917">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-917">Removed support for Python 3.4</span></span>
* <span data-ttu-id="beb0e-918">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-918">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="beb0e-919">DLS</span><span class="sxs-lookup"><span data-stu-id="beb0e-919">DLS</span></span>

* <span data-ttu-id="beb0e-920">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="beb0e-920">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="beb0e-921">Instalar</span><span class="sxs-lookup"><span data-stu-id="beb0e-921">Install</span></span>

* <span data-ttu-id="beb0e-922">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="beb0e-922">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-923">IOT</span><span class="sxs-lookup"><span data-stu-id="beb0e-923">IOT</span></span>

* <span data-ttu-id="beb0e-924">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="beb0e-924">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="beb0e-925">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="beb0e-925">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-926">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-926">Key Vault</span></span>

* <span data-ttu-id="beb0e-927">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-927">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="beb0e-928">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="beb0e-928">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="beb0e-929">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="beb0e-929">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="beb0e-930">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="beb0e-930">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="beb0e-931">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="beb0e-931">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-932">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-932">Network</span></span>

* <span data-ttu-id="beb0e-933">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-933">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="beb0e-934">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-934">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="beb0e-935">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-935">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="beb0e-936">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-936">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="beb0e-937">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="beb0e-937">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-938">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-938">Packaging</span></span>

* <span data-ttu-id="beb0e-939">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="beb0e-939">Added back edge builds for pip install</span></span>
* <span data-ttu-id="beb0e-940">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-940">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="beb0e-941">Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-941">Policy</span></span>

* <span data-ttu-id="beb0e-942">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="beb0e-942">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="beb0e-943">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="beb0e-943">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-944">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-944">Redis</span></span>

* <span data-ttu-id="beb0e-945">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-945">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="beb0e-946">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="beb0e-946">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="beb0e-947">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-947">ServiceFabric</span></span>

* <span data-ttu-id="beb0e-948">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-948">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="beb0e-949">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="beb0e-949">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-950">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-950">SQL</span></span>

* <span data-ttu-id="beb0e-951">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="beb0e-951">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-952">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-952">Storage</span></span>

* <span data-ttu-id="beb0e-953">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-953">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="beb0e-954">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="beb0e-954">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="beb0e-955">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-955">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="beb0e-956">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-956">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="beb0e-957">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="beb0e-957">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="beb0e-958">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-958">November 26, 2019</span></span>

<span data-ttu-id="beb0e-959">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="beb0e-959">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-960">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-960">ACR</span></span>

* <span data-ttu-id="beb0e-961">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-961">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="beb0e-962">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-962">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="beb0e-963">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-963">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="beb0e-964">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-964">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-965">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-965">AKS</span></span>

* <span data-ttu-id="beb0e-966">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="beb0e-966">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-967">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-967">AppConfig</span></span>

* <span data-ttu-id="beb0e-968">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-968">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="beb0e-969">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="beb0e-969">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="beb0e-970">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="beb0e-970">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="beb0e-971">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-971">AppService</span></span>

* <span data-ttu-id="beb0e-972">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-972">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="beb0e-973">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-973">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="beb0e-974">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="beb0e-974">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-975">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-975">Backup</span></span>

* <span data-ttu-id="beb0e-976">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="beb0e-976">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="beb0e-977">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-977">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-978">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-978">Compute</span></span>

* <span data-ttu-id="beb0e-979">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-979">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="beb0e-980">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="beb0e-980">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="beb0e-981">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="beb0e-981">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="beb0e-982">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="beb0e-982">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="beb0e-983">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-983">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="beb0e-984">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-984">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="beb0e-985">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-985">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="beb0e-986">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="beb0e-986">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="beb0e-987">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="beb0e-987">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="beb0e-988">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-988">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-989">IOT</span><span class="sxs-lookup"><span data-stu-id="beb0e-989">IOT</span></span>

* <span data-ttu-id="beb0e-990">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="beb0e-990">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="beb0e-991">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-991">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="beb0e-992">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-992">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-993">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-993">Key Vault</span></span>

* <span data-ttu-id="beb0e-994">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="beb0e-994">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="beb0e-995">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="beb0e-995">NetAppFiles</span></span>

* <span data-ttu-id="beb0e-996">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="beb0e-996">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-997">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-997">Network</span></span>

* <span data-ttu-id="beb0e-998">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-998">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="beb0e-999">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-999">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="beb0e-1000">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="beb0e-1000">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="beb0e-1001">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="beb0e-1001">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="beb0e-1002">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1002">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="beb0e-1003">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1003">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="beb0e-1004">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1004">Packaging</span></span>

* <span data-ttu-id="beb0e-1005">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="beb0e-1005">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="beb0e-1006">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="beb0e-1006">Added support for Python 3.8</span></span>
* <span data-ttu-id="beb0e-1007">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1007">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1008">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1008">Profile</span></span>

* <span data-ttu-id="beb0e-1009">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="beb0e-1009">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="beb0e-1010">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1010">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="beb0e-1011">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1011">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="beb0e-1012">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="beb0e-1012">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="beb0e-1013">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1013">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1014">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1014">RBAC</span></span>

* <span data-ttu-id="beb0e-1015">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1015">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-1016">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-1016">Redis</span></span>

* <span data-ttu-id="beb0e-1017">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="beb0e-1017">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="beb0e-1018">Reservas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1018">Reservations</span></span>

* <span data-ttu-id="beb0e-1019">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-1019">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="beb0e-1020">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="beb0e-1020">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="beb0e-1021">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="beb0e-1021">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="beb0e-1022">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="beb0e-1022">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="beb0e-1023">Rest</span><span class="sxs-lookup"><span data-stu-id="beb0e-1023">Rest</span></span>
* <span data-ttu-id="beb0e-1024">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="beb0e-1024">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1025">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1025">SQL</span></span>

* <span data-ttu-id="beb0e-1026">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1026">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1027">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1027">Storage</span></span>

* <span data-ttu-id="beb0e-1028">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1028">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="beb0e-1029">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1029">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="beb0e-1030">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="beb0e-1030">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="beb0e-1031">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1031">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="beb0e-1032">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1032">November 4, 2019</span></span>

<span data-ttu-id="beb0e-1033">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="beb0e-1033">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1034">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1034">ACR</span></span>

* <span data-ttu-id="beb0e-1035">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1035">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="beb0e-1036">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1036">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="beb0e-1037">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="beb0e-1037">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1038">AKS</span></span>

* <span data-ttu-id="beb0e-1039">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1039">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="beb0e-1040">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1040">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="beb0e-1041">AppConfig</span><span class="sxs-lookup"><span data-stu-id="beb0e-1041">AppConfig</span></span>

* <span data-ttu-id="beb0e-1042">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1042">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="beb0e-1043">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1043">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="beb0e-1044">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1044">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1045">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1045">AppService</span></span>

* <span data-ttu-id="beb0e-1046">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1046">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="beb0e-1047">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1047">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="beb0e-1048">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1048">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="beb0e-1049">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-1049">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="beb0e-1050">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1050">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-1051">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1051">ARM</span></span>

* <span data-ttu-id="beb0e-1052">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1052">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="beb0e-1053">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-1053">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-1054">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-1054">Backup</span></span>

* <span data-ttu-id="beb0e-1055">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-1055">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-1056">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1056">Compute</span></span>

* <span data-ttu-id="beb0e-1057">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1057">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="beb0e-1058">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1058">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="beb0e-1059">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1059">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="beb0e-1060">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1060">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="beb0e-1061">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1061">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="beb0e-1062">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1062">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="beb0e-1063">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1063">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="beb0e-1064">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="beb0e-1064">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-1065">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1065">CosmosDB</span></span>

* <span data-ttu-id="beb0e-1066">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="beb0e-1066">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="beb0e-1067">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="beb0e-1067">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="beb0e-1068">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1068">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="beb0e-1069">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1069">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="beb0e-1070">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1070">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="beb0e-1071">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1071">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="beb0e-1072">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-1072">Fixed typo in help message</span></span>
* <span data-ttu-id="beb0e-1073">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1073">database: Added deprecation information</span></span>
* <span data-ttu-id="beb0e-1074">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1074">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1075">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1075">IoT</span></span>

* <span data-ttu-id="beb0e-1076">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="beb0e-1076">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="beb0e-1077">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1077">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-1078">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1078">Key Vault</span></span>

* <span data-ttu-id="beb0e-1079">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="beb0e-1079">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="beb0e-1080">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-1080">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="beb0e-1081">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="beb0e-1081">NetAppFiles</span></span>

* <span data-ttu-id="beb0e-1082">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1082">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="beb0e-1083">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1083">This new API version includes:</span></span>

    - <span data-ttu-id="beb0e-1084">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="beb0e-1084">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="beb0e-1085">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="beb0e-1085">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="beb0e-1086">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1086">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="beb0e-1087">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="beb0e-1087">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1088">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1088">Network</span></span>

* <span data-ttu-id="beb0e-1089">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1089">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="beb0e-1090">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1090">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="beb0e-1091">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1091">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="beb0e-1092">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-1092">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="beb0e-1093">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="beb0e-1093">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="beb0e-1094">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1094">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1095">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1095">Profile</span></span>

* <span data-ttu-id="beb0e-1096">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-1096">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="beb0e-1097">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1097">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1098">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1098">RBAC</span></span>

* <span data-ttu-id="beb0e-1099">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-1099">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="beb0e-1100">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-1100">ServiceFabric</span></span>

* <span data-ttu-id="beb0e-1101">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1101">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1102">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1102">SQL</span></span>

* <span data-ttu-id="beb0e-1103">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1103">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1104">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1104">Storage</span></span>

* <span data-ttu-id="beb0e-1105">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-1105">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="beb0e-1106">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1106">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="beb0e-1107">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1107">October 15, 2019</span></span>

<span data-ttu-id="beb0e-1108">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="beb0e-1108">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-1109">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1109">AKS</span></span>

* <span data-ttu-id="beb0e-1110">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1110">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="beb0e-1111">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1111">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1112">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1112">AMS</span></span>

* <span data-ttu-id="beb0e-1113">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1113">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="beb0e-1114">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="beb0e-1114">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1115">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1115">AppService</span></span>

* <span data-ttu-id="beb0e-1116">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1116">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="beb0e-1117">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1117">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="beb0e-1118">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1118">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-1119">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1119">ARM</span></span>

* <span data-ttu-id="beb0e-1120">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="beb0e-1120">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-1121">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1121">Compute</span></span>

* <span data-ttu-id="beb0e-1122">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1122">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="beb0e-1123">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1123">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="beb0e-1124">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1124">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="beb0e-1125">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1125">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="beb0e-1126">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1126">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="beb0e-1127">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-1127">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1128">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1128">Core</span></span>

* <span data-ttu-id="beb0e-1129">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="beb0e-1129">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1130">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1130">IoT</span></span>

* <span data-ttu-id="beb0e-1131">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="beb0e-1131">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1132">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1132">Monitor</span></span>

* <span data-ttu-id="beb0e-1133">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1133">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1134">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1134">Network</span></span>

* <span data-ttu-id="beb0e-1135">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1135">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="beb0e-1136">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1136">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1137">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1137">SQL</span></span>

* <span data-ttu-id="beb0e-1138">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1138">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1139">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1139">Storage</span></span>

* <span data-ttu-id="beb0e-1140">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-1140">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="beb0e-1141">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1141">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="beb0e-1142">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1142">September 24, 2019</span></span>

<span data-ttu-id="beb0e-1143">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="beb0e-1143">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1144">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1144">ACR</span></span>

* <span data-ttu-id="beb0e-1145">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1145">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="beb0e-1146">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1146">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-1147">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1147">AKS</span></span>

* <span data-ttu-id="beb0e-1148">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1148">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="beb0e-1149">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1149">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="beb0e-1150">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1150">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-1151">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1151">ARM</span></span>

* <span data-ttu-id="beb0e-1152">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="beb0e-1152">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-1153">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1153">Compute</span></span>

* <span data-ttu-id="beb0e-1154">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1154">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="beb0e-1155">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1155">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="beb0e-1156">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1156">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="beb0e-1157">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="beb0e-1157">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="beb0e-1158">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1158">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-1159">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1159">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-1160">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1160">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="beb0e-1161">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1161">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="beb0e-1162">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1162">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="beb0e-1163">EventGrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-1163">EventGrid</span></span>

* <span data-ttu-id="beb0e-1164">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1164">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-1165">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1165">Key Vault</span></span>

* <span data-ttu-id="beb0e-1166">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1166">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1167">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1167">Monitor</span></span>

* <span data-ttu-id="beb0e-1168">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1168">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="beb0e-1169">Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-1169">Policy</span></span>

* <span data-ttu-id="beb0e-1170">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1170">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="beb0e-1171">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1171">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1172">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1172">Storage</span></span>

* <span data-ttu-id="beb0e-1173">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1173">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="beb0e-1174">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1174">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1175">ACR</span></span>

* <span data-ttu-id="beb0e-1176">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="beb0e-1176">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-1177">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1177">AKS</span></span>

* <span data-ttu-id="beb0e-1178">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1178">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="beb0e-1179">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1179">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="beb0e-1180">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1180">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-1181">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1181">ARM</span></span>

* <span data-ttu-id="beb0e-1182">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="beb0e-1182">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1183">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1183">Batch</span></span>

* <span data-ttu-id="beb0e-1184">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1184">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="beb0e-1185">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1185">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="beb0e-1186">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1186">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="beb0e-1187">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1187">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="beb0e-1188">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1188">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="beb0e-1189">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1189">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="beb0e-1190">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1190">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1191">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1191">HDInsight</span></span>

* <span data-ttu-id="beb0e-1192">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="beb0e-1192">GA release</span></span>
* <span data-ttu-id="beb0e-1193">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1193">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-1194">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1194">Key Vault</span></span>

* <span data-ttu-id="beb0e-1195">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1195">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="beb0e-1196">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1196">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1197">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1197">Network</span></span>

* <span data-ttu-id="beb0e-1198">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="beb0e-1198">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="beb0e-1199">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="beb0e-1199">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="beb0e-1200">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1200">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="beb0e-1201">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1201">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="beb0e-1202">Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-1202">Policy</span></span>

* <span data-ttu-id="beb0e-1203">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-1203">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="beb0e-1204">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1204">August 27, 2019</span></span>

<span data-ttu-id="beb0e-1205">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="beb0e-1205">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1206">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1206">ACR</span></span>

* <span data-ttu-id="beb0e-1207">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1207">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="beb0e-1208">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="beb0e-1208">API Management</span></span>

* <span data-ttu-id="beb0e-1209">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1209">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1210">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1210">AppService</span></span>

* <span data-ttu-id="beb0e-1211">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1211">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="beb0e-1212">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1212">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-1213">Keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1213">Keyvault</span></span>

* <span data-ttu-id="beb0e-1214">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1214">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1215">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1215">Network</span></span>

* <span data-ttu-id="beb0e-1216">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1216">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="beb0e-1217">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1217">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="beb0e-1218">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1218">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="beb0e-1219">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1219">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1220">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1220">RBAC</span></span>

* <span data-ttu-id="beb0e-1221">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="beb0e-1221">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="beb0e-1222">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-1222">ServiceFabric</span></span>

* <span data-ttu-id="beb0e-1223">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1223">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="beb0e-1224">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1224">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="beb0e-1225">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="beb0e-1225">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="beb0e-1226">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1226">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="beb0e-1227">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-1227">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="beb0e-1228">SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1228">SignalR</span></span>

* <span data-ttu-id="beb0e-1229">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1229">Added new commands:</span></span>
  * <span data-ttu-id="beb0e-1230">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1230">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="beb0e-1231">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1231">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="beb0e-1232">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1232">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="beb0e-1233">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1233">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1234">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1234">Storage</span></span>

* <span data-ttu-id="beb0e-1235">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1235">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="beb0e-1236">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1236">August 13, 2019</span></span>

<span data-ttu-id="beb0e-1237">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="beb0e-1237">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1238">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1238">AppService</span></span>

* <span data-ttu-id="beb0e-1239">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1239">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1240">BotService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1240">BotService</span></span>

* <span data-ttu-id="beb0e-1241">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1241">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="beb0e-1242">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="beb0e-1242">CognitiveServices</span></span>

* <span data-ttu-id="beb0e-1243">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1243">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-1244">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1244">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-1245">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1245">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="beb0e-1246">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1246">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1247">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1247">HDInsight</span></span>

<span data-ttu-id="beb0e-1248">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1248">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="beb0e-1249">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1249">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="beb0e-1250">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1250">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="beb0e-1251">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1251">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="beb0e-1252">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-1252">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="beb0e-1253">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="beb0e-1253">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="beb0e-1254">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1254">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="beb0e-1255">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1255">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="beb0e-1256">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1256">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="beb0e-1257">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1257">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="beb0e-1258">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1258">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="beb0e-1259">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1259">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="beb0e-1260">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1260">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="beb0e-1261">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1261">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="beb0e-1262">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="beb0e-1262">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="beb0e-1263">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1263">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="beb0e-1264">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1264">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="beb0e-1265">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="beb0e-1265">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="beb0e-1266">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1266">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="beb0e-1267">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="beb0e-1267">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="beb0e-1268">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1268">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="beb0e-1269">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-1269">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="beb0e-1270">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1270">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="beb0e-1271">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1271">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-1272">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1272">Interactive</span></span>

* <span data-ttu-id="beb0e-1273">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1273">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="beb0e-1274">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1274">Kubernetes</span></span>

* <span data-ttu-id="beb0e-1275">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1275">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1276">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1276">Network</span></span>

* <span data-ttu-id="beb0e-1277">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1277">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1278">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1278">Profile</span></span>

* <span data-ttu-id="beb0e-1279">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1279">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="beb0e-1280">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-1280">ServiceFabric</span></span>

* <span data-ttu-id="beb0e-1281">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1281">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="beb0e-1282">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="beb0e-1282">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1283">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1283">Storage</span></span>

* <span data-ttu-id="beb0e-1284">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1284">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="beb0e-1285">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1285">July 30, 2019</span></span>

<span data-ttu-id="beb0e-1286">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="beb0e-1286">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1287">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1287">ACR</span></span>

* <span data-ttu-id="beb0e-1288">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1288">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="beb0e-1289">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1289">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1290">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1290">Appservice</span></span>

* <span data-ttu-id="beb0e-1291">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1291">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="beb0e-1292">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1292">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="beb0e-1293">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="beb0e-1293">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1294">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1294">Network</span></span>

* <span data-ttu-id="beb0e-1295">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1295">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="beb0e-1296">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1296">Fixes #9604.</span></span> <span data-ttu-id="beb0e-1297">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1297">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="beb0e-1298">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1298">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1299">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1299">RBAC</span></span>

* <span data-ttu-id="beb0e-1300">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1300">Added `user update` command</span></span>
* <span data-ttu-id="beb0e-1301">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-1301">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="beb0e-1302">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1302">Use replacement argument `--id`</span></span>
* <span data-ttu-id="beb0e-1303">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-1303">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1304">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1304">SQL</span></span>

* <span data-ttu-id="beb0e-1305">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="beb0e-1305">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1306">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1306">Storage</span></span>

* <span data-ttu-id="beb0e-1307">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1307">Added `storage remove` command</span></span>
* <span data-ttu-id="beb0e-1308">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1308">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1309">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1309">VM</span></span>

* <span data-ttu-id="beb0e-1310">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="beb0e-1310">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="beb0e-1311">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1311">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="beb0e-1312">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1312">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="beb0e-1313">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1313">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="beb0e-1314">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1314">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="beb0e-1315">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1315">July 16, 2019</span></span>

<span data-ttu-id="beb0e-1316">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="beb0e-1316">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1317">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1317">Appservice</span></span>

* <span data-ttu-id="beb0e-1318">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1318">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="beb0e-1319">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1319">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="beb0e-1320">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1320">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1321">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1321">Core</span></span>

* <span data-ttu-id="beb0e-1322">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="beb0e-1322">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1323">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1323">Batch</span></span>

* <span data-ttu-id="beb0e-1324">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1324">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="beb0e-1325">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1325">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="beb0e-1326">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1326">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="beb0e-1327">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="beb0e-1327">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="beb0e-1328">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1328">Eventhubs</span></span>

* <span data-ttu-id="beb0e-1329">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1329">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-1330">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1330">RDBMS</span></span>

* <span data-ttu-id="beb0e-1331">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="beb0e-1331">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="beb0e-1332">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1332">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="beb0e-1333">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1333">Relay</span></span>

* <span data-ttu-id="beb0e-1334">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1334">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="beb0e-1335">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1335">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="beb0e-1336">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-1336">Servicebus</span></span>

* <span data-ttu-id="beb0e-1337">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1337">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1338">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1338">Storage</span></span>

* <span data-ttu-id="beb0e-1339">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1339">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="beb0e-1340">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1340">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="beb0e-1341">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1341">July 2, 2019</span></span>

<span data-ttu-id="beb0e-1342">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="beb0e-1342">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1343">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1343">Core</span></span>

* <span data-ttu-id="beb0e-1344">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1344">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="beb0e-1345">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1345">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="beb0e-1346">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1346">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1347">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1347">ACR</span></span>

* <span data-ttu-id="beb0e-1348">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="beb0e-1348">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1349">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1349">Appservice</span></span>

* <span data-ttu-id="beb0e-1350">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1350">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="beb0e-1351">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1351">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="beb0e-1352">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1352">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="beb0e-1353">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1353">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-1354">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1354">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-1355">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1355">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="beb0e-1356">DLS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1356">DLS</span></span>

* <span data-ttu-id="beb0e-1357">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1357">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="beb0e-1358">Comentários</span><span class="sxs-lookup"><span data-stu-id="beb0e-1358">Feedback</span></span>

* <span data-ttu-id="beb0e-1359">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="beb0e-1359">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1360">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1360">HDInsight</span></span>

* <span data-ttu-id="beb0e-1361">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1361">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="beb0e-1362">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="beb0e-1362">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="beb0e-1363">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1363">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="beb0e-1364">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1364">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="beb0e-1365">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1365">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="beb0e-1366">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1366">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="beb0e-1367">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1367">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="beb0e-1368">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1368">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="beb0e-1369">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1369">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="beb0e-1370">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1370">Managed Services</span></span>

* <span data-ttu-id="beb0e-1371">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-1371">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1372">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1372">Profile</span></span>
* <span data-ttu-id="beb0e-1373">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="beb0e-1373">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1374">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1374">RBAC</span></span>

* <span data-ttu-id="beb0e-1375">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1375">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="beb0e-1376">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="beb0e-1376">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="beb0e-1377">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="beb0e-1377">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="beb0e-1378">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-1378">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-1379">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1379">RDBMS</span></span>

* <span data-ttu-id="beb0e-1380">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1380">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1381">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1381">SQL</span></span>

* <span data-ttu-id="beb0e-1382">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1382">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1383">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1383">Storage</span></span>

* <span data-ttu-id="beb0e-1384">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1384">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="beb0e-1385">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1385">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="beb0e-1386">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1386">VM</span></span>

* <span data-ttu-id="beb0e-1387">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1387">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="beb0e-1388">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1388">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="beb0e-1389">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1389">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="beb0e-1390">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1390">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="beb0e-1391">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1391">June 18, 2019</span></span>

<span data-ttu-id="beb0e-1392">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="beb0e-1392">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1393">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1393">Core</span></span>

<span data-ttu-id="beb0e-1394">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1394">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="beb0e-1395">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1395">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="beb0e-1396">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1396">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="beb0e-1397">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1397">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="beb0e-1398">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1398">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="beb0e-1399">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1399">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="beb0e-1400">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1400">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1401">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1401">ACR</span></span>
* <span data-ttu-id="beb0e-1402">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="beb0e-1402">Added 'acr check-health' command</span></span>
* <span data-ttu-id="beb0e-1403">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1403">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1404">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1404">ACS</span></span>
* <span data-ttu-id="beb0e-1405">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-1405">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1406">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1406">AMS</span></span>
* <span data-ttu-id="beb0e-1407">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="beb0e-1407">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1408">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1408">AppService</span></span>
* <span data-ttu-id="beb0e-1409">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1409">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="beb0e-1410">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="beb0e-1410">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="beb0e-1411">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="beb0e-1411">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="beb0e-1412">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1412">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="beb0e-1413">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1413">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="beb0e-1414">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1414">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1415">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1415">Batch</span></span>
* <span data-ttu-id="beb0e-1416">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="beb0e-1416">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-1417">BatchAI</span><span class="sxs-lookup"><span data-stu-id="beb0e-1417">BatchAI</span></span>
* <span data-ttu-id="beb0e-1418">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1418">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1419">BotService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1419">BotService</span></span>
* <span data-ttu-id="beb0e-1420">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="beb0e-1420">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-1421">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1421">CosmosDB</span></span>
* <span data-ttu-id="beb0e-1422">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1422">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="beb0e-1423">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1423">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="beb0e-1424">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="beb0e-1424">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="beb0e-1425">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1425">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="beb0e-1426">EventGrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-1426">EventGrid</span></span>
* <span data-ttu-id="beb0e-1427">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="beb0e-1427">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="beb0e-1428">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="beb0e-1428">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="beb0e-1429">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="beb0e-1429">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="beb0e-1430">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1430">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="beb0e-1431">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1431">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1432">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1432">HDInsight</span></span>
* <span data-ttu-id="beb0e-1433">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1433">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1434">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1434">IoT</span></span>
* <span data-ttu-id="beb0e-1435">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="beb0e-1435">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="beb0e-1436">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="beb0e-1436">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1437">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1437">Network</span></span>
* <span data-ttu-id="beb0e-1438">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1438">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="beb0e-1439">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1439">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="beb0e-1440">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="beb0e-1440">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="beb0e-1441">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="beb0e-1441">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1442">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1442">Resource</span></span>
* <span data-ttu-id="beb0e-1443">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="beb0e-1443">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="beb0e-1444">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1444">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="beb0e-1445">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="beb0e-1445">ServiceBus</span></span>
* <span data-ttu-id="beb0e-1446">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1446">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1447">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1447">SQL</span></span>
* <span data-ttu-id="beb0e-1448">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1448">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="beb0e-1449">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1449">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="beb0e-1450">SQLVm</span><span class="sxs-lookup"><span data-stu-id="beb0e-1450">SQLVm</span></span>
* <span data-ttu-id="beb0e-1451">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1451">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="beb0e-1452">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1452">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1453">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1453">Storage</span></span>
* <span data-ttu-id="beb0e-1454">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1454">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="beb0e-1455">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-1455">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1456">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1456">VM</span></span>
* <span data-ttu-id="beb0e-1457">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1457">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="beb0e-1458">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1458">June 4, 2019</span></span>

<span data-ttu-id="beb0e-1459">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="beb0e-1459">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1460">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1460">Core</span></span>
* <span data-ttu-id="beb0e-1461">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1461">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1462">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1462">ACR</span></span>
* <span data-ttu-id="beb0e-1463">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1463">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1464">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1464">ACS</span></span>
* <span data-ttu-id="beb0e-1465">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1465">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="beb0e-1466">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-1466">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1467">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1467">Batch</span></span>
* <span data-ttu-id="beb0e-1468">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="beb0e-1468">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1469">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1469">IoT</span></span>
* <span data-ttu-id="beb0e-1470">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="beb0e-1470">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1471">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1471">Network</span></span>
* <span data-ttu-id="beb0e-1472">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1472">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="beb0e-1473">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1473">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="beb0e-1474">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1474">Resource</span></span>
* <span data-ttu-id="beb0e-1475">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="beb0e-1475">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1476">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1476">Role</span></span>
* <span data-ttu-id="beb0e-1477">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1477">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-1478">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1478">Compute</span></span>
* <span data-ttu-id="beb0e-1479">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="beb0e-1479">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="beb0e-1480">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1480">May 21, 2019</span></span>

<span data-ttu-id="beb0e-1481">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="beb0e-1481">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1482">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1482">Core</span></span>
* <span data-ttu-id="beb0e-1483">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1483">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="beb0e-1484">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1484">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="beb0e-1485">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1485">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1486">ACR</span></span>
* <span data-ttu-id="beb0e-1487">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1487">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1488">ACS</span></span>
* <span data-ttu-id="beb0e-1489">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="beb0e-1489">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1490">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1490">AppService</span></span>
* <span data-ttu-id="beb0e-1491">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1491">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="beb0e-1492">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1492">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="beb0e-1493">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="beb0e-1493">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="beb0e-1494">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1494">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="beb0e-1495">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1495">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="beb0e-1496">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1496">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="beb0e-1497">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-1497">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1498">BotService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1498">BotService</span></span>
* <span data-ttu-id="beb0e-1499">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1499">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="beb0e-1500">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-1500">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-1501">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1501">Consumption</span></span>
* <span data-ttu-id="beb0e-1502">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1502">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1503">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1503">IoT</span></span>
* <span data-ttu-id="beb0e-1504">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="beb0e-1504">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1505">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1505">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="beb0e-1507">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1507">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="beb0e-1508">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1508">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-1509">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1509">RDBMS</span></span>
* <span data-ttu-id="beb0e-1510">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="beb0e-1510">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-1511">RBAC</span><span class="sxs-lookup"><span data-stu-id="beb0e-1511">RBAC</span></span>
* <span data-ttu-id="beb0e-1512">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1512">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1513">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1513">Storage</span></span>
* <span data-ttu-id="beb0e-1514">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="beb0e-1514">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="beb0e-1515">Computação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1515">Compute</span></span>
* <span data-ttu-id="beb0e-1516">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1516">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="beb0e-1517">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="beb0e-1517">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="beb0e-1518">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1518">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="beb0e-1519">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="beb0e-1519">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="beb0e-1520">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1520">May 6, 2019</span></span>

<span data-ttu-id="beb0e-1521">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="beb0e-1521">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1522">ACS</span></span>
* <span data-ttu-id="beb0e-1523">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1523">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="beb0e-1524">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="beb0e-1524">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="beb0e-1525">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1525">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="beb0e-1526">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1526">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1527">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1527">Appservice</span></span>
* <span data-ttu-id="beb0e-1528">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1528">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="beb0e-1529">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1529">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="beb0e-1530">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1530">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="beb0e-1531">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="beb0e-1531">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="beb0e-1532">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1532">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="beb0e-1533">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1533">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="beb0e-1534">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-1534">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="beb0e-1535">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="beb0e-1535">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="beb0e-1536">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-1536">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="beb0e-1537">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1537">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1538">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1538">Batch</span></span>
* <span data-ttu-id="beb0e-1539">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1539">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1540">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1540">Botservice</span></span>
* <span data-ttu-id="beb0e-1541">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1541">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="beb0e-1542">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1542">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="beb0e-1543">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1543">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="beb0e-1544">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1544">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="beb0e-1545">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1545">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="beb0e-1546">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1546">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="beb0e-1547">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1547">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="beb0e-1548">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1548">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="beb0e-1549">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="beb0e-1549">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="beb0e-1550">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="beb0e-1550">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="beb0e-1551">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1551">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="beb0e-1552">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1552">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="beb0e-1553">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1553">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="beb0e-1554">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1554">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="beb0e-1555">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1555">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="beb0e-1556">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1556">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="beb0e-1557">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1557">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="beb0e-1558">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1558">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="beb0e-1559">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1559">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="beb0e-1560">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1560">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="beb0e-1561">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1561">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="beb0e-1562">Configurar</span><span class="sxs-lookup"><span data-stu-id="beb0e-1562">Configure</span></span>
* <span data-ttu-id="beb0e-1563">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="beb0e-1563">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="beb0e-1564">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1564">Eventhubs</span></span>
* <span data-ttu-id="beb0e-1565">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1565">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="beb0e-1566">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1566">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1567">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1567">Network</span></span>
* <span data-ttu-id="beb0e-1568">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1568">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="beb0e-1569">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-1569">Policy Insights</span></span>
* <span data-ttu-id="beb0e-1570">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1570">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1571">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1571">Role</span></span>
* <span data-ttu-id="beb0e-1572">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1572">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="beb0e-1573">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-1573">Service Bus</span></span>
* <span data-ttu-id="beb0e-1574">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1574">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="beb0e-1575">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1575">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="beb0e-1576">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="beb0e-1576">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1577">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1577">SQL</span></span>
* <span data-ttu-id="beb0e-1578">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1578">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1579">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1579">VM</span></span>
* <span data-ttu-id="beb0e-1580">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1580">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="beb0e-1581">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1581">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="beb0e-1582">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1582">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="beb0e-1583">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-1583">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="beb0e-1584">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="beb0e-1584">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="beb0e-1585">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1585">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="beb0e-1586">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1586">April 23, 2019</span></span>

<span data-ttu-id="beb0e-1587">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="beb0e-1587">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1588">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1588">ACS</span></span>
* <span data-ttu-id="beb0e-1589">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1589">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="beb0e-1590">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="beb0e-1590">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1591">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1591">AMS</span></span>
* <span data-ttu-id="beb0e-1592">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1592">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1593">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1593">AppService</span></span>
* <span data-ttu-id="beb0e-1594">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1594">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="beb0e-1595">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="beb0e-1595">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="beb0e-1596">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="beb0e-1596">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="beb0e-1597">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="beb0e-1597">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="beb0e-1598">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="beb0e-1598">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="beb0e-1599">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1599">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="beb0e-1600">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="beb0e-1600">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="beb0e-1601">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="beb0e-1601">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="beb0e-1602">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1602">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="beb0e-1603">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1603">Deployment Manager</span></span>
* <span data-ttu-id="beb0e-1604">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="beb0e-1604">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="beb0e-1605">Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-1605">Lab</span></span>
* <span data-ttu-id="beb0e-1606">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-1606">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1607">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1607">Network</span></span>
* <span data-ttu-id="beb0e-1608">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="beb0e-1608">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1609">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1609">Resource</span></span>
* <span data-ttu-id="beb0e-1610">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1610">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="beb0e-1611">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1611">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="beb0e-1612">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="beb0e-1612">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="beb0e-1613">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1613">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1614">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1614">SQL</span></span>
* <span data-ttu-id="beb0e-1615">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1615">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="beb0e-1616">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1616">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="beb0e-1617">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1617">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="beb0e-1618">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1618">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1619">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1619">Storage</span></span>
* <span data-ttu-id="beb0e-1620">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1620">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1621">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1621">VM</span></span>
* <span data-ttu-id="beb0e-1622">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1622">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="beb0e-1623">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1623">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="beb0e-1624">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="beb0e-1624">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="beb0e-1625">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1625">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1626">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1626">Core</span></span>
* <span data-ttu-id="beb0e-1627">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1627">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1628">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1628">ACR</span></span>
* <span data-ttu-id="beb0e-1629">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1629">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1630">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1630">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="beb0e-1633">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1633">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="beb0e-1634">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1634">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1635">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1635">AppService</span></span>
* <span data-ttu-id="beb0e-1636">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1636">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="beb0e-1637">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1637">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="beb0e-1638">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1638">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="beb0e-1639">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="beb0e-1639">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="beb0e-1640">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-1640">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="beb0e-1641">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1641">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="beb0e-1642">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="beb0e-1642">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-1643">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-1643">CDN</span></span>
* <span data-ttu-id="beb0e-1644">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1644">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="beb0e-1645">Comentários</span><span class="sxs-lookup"><span data-stu-id="beb0e-1645">Feedback</span></span>
* <span data-ttu-id="beb0e-1646">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1646">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="beb0e-1647">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="beb0e-1647">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="beb0e-1648">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="beb0e-1648">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1649">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1649">Monitor</span></span>
* <span data-ttu-id="beb0e-1650">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1650">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="beb0e-1651">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1651">Network</span></span>
* <span data-ttu-id="beb0e-1652">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1652">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="beb0e-1653">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1653">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="beb0e-1654">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1654">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="beb0e-1655">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1655">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="beb0e-1656">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1656">PrivateDNS</span></span>
* <span data-ttu-id="beb0e-1657">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1657">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1658">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1658">Resource</span></span>
* <span data-ttu-id="beb0e-1659">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="beb0e-1659">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1660">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1660">Role</span></span>
* <span data-ttu-id="beb0e-1661">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1661">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="beb0e-1662">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1662">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1663">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1663">SQL</span></span>
* <span data-ttu-id="beb0e-1664">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="beb0e-1664">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1665">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1665">Storage</span></span>
* <span data-ttu-id="beb0e-1666">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1666">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="beb0e-1667">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1667">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="beb0e-1668">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1668">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="beb0e-1669">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="beb0e-1669">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="beb0e-1670">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1670">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="beb0e-1671">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1671">Core</span></span>
* <span data-ttu-id="beb0e-1672">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1672">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="beb0e-1673">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1673">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="beb0e-1674">Nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-1674">Cloud</span></span>
* <span data-ttu-id="beb0e-1675">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1675">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1676">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1676">ACR</span></span>
* <span data-ttu-id="beb0e-1677">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1677">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="beb0e-1678">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1678">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="beb0e-1679">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="beb0e-1679">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="beb0e-1680">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1680">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1681">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1681">AppService</span></span>
* <span data-ttu-id="beb0e-1682">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1682">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="beb0e-1683">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1683">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="beb0e-1684">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1684">BOT Service</span></span>
* <span data-ttu-id="beb0e-1685">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1685">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="beb0e-1686">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="beb0e-1686">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="beb0e-1687">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1687">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="beb0e-1688">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1688">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-1689">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-1689">CDN</span></span>
* <span data-ttu-id="beb0e-1690">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1690">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="beb0e-1692">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="beb0e-1692">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="beb0e-1693">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-1693">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-1694">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="beb0e-1694">Cosmosdb</span></span>
* <span data-ttu-id="beb0e-1695">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="beb0e-1695">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="beb0e-1696">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1696">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-1697">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1697">Interactive</span></span>
* <span data-ttu-id="beb0e-1698">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="beb0e-1698">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1699">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1699">Monitor</span></span>
* <span data-ttu-id="beb0e-1700">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1700">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1701">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1701">Network</span></span>
* <span data-ttu-id="beb0e-1702">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1702">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1703">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1703">Profile</span></span>
* <span data-ttu-id="beb0e-1704">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1704">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="beb0e-1705">Postgres</span><span class="sxs-lookup"><span data-stu-id="beb0e-1705">Postgres</span></span> 
* <span data-ttu-id="beb0e-1706">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1706">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="beb0e-1707">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="beb0e-1707">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1708">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1708">Resource</span></span>
* <span data-ttu-id="beb0e-1709">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1709">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="beb0e-1710">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1710">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="beb0e-1711">Grafo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1711">Graph</span></span>
* <span data-ttu-id="beb0e-1712">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1712">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="beb0e-1713">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1713">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="beb0e-1714">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1714">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="beb0e-1715">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-1715">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="beb0e-1716">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1716">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1717">armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1717">storage</span></span>
* <span data-ttu-id="beb0e-1718">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1718">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="beb0e-1719">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="beb0e-1719">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="beb0e-1720">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="beb0e-1720">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="beb0e-1721">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1721">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1722">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1722">VM</span></span>
* <span data-ttu-id="beb0e-1723">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1723">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="beb0e-1724">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1724">March 12, 2019</span></span>

<span data-ttu-id="beb0e-1725">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="beb0e-1725">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1726">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1726">Core</span></span>

* <span data-ttu-id="beb0e-1727">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1727">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1728">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1728">ACR</span></span>

* <span data-ttu-id="beb0e-1729">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1729">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1730">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1730">ACS</span></span>

* <span data-ttu-id="beb0e-1731">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="beb0e-1731">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="beb0e-1732">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1732">AppService</span></span>

* <span data-ttu-id="beb0e-1733">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1733">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="beb0e-1734">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1734">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="beb0e-1735">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1735">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="beb0e-1736">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1736">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1737">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1737">Botservice</span></span>

* <span data-ttu-id="beb0e-1738">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1738">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="beb0e-1739">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1739">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="beb0e-1740">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1740">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="beb0e-1741">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1741">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-1742">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-1742">Container</span></span>

* <span data-ttu-id="beb0e-1743">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1743">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="beb0e-1744">EventHub</span><span class="sxs-lookup"><span data-stu-id="beb0e-1744">EventHub</span></span>

* <span data-ttu-id="beb0e-1745">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1745">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="beb0e-1746">Localizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-1746">Find</span></span>

* <span data-ttu-id="beb0e-1747">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="beb0e-1747">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1748">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1748">HDInsight</span></span>

* <span data-ttu-id="beb0e-1749">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1749">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1750">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1750">Network</span></span>

* <span data-ttu-id="beb0e-1751">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1751">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-1752">Rdbms</span><span class="sxs-lookup"><span data-stu-id="beb0e-1752">Rdbms</span></span>

* <span data-ttu-id="beb0e-1753">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1753">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1754">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1754">Role</span></span>

* <span data-ttu-id="beb0e-1755">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1755">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="beb0e-1756">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1756">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="beb0e-1757">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-1757">Service Fabric</span></span>

* <span data-ttu-id="beb0e-1758">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1758">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="beb0e-1759">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1759">February 26, 2019</span></span>

<span data-ttu-id="beb0e-1760">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="beb0e-1760">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1761">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1761">Core</span></span>

* <span data-ttu-id="beb0e-1762">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="beb0e-1762">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1763">ACR</span></span>

* <span data-ttu-id="beb0e-1764">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1764">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="beb0e-1765">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-1765">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1766">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1766">ACS</span></span>

* <span data-ttu-id="beb0e-1767">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1767">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1768">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1768">AppService</span></span>

* <span data-ttu-id="beb0e-1769">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1769">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-1770">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-1770">Batch</span></span>
* <span data-ttu-id="beb0e-1771">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1771">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="beb0e-1772">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1772">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="beb0e-1773">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1773">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="beb0e-1774">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="beb0e-1774">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="beb0e-1775">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="beb0e-1775">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="beb0e-1776">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1776">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-1777">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1777">CosmosDB</span></span>

* <span data-ttu-id="beb0e-1778">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1778">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="beb0e-1779">Kusto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1779">Kusto</span></span>

* <span data-ttu-id="beb0e-1780">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="beb0e-1780">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1781">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1781">Network</span></span>

* <span data-ttu-id="beb0e-1782">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1782">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="beb0e-1783">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1783">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="beb0e-1784">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1784">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="beb0e-1785">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1785">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="beb0e-1786">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1786">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="beb0e-1787">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1787">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="beb0e-1788">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1788">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1789">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1789">Resource</span></span>

* <span data-ttu-id="beb0e-1790">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1790">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="beb0e-1791">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1791">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="beb0e-1792">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1792">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="beb0e-1793">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1793">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="beb0e-1794">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-1794">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1795">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1795">Role</span></span>

* <span data-ttu-id="beb0e-1796">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1796">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1797">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1797">VM</span></span>

* <span data-ttu-id="beb0e-1798">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-1798">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="beb0e-1799">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1799">February 12, 2019</span></span>

<span data-ttu-id="beb0e-1800">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="beb0e-1800">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1801">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1801">Core</span></span>

* <span data-ttu-id="beb0e-1802">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-1802">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="beb0e-1803">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="beb0e-1803">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1804">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1804">ACR</span></span>
* <span data-ttu-id="beb0e-1805">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1805">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="beb0e-1806">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1806">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1807">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1807">ACS</span></span>
* <span data-ttu-id="beb0e-1808">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1808">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="beb0e-1809">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1809">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="beb0e-1810">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1810">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1811">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1811">AMS</span></span>
* <span data-ttu-id="beb0e-1812">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1812">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="beb0e-1813">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1813">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1814">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1814">Appservice</span></span>
* <span data-ttu-id="beb0e-1815">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1815">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="beb0e-1816">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="beb0e-1816">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="beb0e-1817">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1817">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="beb0e-1818">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="beb0e-1818">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="beb0e-1819">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1819">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1820">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1820">Botservice</span></span>
* <span data-ttu-id="beb0e-1821">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="beb0e-1821">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="beb0e-1822">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1822">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="beb0e-1823">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1823">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="beb0e-1824">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="beb0e-1824">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="beb0e-1825">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1825">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="beb0e-1826">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="beb0e-1826">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="beb0e-1827">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1827">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="beb0e-1828">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="beb0e-1828">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="beb0e-1829">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1829">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="beb0e-1830">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="beb0e-1830">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-1831">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-1831">Key Vault</span></span>
* <span data-ttu-id="beb0e-1832">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1832">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1833">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1833">Monitor</span></span>
* <span data-ttu-id="beb0e-1834">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1834">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1835">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1835">Network</span></span>
* <span data-ttu-id="beb0e-1836">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="beb0e-1836">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="beb0e-1837">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1837">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="beb0e-1838">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-1838">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="beb0e-1839">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1839">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="beb0e-1840">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-1840">Policy Insights</span></span>
* <span data-ttu-id="beb0e-1841">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1841">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-1842">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1842">RDBMS</span></span>
* <span data-ttu-id="beb0e-1843">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1843">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-1844">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-1844">Redis</span></span>
* <span data-ttu-id="beb0e-1845">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1845">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="beb0e-1846">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1846">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="beb0e-1847">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1847">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="beb0e-1848">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-1848">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="beb0e-1849">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1849">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="beb0e-1850">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="beb0e-1850">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="beb0e-1851">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1851">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1852">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1852">Role</span></span>
* <span data-ttu-id="beb0e-1853">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="beb0e-1853">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="beb0e-1854">SQL VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1854">SQL VM</span></span>
* <span data-ttu-id="beb0e-1855">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="beb0e-1855">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1856">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1856">VM</span></span>
* <span data-ttu-id="beb0e-1857">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1857">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="beb0e-1858">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1858">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="beb0e-1859">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="beb0e-1859">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="beb0e-1860">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1860">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="beb0e-1861">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1861">January 31, 2019</span></span>

<span data-ttu-id="beb0e-1862">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="beb0e-1862">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-1863">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1863">Core</span></span>

* <span data-ttu-id="beb0e-1864">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="beb0e-1864">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="beb0e-1865">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1865">January 28, 2019</span></span>

<span data-ttu-id="beb0e-1866">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="beb0e-1866">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1867">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1867">ACR</span></span>
* <span data-ttu-id="beb0e-1868">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="beb0e-1868">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1869">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1869">ACS</span></span>
* <span data-ttu-id="beb0e-1870">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="beb0e-1870">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="beb0e-1871">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1871">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="beb0e-1872">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1872">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-1873">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1873">AMS</span></span>
* <span data-ttu-id="beb0e-1874">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1874">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="beb0e-1875">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1875">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1876">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1876">Appservice</span></span>
* <span data-ttu-id="beb0e-1877">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1877">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="beb0e-1878">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="beb0e-1878">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="beb0e-1879">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="beb0e-1879">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-1880">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-1880">Container</span></span>
* <span data-ttu-id="beb0e-1881">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1881">Added `container start` command</span></span>
* <span data-ttu-id="beb0e-1882">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-1882">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="beb0e-1883">EventGrid</span><span class="sxs-lookup"><span data-stu-id="beb0e-1883">EventGrid</span></span>
* <span data-ttu-id="beb0e-1884">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1884">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="beb0e-1885">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1885">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="beb0e-1886">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1886">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="beb0e-1887">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1887">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="beb0e-1888">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1888">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1889">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1889">HDInsight</span></span>
* <span data-ttu-id="beb0e-1890">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1890">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="beb0e-1891">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="beb0e-1891">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="beb0e-1892">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1892">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="beb0e-1893">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1893">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="beb0e-1894">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1894">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="beb0e-1895">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1895">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-1896">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-1896">IoT</span></span>
* <span data-ttu-id="beb0e-1897">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="beb0e-1897">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="beb0e-1898">Kusto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1898">Kusto</span></span>
* <span data-ttu-id="beb0e-1899">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-1899">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-1900">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1900">Monitor</span></span>
* <span data-ttu-id="beb0e-1901">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1901">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-1902">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-1902">Profile</span></span>
* <span data-ttu-id="beb0e-1903">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1903">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1904">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1904">Network</span></span>
* <span data-ttu-id="beb0e-1905">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="beb0e-1905">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="beb0e-1906">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="beb0e-1906">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-1907">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-1907">Resource</span></span>
* <span data-ttu-id="beb0e-1908">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1908">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="beb0e-1909">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1909">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="beb0e-1910">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1910">SQL Virtual Machine</span></span>
* <span data-ttu-id="beb0e-1911">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-1911">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1912">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1912">Storage</span></span>
* <span data-ttu-id="beb0e-1913">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="beb0e-1913">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="beb0e-1914">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1914">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1915">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1915">VM</span></span>
* <span data-ttu-id="beb0e-1916">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="beb0e-1916">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="beb0e-1917">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1917">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="beb0e-1918">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="beb0e-1918">January 15, 2019</span></span>

<span data-ttu-id="beb0e-1919">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="beb0e-1919">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-1920">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1920">ACR</span></span>
* <span data-ttu-id="beb0e-1921">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="beb0e-1921">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="beb0e-1922">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1922">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="beb0e-1923">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="beb0e-1923">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="beb0e-1924">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1924">ACS</span></span>
* <span data-ttu-id="beb0e-1925">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="beb0e-1925">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1926">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1926">Appservice</span></span>
* <span data-ttu-id="beb0e-1927">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1927">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="beb0e-1928">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-1928">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="beb0e-1929">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="beb0e-1929">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="beb0e-1930">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1930">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1931">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1931">Botservice</span></span>
* <span data-ttu-id="beb0e-1932">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1932">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="beb0e-1933">Configurar</span><span class="sxs-lookup"><span data-stu-id="beb0e-1933">Configure</span></span>
* <span data-ttu-id="beb0e-1934">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="beb0e-1934">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-1935">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-1935">CosmosDB</span></span>
* <span data-ttu-id="beb0e-1936">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="beb0e-1936">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-1937">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-1937">HDInsight</span></span>
* <span data-ttu-id="beb0e-1938">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1938">Added commands for managing applications</span></span>
* <span data-ttu-id="beb0e-1939">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="beb0e-1939">Added commands for managing script actions</span></span>
* <span data-ttu-id="beb0e-1940">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="beb0e-1940">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="beb0e-1941">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1941">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="beb0e-1942">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-1942">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-1943">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-1943">Network</span></span>
* <span data-ttu-id="beb0e-1944">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1944">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="beb0e-1945">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="beb0e-1945">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="beb0e-1946">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1946">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="beb0e-1947">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-1947">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1948">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1948">Role</span></span>
* <span data-ttu-id="beb0e-1949">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1949">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="beb0e-1950">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-1950">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="beb0e-1951">Segurança</span><span class="sxs-lookup"><span data-stu-id="beb0e-1951">Security</span></span>
* <span data-ttu-id="beb0e-1952">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-1952">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-1953">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-1953">Storage</span></span>
* <span data-ttu-id="beb0e-1954">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1954">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="beb0e-1955">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="beb0e-1955">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="beb0e-1956">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1956">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="beb0e-1957">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1957">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="beb0e-1958">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1958">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1959">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1959">VM</span></span>
* <span data-ttu-id="beb0e-1960">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-1960">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="beb0e-1961">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1961">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="beb0e-1962">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1962">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="beb0e-1963">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="beb0e-1963">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="beb0e-1964">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1964">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="beb0e-1965">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="beb0e-1965">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="beb0e-1966">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-1966">December 20, 2018</span></span>

<span data-ttu-id="beb0e-1967">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="beb0e-1967">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="beb0e-1968">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1968">Appservice</span></span>
* <span data-ttu-id="beb0e-1969">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1969">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="beb0e-1970">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="beb0e-1970">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="beb0e-1971">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-1971">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="beb0e-1972">IoT Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-1972">IoTCentral</span></span>
* <span data-ttu-id="beb0e-1973">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-1973">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-1974">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-1974">Role</span></span>
* <span data-ttu-id="beb0e-1975">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-1975">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-1976">SQL</span></span>
* <span data-ttu-id="beb0e-1977">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1977">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-1978">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-1978">VM</span></span>
* <span data-ttu-id="beb0e-1979">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1979">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="beb0e-1980">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-1980">December 18, 2018</span></span>

<span data-ttu-id="beb0e-1981">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="beb0e-1981">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="beb0e-1982">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-1982">ACR</span></span>
* <span data-ttu-id="beb0e-1983">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="beb0e-1983">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="beb0e-1984">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="beb0e-1984">Condensed the table layout for task list</span></span>
* <span data-ttu-id="beb0e-1985">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="beb0e-1985">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-1986">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1986">ACS</span></span>
* <span data-ttu-id="beb0e-1987">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="beb0e-1987">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="beb0e-1988">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1988">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="beb0e-1989">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-1989">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="beb0e-1990">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-1990">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="beb0e-1991">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-1991">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="beb0e-1992">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="beb0e-1992">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-1993">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-1993">Appservice</span></span>
* <span data-ttu-id="beb0e-1994">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1994">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="beb0e-1995">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-1995">Botservice</span></span>
* <span data-ttu-id="beb0e-1996">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-1996">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="beb0e-1997">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="beb0e-1997">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="beb0e-1998">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="beb0e-1998">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="beb0e-1999">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="beb0e-1999">Reduced Kudu network calls</span></span>
* <span data-ttu-id="beb0e-2000">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2000">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-2001">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2001">Consumption</span></span>
* <span data-ttu-id="beb0e-2002">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="beb0e-2002">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-2003">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2003">CosmosDB</span></span>
* <span data-ttu-id="beb0e-2004">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="beb0e-2004">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="beb0e-2005">Mapas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2005">Maps</span></span>
* <span data-ttu-id="beb0e-2006">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2006">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2007">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2007">Network</span></span>
* <span data-ttu-id="beb0e-2008">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2008">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="beb0e-2009">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-2009">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2010">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2010">Resource</span></span>
* <span data-ttu-id="beb0e-2011">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2011">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="beb0e-2012">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2012">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2013">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2013">Storage</span></span>
*  <span data-ttu-id="beb0e-2014">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2014">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2015">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2015">VM</span></span>
* <span data-ttu-id="beb0e-2016">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="beb0e-2016">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="beb0e-2017">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2017">December 4, 2018</span></span>

<span data-ttu-id="beb0e-2018">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="beb0e-2018">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="beb0e-2019">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2019">Core</span></span>
* <span data-ttu-id="beb0e-2020">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="beb0e-2020">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="beb0e-2021">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2021">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2022">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2022">Appservice</span></span>
* <span data-ttu-id="beb0e-2023">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2023">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="beb0e-2024">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="beb0e-2024">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2025">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2025">Network</span></span>
* <span data-ttu-id="beb0e-2026">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="beb0e-2026">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2027">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2027">Role</span></span>
* <span data-ttu-id="beb0e-2028">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="beb0e-2028">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="beb0e-2029">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2029">VM</span></span>
* <span data-ttu-id="beb0e-2030">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2030">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="beb0e-2031">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="beb0e-2031">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="beb0e-2032">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="beb0e-2032">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="beb0e-2033">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2033">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="beb0e-2034">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2034">November 20, 2018</span></span>

<span data-ttu-id="beb0e-2035">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="beb0e-2035">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="beb0e-2036">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2036">Core</span></span>
* <span data-ttu-id="beb0e-2037">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-2037">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2038">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2038">ACR</span></span>
* <span data-ttu-id="beb0e-2039">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="beb0e-2039">Added context token to task step</span></span>
* <span data-ttu-id="beb0e-2040">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="beb0e-2040">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="beb0e-2041">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2041">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2042">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2042">Appservice</span></span>
* <span data-ttu-id="beb0e-2043">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="beb0e-2043">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="beb0e-2044">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2044">Updated the default `node_version`.</span></span> <span data-ttu-id="beb0e-2045">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2045">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="beb0e-2046">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2046">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="beb0e-2047">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="beb0e-2047">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="beb0e-2048">Iot Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-2048">IotCentral</span></span>
* <span data-ttu-id="beb0e-2049">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-2049">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-2050">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-2050">KeyVault</span></span>
* <span data-ttu-id="beb0e-2051">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2051">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2052">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2052">Network</span></span>
* <span data-ttu-id="beb0e-2053">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="beb0e-2053">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="beb0e-2054">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2054">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="beb0e-2055">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2055">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="beb0e-2056">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2056">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2057">Rdbms</span><span class="sxs-lookup"><span data-stu-id="beb0e-2057">Rdbms</span></span>
* <span data-ttu-id="beb0e-2058">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2058">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="beb0e-2059">Rbac</span><span class="sxs-lookup"><span data-stu-id="beb0e-2059">Rbac</span></span>
* <span data-ttu-id="beb0e-2060">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2060">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="beb0e-2061">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2061">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="beb0e-2062">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2062">Storage</span></span>
* <span data-ttu-id="beb0e-2063">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2063">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="beb0e-2064">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2064">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="beb0e-2065">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2065">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="beb0e-2066">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2066">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2067">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2067">VM</span></span>
* <span data-ttu-id="beb0e-2068">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2068">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="beb0e-2069">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2069">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="beb0e-2070">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2070">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="beb0e-2071">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2071">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="beb0e-2072">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2072">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="beb0e-2073">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2073">Added `snapshot wait` command</span></span>
* <span data-ttu-id="beb0e-2074">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2074">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="beb0e-2075">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2075">November 6, 2018</span></span>

<span data-ttu-id="beb0e-2076">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="beb0e-2076">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2077">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2077">Core</span></span>
* <span data-ttu-id="beb0e-2078">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="beb0e-2078">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2079">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2079">ACR</span></span>
* <span data-ttu-id="beb0e-2080">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="beb0e-2080">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="beb0e-2081">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="beb0e-2081">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2082">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2082">ACS</span></span>
* <span data-ttu-id="beb0e-2083">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2083">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="beb0e-2084">Supervisor</span><span class="sxs-lookup"><span data-stu-id="beb0e-2084">Advisor</span></span>
* <span data-ttu-id="beb0e-2085">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="beb0e-2085">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-2086">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2086">AMS</span></span>
* <span data-ttu-id="beb0e-2087">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2087">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="beb0e-2088">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2088">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="beb0e-2089">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2089">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="beb0e-2090">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2090">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="beb0e-2091">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2091">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="beb0e-2092">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2092">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="beb0e-2093">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2093">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="beb0e-2094">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2094">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="beb0e-2095">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2095">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="beb0e-2096">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2096">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="beb0e-2097">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2097">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="beb0e-2098">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2098">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="beb0e-2099">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="beb0e-2099">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="beb0e-2100">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2100">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="beb0e-2101">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2101">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="beb0e-2102">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2102">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="beb0e-2103">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="beb0e-2103">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2104">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2104">AppService</span></span>
* <span data-ttu-id="beb0e-2105">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2105">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="beb0e-2106">Configurar</span><span class="sxs-lookup"><span data-stu-id="beb0e-2106">Configure</span></span>
* <span data-ttu-id="beb0e-2107">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="beb0e-2107">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2108">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2108">Container</span></span>
* <span data-ttu-id="beb0e-2109">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="beb0e-2109">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="beb0e-2110">EventHub</span><span class="sxs-lookup"><span data-stu-id="beb0e-2110">EventHub</span></span>
* <span data-ttu-id="beb0e-2111">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2111">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2112">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2112">Interactive</span></span>
* <span data-ttu-id="beb0e-2113">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2113">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-2114">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2114">Monitor</span></span>
* <span data-ttu-id="beb0e-2115">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2115">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2116">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2116">Network</span></span>
* <span data-ttu-id="beb0e-2117">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2117">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="beb0e-2118">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="beb0e-2118">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="beb0e-2119">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2119">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="beb0e-2120">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-2120">Profile</span></span>
* <span data-ttu-id="beb0e-2121">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2121">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2122">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2122">RDBMS</span></span>
* <span data-ttu-id="beb0e-2123">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="beb0e-2123">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2124">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2124">Resource</span></span>
* <span data-ttu-id="beb0e-2125">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2125">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2126">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2126">Role</span></span>
* <span data-ttu-id="beb0e-2127">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2127">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="beb0e-2128">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2128">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="beb0e-2129">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="beb0e-2129">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2130">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2130">Storage</span></span>
* <span data-ttu-id="beb0e-2131">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2131">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2132">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2132">VM</span></span>
* <span data-ttu-id="beb0e-2133">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2133">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="beb0e-2134">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2134">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="beb0e-2135">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2135">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="beb0e-2136">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2136">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="beb0e-2137">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2137">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="beb0e-2138">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2138">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="beb0e-2139">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2139">October 23, 2018</span></span>

<span data-ttu-id="beb0e-2140">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="beb0e-2140">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2141">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2141">Core</span></span>
* <span data-ttu-id="beb0e-2142">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2142">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="beb0e-2143">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2143">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2144">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2144">ACR</span></span>
* <span data-ttu-id="beb0e-2145">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="beb0e-2145">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-2146">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-2146">CDN</span></span>
* <span data-ttu-id="beb0e-2147">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="beb0e-2147">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="beb0e-2148">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2148">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2149">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2149">Container</span></span>
* <span data-ttu-id="beb0e-2150">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="beb0e-2150">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="beb0e-2151">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-2151">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="beb0e-2152">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2152">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="beb0e-2153">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-2153">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="beb0e-2154">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="beb0e-2154">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="beb0e-2155">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="beb0e-2155">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="beb0e-2156">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2156">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-2157">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2157">CosmosDB</span></span>
* <span data-ttu-id="beb0e-2158">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2158">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2159">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2159">Interactive</span></span>
* <span data-ttu-id="beb0e-2160">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="beb0e-2160">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="beb0e-2161">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2161">IoT Central</span></span>
* <span data-ttu-id="beb0e-2162">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-2162">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="beb0e-2163">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="beb0e-2163">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-2164">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2164">Monitor</span></span>
* <span data-ttu-id="beb0e-2165">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2165">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="beb0e-2166">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2166">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="beb0e-2167">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2167">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="beb0e-2168">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-2168">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="beb0e-2169">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2169">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="beb0e-2170">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2170">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="beb0e-2171">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2171">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="beb0e-2172">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2172">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="beb0e-2173">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-2173">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="beb0e-2174">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2174">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2175">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2175">Network</span></span>
* <span data-ttu-id="beb0e-2176">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="beb0e-2176">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="beb0e-2177">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="beb0e-2177">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="beb0e-2178">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="beb0e-2178">ServiceBus</span></span>
* <span data-ttu-id="beb0e-2179">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2179">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2180">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2180">SQL</span></span>
* <span data-ttu-id="beb0e-2181">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="beb0e-2181">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2182">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2182">Storage</span></span>
* <span data-ttu-id="beb0e-2183">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="beb0e-2183">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="beb0e-2184">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-2184">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2185">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2185">VM</span></span>
* <span data-ttu-id="beb0e-2186">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2186">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="beb0e-2187">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2187">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="beb0e-2188">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2188">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="beb0e-2189">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2189">October 16, 2018</span></span>

<span data-ttu-id="beb0e-2190">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="beb0e-2190">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2191">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2191">VM</span></span>
* <span data-ttu-id="beb0e-2192">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="beb0e-2192">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="beb0e-2193">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2193">October 9, 2018</span></span>

<span data-ttu-id="beb0e-2194">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="beb0e-2194">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2195">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2195">Core</span></span>
* <span data-ttu-id="beb0e-2196">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="beb0e-2196">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2197">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2197">ACR</span></span>
* <span data-ttu-id="beb0e-2198">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="beb0e-2198">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2199">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2199">ACS</span></span>
* <span data-ttu-id="beb0e-2200">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="beb0e-2200">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="beb0e-2201">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="beb0e-2201">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="beb0e-2202">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2202">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="beb0e-2203">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2203">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2204">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2204">Container</span></span>
* <span data-ttu-id="beb0e-2205">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="beb0e-2205">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="beb0e-2206">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-2206">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="beb0e-2207">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2207">Event Hub</span></span>
* <span data-ttu-id="beb0e-2208">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2208">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="beb0e-2209">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="beb0e-2209">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="beb0e-2210">Extensões</span><span class="sxs-lookup"><span data-stu-id="beb0e-2210">Extensions</span></span>
* <span data-ttu-id="beb0e-2211">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2211">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="beb0e-2212">HDInsight</span><span class="sxs-lookup"><span data-stu-id="beb0e-2212">HDInsight</span></span>
* <span data-ttu-id="beb0e-2213">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2213">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-2214">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2214">IoT</span></span>
* <span data-ttu-id="beb0e-2215">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2215">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-2216">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-2216">KeyVault</span></span>
* <span data-ttu-id="beb0e-2217">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2217">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2218">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2218">Network</span></span>
* <span data-ttu-id="beb0e-2219">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2219">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="beb0e-2220">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="beb0e-2220">See #6052</span></span>
* <span data-ttu-id="beb0e-2221">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2221">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="beb0e-2222">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="beb0e-2222">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="beb0e-2223">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2223">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="beb0e-2224">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2224">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="beb0e-2225">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2225">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="beb0e-2226">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2226">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2227">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2227">Role</span></span>
* <span data-ttu-id="beb0e-2228">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2228">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="beb0e-2229">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2229">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="beb0e-2230">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2230">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="beb0e-2231">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="beb0e-2231">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="beb0e-2232">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2232">Service Bus</span></span>
* <span data-ttu-id="beb0e-2233">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="beb0e-2233">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2234">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2234">VM</span></span>
* <span data-ttu-id="beb0e-2235">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2235">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="beb0e-2236">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2236">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="beb0e-2237">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2237">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="beb0e-2238">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2238">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="beb0e-2239">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2239">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="beb0e-2240">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="beb0e-2240">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="beb0e-2241">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2241">September 21, 2018</span></span>

<span data-ttu-id="beb0e-2242">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="beb0e-2242">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2243">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2243">ACR</span></span>
* <span data-ttu-id="beb0e-2244">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2244">Added ACR Task commands</span></span>
* <span data-ttu-id="beb0e-2245">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2245">Added quick run command</span></span>
* <span data-ttu-id="beb0e-2246">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2246">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="beb0e-2247">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2247">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="beb0e-2248">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2248">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="beb0e-2249">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="beb0e-2249">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2250">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2250">ACS</span></span>
* <span data-ttu-id="beb0e-2251">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2251">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="beb0e-2252">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="beb0e-2252">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2253">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2253">AppService</span></span>

* <span data-ttu-id="beb0e-2254">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2254">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="beb0e-2255">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="beb0e-2255">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="beb0e-2256">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="beb0e-2256">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="beb0e-2257">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2257">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-2258">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2258">Batch</span></span>
* <span data-ttu-id="beb0e-2259">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="beb0e-2259">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="beb0e-2260">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2260">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="beb0e-2261">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2261">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="beb0e-2262">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2262">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="beb0e-2263">Lote AI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2263">Batch AI</span></span> 
* <span data-ttu-id="beb0e-2264">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2264">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="beb0e-2265">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2265">Cognitive Services</span></span>
* <span data-ttu-id="beb0e-2266">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2266">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="beb0e-2267">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2267">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="beb0e-2268">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2268">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="beb0e-2269">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2269">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="beb0e-2270">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2270">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="beb0e-2271">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2271">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2272">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2272">Container</span></span>
* <span data-ttu-id="beb0e-2273">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="beb0e-2273">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="beb0e-2274">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2274">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="beb0e-2275">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="beb0e-2275">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="beb0e-2276">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-2276">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="beb0e-2277">DataLake</span><span class="sxs-lookup"><span data-stu-id="beb0e-2277">Datalake</span></span>
* <span data-ttu-id="beb0e-2278">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="beb0e-2278">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="beb0e-2279">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2279">Interactive Shell</span></span>
* <span data-ttu-id="beb0e-2280">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2280">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="beb0e-2281">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2281">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-2282">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2282">IoT</span></span>
* <span data-ttu-id="beb0e-2283">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2283">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-2284">Key Vault</span><span class="sxs-lookup"><span data-stu-id="beb0e-2284">Key Vault</span></span>
* <span data-ttu-id="beb0e-2285">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="beb0e-2285">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2286">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2286">Network</span></span>
* <span data-ttu-id="beb0e-2287">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="beb0e-2287">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="beb0e-2288">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2288">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="beb0e-2289">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="beb0e-2289">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="beb0e-2290">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="beb0e-2290">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="beb0e-2291">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2291">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="beb0e-2292">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2292">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="beb0e-2293">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2293">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="beb0e-2294">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2294">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="beb0e-2295">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2295">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="beb0e-2296">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2296">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="beb0e-2297">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2297">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="beb0e-2298">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2298">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="beb0e-2299">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2299">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="beb0e-2300">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2300">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="beb0e-2301">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2301">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="beb0e-2302">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="beb0e-2302">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="beb0e-2303">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2303">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="beb0e-2304">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="beb0e-2304">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2305">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2305">RDBMS</span></span>
* <span data-ttu-id="beb0e-2306">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2306">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="beb0e-2307">Reserva</span><span class="sxs-lookup"><span data-stu-id="beb0e-2307">Reservation</span></span>
* <span data-ttu-id="beb0e-2308">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2308">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="beb0e-2309">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="beb0e-2309">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="beb0e-2310">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2310">Manage App</span></span>
* <span data-ttu-id="beb0e-2311">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="beb0e-2311">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="beb0e-2312">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="beb0e-2312">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2313">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2313">Role</span></span>
* <span data-ttu-id="beb0e-2314">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="beb0e-2314">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="beb0e-2315">SignalR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2315">SignalR</span></span>
* <span data-ttu-id="beb0e-2316">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2316">First release</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2317">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2317">Storage</span></span>
* <span data-ttu-id="beb0e-2318">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="beb0e-2318">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="beb0e-2319">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="beb0e-2319">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2320">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2320">VM</span></span>
* <span data-ttu-id="beb0e-2321">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2321">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="beb0e-2322">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2322">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="beb0e-2323">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2323">August 28, 2018</span></span>

<span data-ttu-id="beb0e-2324">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="beb0e-2324">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2325">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2325">Core</span></span>

* <span data-ttu-id="beb0e-2326">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="beb0e-2326">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="beb0e-2327">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="beb0e-2327">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2328">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2328">ACR</span></span>

* <span data-ttu-id="beb0e-2329">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2329">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="beb0e-2330">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2330">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2331">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2331">ACS</span></span>

* <span data-ttu-id="beb0e-2332">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2332">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="beb0e-2333">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-2333">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2334">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2334">AppService</span></span>

* <span data-ttu-id="beb0e-2335">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="beb0e-2335">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="beb0e-2336">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2336">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="beb0e-2337">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2337">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-2338">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-2338">Backup</span></span>

* <span data-ttu-id="beb0e-2339">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2339">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="beb0e-2340">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="beb0e-2340">Bot Service</span></span>

* <span data-ttu-id="beb0e-2341">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2341">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="beb0e-2342">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2342">Cognitive Services</span></span>

* <span data-ttu-id="beb0e-2343">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="beb0e-2343">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-2344">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2344">IoT</span></span>

* <span data-ttu-id="beb0e-2345">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2345">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-2346">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2346">Monitor</span></span>

* <span data-ttu-id="beb0e-2347">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="beb0e-2347">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="beb0e-2348">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2348">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2349">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2349">Network</span></span>

* <span data-ttu-id="beb0e-2350">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2350">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2351">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2351">Resource</span></span>

* <span data-ttu-id="beb0e-2352">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2352">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2353">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2353">Storage</span></span>

* <span data-ttu-id="beb0e-2354">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2354">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2355">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2355">VM</span></span>

* <span data-ttu-id="beb0e-2356">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2356">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="beb0e-2357">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2357">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="beb0e-2358">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2358">Auguest 14, 2018</span></span>

<span data-ttu-id="beb0e-2359">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="beb0e-2359">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2360">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2360">Core</span></span>

* <span data-ttu-id="beb0e-2361">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2361">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="beb0e-2362">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="beb0e-2362">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="beb0e-2363">Telemetria</span><span class="sxs-lookup"><span data-stu-id="beb0e-2363">Telemetry</span></span>

* <span data-ttu-id="beb0e-2364">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="beb0e-2364">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2365">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2365">ACR</span></span>

* <span data-ttu-id="beb0e-2366">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2366">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="beb0e-2367">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2367">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2368">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2368">ACS</span></span>

* <span data-ttu-id="beb0e-2369">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-2369">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="beb0e-2370">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2370">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="beb0e-2371">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="beb0e-2371">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="beb0e-2372">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="beb0e-2372">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="beb0e-2373">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="beb0e-2373">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="beb0e-2374">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2374">AppService</span></span>

* <span data-ttu-id="beb0e-2375">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2375">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="beb0e-2376">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="beb0e-2376">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-2377">BatchAI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2377">BatchAI</span></span>

* <span data-ttu-id="beb0e-2378">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2378">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="beb0e-2379">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2379">Container</span></span>

* <span data-ttu-id="beb0e-2380">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2380">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="beb0e-2381">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2381">IoT</span></span>

* <span data-ttu-id="beb0e-2382">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="beb0e-2382">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="beb0e-2383">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2383">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="beb0e-2384">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2384">Iot Central</span></span>

* <span data-ttu-id="beb0e-2385">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="beb0e-2385">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-2386">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-2386">KeyVault</span></span>


* <span data-ttu-id="beb0e-2387">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2387">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="beb0e-2388">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2388">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="beb0e-2389">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2389">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="beb0e-2390">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="beb0e-2390">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="beb0e-2391">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="beb0e-2391">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="beb0e-2392">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2392">Relay</span></span>

* <span data-ttu-id="beb0e-2393">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2393">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2394">Sql</span><span class="sxs-lookup"><span data-stu-id="beb0e-2394">Sql</span></span>

* <span data-ttu-id="beb0e-2395">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2395">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2396">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2396">Storage</span></span>

* <span data-ttu-id="beb0e-2397">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="beb0e-2397">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="beb0e-2398">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2398">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="beb0e-2399">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2399">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="beb0e-2400">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2400">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="beb0e-2401">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2401">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2402">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2402">VM</span></span>

* <span data-ttu-id="beb0e-2403">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2403">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="beb0e-2404">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2404">July 31, 2018</span></span>

<span data-ttu-id="beb0e-2405">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="beb0e-2405">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2406">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2406">ACR</span></span>

* <span data-ttu-id="beb0e-2407">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2407">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="beb0e-2408">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2408">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2409">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2409">ACS</span></span>

* <span data-ttu-id="beb0e-2410">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2410">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-2411">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2411">Batch</span></span>

* <span data-ttu-id="beb0e-2412">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="beb0e-2412">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2413">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2413">Container</span></span>

* <span data-ttu-id="beb0e-2414">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2414">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2415">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2415">Network</span></span>

* <span data-ttu-id="beb0e-2416">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="beb0e-2416">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="beb0e-2417">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2417">Resource</span></span>

* <span data-ttu-id="beb0e-2418">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-2418">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="beb0e-2419">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-2419">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2420">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2420">Role</span></span>

* <span data-ttu-id="beb0e-2421">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="beb0e-2421">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="beb0e-2422">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2422">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="beb0e-2423">Search</span><span class="sxs-lookup"><span data-stu-id="beb0e-2423">Search</span></span>

* <span data-ttu-id="beb0e-2424">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="beb0e-2424">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="beb0e-2425">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2425">Service Bus</span></span>

* <span data-ttu-id="beb0e-2426">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="beb0e-2426">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="beb0e-2427">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2427">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="beb0e-2428">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2428">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="beb0e-2429">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2429">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2430">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2430">Storage</span></span>

* <span data-ttu-id="beb0e-2431">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2431">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="beb0e-2432">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2432">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2433">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2433">VM</span></span>

* <span data-ttu-id="beb0e-2434">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2434">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="beb0e-2435">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2435">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="beb0e-2436">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2436">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="beb0e-2437">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="beb0e-2437">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="beb0e-2438">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2438">July 18, 2018</span></span>

<span data-ttu-id="beb0e-2439">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="beb0e-2439">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2440">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2440">Core</span></span>

* <span data-ttu-id="beb0e-2441">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2441">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="beb0e-2442">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="beb0e-2442">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="beb0e-2443">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2443">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2444">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2444">ACR</span></span>

* <span data-ttu-id="beb0e-2445">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="beb0e-2445">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="beb0e-2446">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2446">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="beb0e-2447">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2447">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="beb0e-2448">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2448">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2449">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2449">ACS</span></span>

* <span data-ttu-id="beb0e-2450">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="beb0e-2450">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2451">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2451">AppService</span></span>

* <span data-ttu-id="beb0e-2452">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="beb0e-2452">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-2453">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2453">Batch</span></span>

* <span data-ttu-id="beb0e-2454">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="beb0e-2454">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="beb0e-2455">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2455">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="beb0e-2456">Lote AI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2456">Batch AI</span></span>

* <span data-ttu-id="beb0e-2457">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2457">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2458">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2458">Container</span></span>

* <span data-ttu-id="beb0e-2459">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="beb0e-2459">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="beb0e-2460">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="beb0e-2460">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2461">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2461">Network</span></span>

* <span data-ttu-id="beb0e-2462">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2462">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="beb0e-2463">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2463">Added `network nic wait`</span></span>
* <span data-ttu-id="beb0e-2464">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2464">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="beb0e-2465">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2465">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="beb0e-2466">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2466">Resource</span></span>

* <span data-ttu-id="beb0e-2467">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2467">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="beb0e-2468">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2468">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="beb0e-2469">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2469">Added `deployment wait` command</span></span>
* <span data-ttu-id="beb0e-2470">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="beb0e-2470">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2471">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2471">SQL</span></span>

* <span data-ttu-id="beb0e-2472">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2472">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="beb0e-2473">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2473">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="beb0e-2474">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2474">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2475">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2475">Storage</span></span>

* <span data-ttu-id="beb0e-2476">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="beb0e-2476">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2477">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2477">VM</span></span>

* <span data-ttu-id="beb0e-2478">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2478">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="beb0e-2479">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2479">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="beb0e-2480">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2480">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="beb0e-2481">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2481">July 3, 2018</span></span>

<span data-ttu-id="beb0e-2482">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="beb0e-2482">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-2483">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2483">AKS</span></span>

* <span data-ttu-id="beb0e-2484">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2484">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="beb0e-2485">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2485">July 3, 2018</span></span>

<span data-ttu-id="beb0e-2486">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="beb0e-2486">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2487">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2487">Core</span></span>

* <span data-ttu-id="beb0e-2488">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2488">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2489">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2489">ACR</span></span>

* <span data-ttu-id="beb0e-2490">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2490">Added polling build status</span></span>
* <span data-ttu-id="beb0e-2491">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2491">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="beb0e-2492">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2492">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2493">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2493">ACS</span></span>

* <span data-ttu-id="beb0e-2494">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2494">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="beb0e-2495">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="beb0e-2495">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="beb0e-2496">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2496">Updated options for `aks browse` command.</span></span> <span data-ttu-id="beb0e-2497">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2497">Added `--listen-port` support</span></span>
* <span data-ttu-id="beb0e-2498">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2498">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="beb0e-2499">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="beb0e-2499">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="beb0e-2500">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2500">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2501">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2501">AppService</span></span>

* <span data-ttu-id="beb0e-2502">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2502">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="beb0e-2503">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-2503">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-2504">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-2504">Backup</span></span>

* <span data-ttu-id="beb0e-2505">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2505">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-2506">BatchAI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2506">BatchAI</span></span>

* <span data-ttu-id="beb0e-2507">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2507">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="beb0e-2508">Nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2508">Cloud</span></span>

* <span data-ttu-id="beb0e-2509">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2509">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2510">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2510">Container</span></span>

* <span data-ttu-id="beb0e-2511">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="beb0e-2511">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="beb0e-2512">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-2512">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="beb0e-2513">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="beb0e-2513">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2514">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2514">Extension</span></span>

* <span data-ttu-id="beb0e-2515">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2515">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2516">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2516">Network</span></span>

* <span data-ttu-id="beb0e-2517">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="beb0e-2517">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2518">Rdbms</span><span class="sxs-lookup"><span data-stu-id="beb0e-2518">Rdbms</span></span>

* <span data-ttu-id="beb0e-2519">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2519">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2520">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2520">Resource</span></span>

* <span data-ttu-id="beb0e-2521">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2521">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2522">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2522">VM</span></span>

* <span data-ttu-id="beb0e-2523">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="beb0e-2523">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="beb0e-2524">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2524">June 25, 2018</span></span>

<span data-ttu-id="beb0e-2525">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="beb0e-2525">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="beb0e-2526">CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2526">CLI</span></span>

* <span data-ttu-id="beb0e-2527">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2527">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="beb0e-2528">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2528">June 19, 2018</span></span>

<span data-ttu-id="beb0e-2529">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="beb0e-2529">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2530">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2530">Core</span></span>

* <span data-ttu-id="beb0e-2531">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2531">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2532">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2532">ACR</span></span>

* <span data-ttu-id="beb0e-2533">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="beb0e-2533">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="beb0e-2534">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2534">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2535">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2535">ACS</span></span>

* <span data-ttu-id="beb0e-2536">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2536">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="beb0e-2537">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2537">Added `--update` support</span></span>
* <span data-ttu-id="beb0e-2538">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2538">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="beb0e-2539">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2539">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="beb0e-2540">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2540">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="beb0e-2541">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2541">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="beb0e-2542">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2542">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="beb0e-2543">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2543">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2544">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2544">AppService</span></span>

* <span data-ttu-id="beb0e-2545">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="beb0e-2545">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="beb0e-2546">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2546">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-2547">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2547">Batch</span></span>

* <span data-ttu-id="beb0e-2548">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="beb0e-2548">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="beb0e-2549">Lote AI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2549">Batch AI</span></span>

* <span data-ttu-id="beb0e-2550">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2550">Added support for workspaces.</span></span> <span data-ttu-id="beb0e-2551">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2551">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="beb0e-2552">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2552">Added support for experiments.</span></span> <span data-ttu-id="beb0e-2553">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2553">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="beb0e-2554">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="beb0e-2554">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="beb0e-2555">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2555">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="beb0e-2556">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2556">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="beb0e-2557">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2557">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="beb0e-2558">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="beb0e-2558">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="beb0e-2559">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="beb0e-2559">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="beb0e-2560">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2560">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="beb0e-2561">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2561">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="beb0e-2562">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2562">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="beb0e-2563">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2563">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="beb0e-2564">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2564">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="beb0e-2565">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2565">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="beb0e-2566">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2566">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="beb0e-2567">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2567">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="beb0e-2568">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2568">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="beb0e-2569">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2569">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="beb0e-2570">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2570">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="beb0e-2571">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2571">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="beb0e-2572">Mapas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2572">Maps</span></span>

* <span data-ttu-id="beb0e-2573">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2573">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2574">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2574">Network</span></span>

* <span data-ttu-id="beb0e-2575">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2575">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="beb0e-2576">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2576">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="beb0e-2577">#6502</span><span class="sxs-lookup"><span data-stu-id="beb0e-2577">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="beb0e-2578">Reservas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2578">Reservations</span></span>

* <span data-ttu-id="beb0e-2579">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2579">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="beb0e-2580">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2580">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="beb0e-2581">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2581">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="beb0e-2582">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2582">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="beb0e-2583">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2583">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="beb0e-2584">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2584">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2585">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2585">Role</span></span>

* <span data-ttu-id="beb0e-2586">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2586">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2587">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2587">SQL</span></span>

* <span data-ttu-id="beb0e-2588">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2588">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2589">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2589">Storage</span></span>

* <span data-ttu-id="beb0e-2590">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="beb0e-2590">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2591">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2591">VM</span></span>

* <span data-ttu-id="beb0e-2592">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2592">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="beb0e-2593">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2593">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="beb0e-2594">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2594">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="beb0e-2595">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2595">June 13, 2018</span></span>

<span data-ttu-id="beb0e-2596">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="beb0e-2596">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2597">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2597">Core</span></span>

* <span data-ttu-id="beb0e-2598">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2598">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="beb0e-2599">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2599">June 13, 2018</span></span>

<span data-ttu-id="beb0e-2600">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="beb0e-2600">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-2601">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2601">AKS</span></span>

* <span data-ttu-id="beb0e-2602">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2602">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="beb0e-2603">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="beb0e-2603">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="beb0e-2604">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2604">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="beb0e-2605">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2605">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="beb0e-2606">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2606">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2607">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2607">AppService</span></span>

* <span data-ttu-id="beb0e-2608">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="beb0e-2608">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="beb0e-2609">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2609">June 5, 2018</span></span>

<span data-ttu-id="beb0e-2610">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="beb0e-2610">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2611">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2611">Interactive</span></span>

* <span data-ttu-id="beb0e-2612">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2612">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="beb0e-2613">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2613">June 5, 2018</span></span>

<span data-ttu-id="beb0e-2614">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="beb0e-2614">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2615">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2615">Core</span></span>

* <span data-ttu-id="beb0e-2616">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2616">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="beb0e-2617">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="beb0e-2617">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2618">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2618">ACR</span></span>

* <span data-ttu-id="beb0e-2619">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="beb0e-2619">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="beb0e-2620">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2620">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="beb0e-2621">AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2621">AKS</span></span>

* <span data-ttu-id="beb0e-2622">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="beb0e-2622">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-2623">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2623">Batch</span></span>

* <span data-ttu-id="beb0e-2624">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="beb0e-2624">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-2625">IOT</span><span class="sxs-lookup"><span data-stu-id="beb0e-2625">IOT</span></span>

* <span data-ttu-id="beb0e-2626">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="beb0e-2626">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2627">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2627">Network</span></span>

* <span data-ttu-id="beb0e-2628">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2628">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="beb0e-2629">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="beb0e-2629">Policy Insights</span></span>

* <span data-ttu-id="beb0e-2630">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2630">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="beb0e-2631">ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2631">ARM</span></span>

* <span data-ttu-id="beb0e-2632">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2632">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2633">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2633">SQL</span></span>

* <span data-ttu-id="beb0e-2634">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2634">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="beb0e-2635">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2635">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="beb0e-2636">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2636">Storage</span></span>

* <span data-ttu-id="beb0e-2637">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2637">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2638">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2638">VM</span></span>

* <span data-ttu-id="beb0e-2639">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2639">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="beb0e-2640">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2640">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="beb0e-2641">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2641">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="beb0e-2642">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2642">May 22, 2018</span></span>

<span data-ttu-id="beb0e-2643">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="beb0e-2643">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2644">Core</span></span>

* <span data-ttu-id="beb0e-2645">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2645">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2646">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2646">ACS</span></span>

* <span data-ttu-id="beb0e-2647">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2647">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="beb0e-2648">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-2648">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2649">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2649">AppService</span></span>

* <span data-ttu-id="beb0e-2650">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="beb0e-2650">Improved generic update commands</span></span>
* <span data-ttu-id="beb0e-2651">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2651">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2652">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2652">Container</span></span>

* <span data-ttu-id="beb0e-2653">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="beb0e-2653">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="beb0e-2654">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2654">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2655">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2655">Extension</span></span>

* <span data-ttu-id="beb0e-2656">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2656">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2657">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2657">Interactive</span></span>

* <span data-ttu-id="beb0e-2658">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="beb0e-2658">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="beb0e-2659">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="beb0e-2659">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-2660">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-2660">KeyVault</span></span>

* <span data-ttu-id="beb0e-2661">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-2661">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2662">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2662">Network</span></span>

* <span data-ttu-id="beb0e-2663">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2663">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="beb0e-2664">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2664">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2665">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2665">SQL</span></span>

* <span data-ttu-id="beb0e-2666">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2666">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="beb0e-2667">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2667">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="beb0e-2668">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2668">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="beb0e-2669">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb0e-2669">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="beb0e-2670">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2670">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="beb0e-2671">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2671">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="beb0e-2672">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2672">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="beb0e-2673">`edition`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2673">`edition`.</span></span> <span data-ttu-id="beb0e-2674">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2674">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="beb0e-2675">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2675">`elasticPoolName`.</span></span> <span data-ttu-id="beb0e-2676">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2676">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="beb0e-2677">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2677">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="beb0e-2678">`edition`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2678">`edition`.</span></span> <span data-ttu-id="beb0e-2679">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2679">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="beb0e-2680">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2680">`dtu`.</span></span> <span data-ttu-id="beb0e-2681">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2681">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="beb0e-2682">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2682">`databaseDtuMin`.</span></span> <span data-ttu-id="beb0e-2683">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2683">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="beb0e-2684">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2684">`databaseDtuMax`.</span></span> <span data-ttu-id="beb0e-2685">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2685">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="beb0e-2686">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2686">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="beb0e-2687">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2687">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2688">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2688">Storage</span></span>

* <span data-ttu-id="beb0e-2689">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2689">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="beb0e-2690">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2690">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2691">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2691">VM</span></span>

* <span data-ttu-id="beb0e-2692">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2692">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="beb0e-2693">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2693">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="beb0e-2694">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2694">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="beb0e-2695">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="beb0e-2695">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="beb0e-2696">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2696">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="beb0e-2697">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2697">May 7, 2018</span></span>

<span data-ttu-id="beb0e-2698">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="beb0e-2698">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2699">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2699">Core</span></span>

* <span data-ttu-id="beb0e-2700">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2700">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="beb0e-2701">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2701">Added limited support for positional arguments</span></span>
* <span data-ttu-id="beb0e-2702">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2702">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="beb0e-2703">#5591</span><span class="sxs-lookup"><span data-stu-id="beb0e-2703">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="beb0e-2704">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2704">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="beb0e-2705">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="beb0e-2705">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="beb0e-2706">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2706">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="beb0e-2707">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2707">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="beb0e-2708">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="beb0e-2708">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2709">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2709">ACR</span></span>

* <span data-ttu-id="beb0e-2710">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2710">Added ACR Build commands</span></span>
* <span data-ttu-id="beb0e-2711">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-2711">Improved resource not found error messages</span></span>
* <span data-ttu-id="beb0e-2712">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="beb0e-2712">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="beb0e-2713">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2713">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="beb0e-2714">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2714">Improved repository commands error messages</span></span>
* <span data-ttu-id="beb0e-2715">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2715">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2716">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2716">ACS</span></span>

* <span data-ttu-id="beb0e-2717">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-2717">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="beb0e-2718">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2718">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="beb0e-2719">AMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2719">AMS</span></span>

* <span data-ttu-id="beb0e-2720">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-2720">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2721">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2721">Appservice</span></span>

* <span data-ttu-id="beb0e-2722">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2722">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="beb0e-2723">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2723">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="beb0e-2724">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-2724">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="beb0e-2725">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="beb0e-2725">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="beb0e-2726">Lote AI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2726">Batch AI</span></span>

* <span data-ttu-id="beb0e-2727">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-2727">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="beb0e-2728">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2728">Cognitive Services</span></span>

* <span data-ttu-id="beb0e-2729">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2729">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-2730">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2730">Consumption</span></span>

* <span data-ttu-id="beb0e-2731">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2731">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2732">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2732">Container</span></span>

* <span data-ttu-id="beb0e-2733">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-2733">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="beb0e-2734">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2734">Cosmos DB</span></span>

* <span data-ttu-id="beb0e-2735">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2735">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="beb0e-2736">DMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2736">DMS</span></span>

* <span data-ttu-id="beb0e-2737">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-2737">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2738">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2738">Extension</span></span>

* <span data-ttu-id="beb0e-2739">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2739">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2740">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2740">Interactive</span></span>

* <span data-ttu-id="beb0e-2741">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2741">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="beb0e-2742">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="beb0e-2742">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="beb0e-2743">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-2743">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="beb0e-2744">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-2744">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="beb0e-2745">Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-2745">Lab</span></span>

* <span data-ttu-id="beb0e-2746">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2746">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2747">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2747">Network</span></span>

* <span data-ttu-id="beb0e-2748">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2748">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="beb0e-2749">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-2749">Profile</span></span>

* <span data-ttu-id="beb0e-2750">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="beb0e-2750">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="beb0e-2751">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2751">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="beb0e-2752">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2752">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-2753">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-2753">Redis</span></span>

* <span data-ttu-id="beb0e-2754">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2754">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="beb0e-2755">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2755">Deprecated `redis list-all`.</span></span> <span data-ttu-id="beb0e-2756">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2756">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="beb0e-2757">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2757">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="beb0e-2758">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2758">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2759">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2759">Role</span></span>

* <span data-ttu-id="beb0e-2760">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2760">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2761">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2761">Storage</span></span>

* <span data-ttu-id="beb0e-2762">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2762">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="beb0e-2763">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="beb0e-2763">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="beb0e-2764">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2764">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="beb0e-2765">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="beb0e-2765">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="beb0e-2766">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="beb0e-2766">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2767">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2767">VM</span></span>

* <span data-ttu-id="beb0e-2768">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2768">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="beb0e-2769">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-2769">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="beb0e-2770">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2770">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="beb0e-2771">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2771">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="beb0e-2772">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2772">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="beb0e-2773">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="beb0e-2773">Added write accelerator support</span></span>
* <span data-ttu-id="beb0e-2774">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2774">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="beb0e-2775">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="beb0e-2775">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="beb0e-2776">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="beb0e-2776">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="beb0e-2777">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2777">April 10, 2018</span></span>

<span data-ttu-id="beb0e-2778">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="beb0e-2778">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2779">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2779">ACR</span></span>

* <span data-ttu-id="beb0e-2780">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="beb0e-2780">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2781">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2781">ACS</span></span>

* <span data-ttu-id="beb0e-2782">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2782">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2783">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2783">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="beb0e-2785">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-2785">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-2786">BatchAI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2786">BatchAI</span></span>

* <span data-ttu-id="beb0e-2787">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-2787">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="beb0e-2788">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-2788">Job level mounting</span></span>
  - <span data-ttu-id="beb0e-2789">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2789">Environment variables with secret values</span></span>
  - <span data-ttu-id="beb0e-2790">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="beb0e-2790">Performance counters settings</span></span>
  - <span data-ttu-id="beb0e-2791">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-2791">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="beb0e-2792">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="beb0e-2792">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="beb0e-2793">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="beb0e-2793">Usage and limits reporting</span></span>
  - <span data-ttu-id="beb0e-2794">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2794">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="beb0e-2795">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2795">Support for custom images</span></span>
  - <span data-ttu-id="beb0e-2796">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="beb0e-2796">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="beb0e-2797">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-2797">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="beb0e-2798">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="beb0e-2798">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="beb0e-2799">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-2799">National clouds are supported</span></span>
* <span data-ttu-id="beb0e-2800">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="beb0e-2800">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="beb0e-2801">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="beb0e-2801">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="beb0e-2802">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-2802">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="beb0e-2803">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2803">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="beb0e-2804">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2804">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="beb0e-2805">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2805">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="beb0e-2806">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2806">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="beb0e-2807">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2807">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="beb0e-2808">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="beb0e-2808">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="beb0e-2809">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2809">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="beb0e-2810">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-2810">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="beb0e-2811">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2811">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="beb0e-2812">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2812">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="beb0e-2813">Cobrança</span><span class="sxs-lookup"><span data-stu-id="beb0e-2813">Billing</span></span>

* <span data-ttu-id="beb0e-2814">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="beb0e-2814">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-2815">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2815">Consumption</span></span>

* <span data-ttu-id="beb0e-2816">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2816">Added `marketplace` commands</span></span>
* <span data-ttu-id="beb0e-2817">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2817">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="beb0e-2818">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2818">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="beb0e-2819">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2819">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="beb0e-2820">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2820">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="beb0e-2821">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2821">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2822">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2822">Container</span></span>

* <span data-ttu-id="beb0e-2823">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2823">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="beb0e-2824">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2824">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2825">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2825">Extension</span></span>

* <span data-ttu-id="beb0e-2826">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="beb0e-2826">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2827">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2827">Interactive</span></span>

* <span data-ttu-id="beb0e-2828">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2828">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="beb0e-2829">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-2829">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="beb0e-2830">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2830">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2831">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2831">Network</span></span>

* <span data-ttu-id="beb0e-2832">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2832">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="beb0e-2833">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2833">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="beb0e-2834">#4910</span><span class="sxs-lookup"><span data-stu-id="beb0e-2834">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="beb0e-2835">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2835">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="beb0e-2836">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2836">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="beb0e-2837">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2837">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="beb0e-2838">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2838">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="beb0e-2839">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2839">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-2840">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-2840">Profile</span></span>

* <span data-ttu-id="beb0e-2841">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2841">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="beb0e-2842">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2842">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2843">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2843">RDBMS</span></span>

* <span data-ttu-id="beb0e-2844">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2844">Added `georestore` command</span></span>
* <span data-ttu-id="beb0e-2845">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2845">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2846">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2846">Resource</span></span>

* <span data-ttu-id="beb0e-2847">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2847">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="beb0e-2848">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2848">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2849">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2849">SQL</span></span>

* <span data-ttu-id="beb0e-2850">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2850">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2851">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2851">Storage</span></span>

* <span data-ttu-id="beb0e-2852">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2852">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2853">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2853">VM</span></span>

* <span data-ttu-id="beb0e-2854">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2854">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="beb0e-2855">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2855">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="beb0e-2857">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2857">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="beb0e-2858">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2858">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="beb0e-2859">#5718</span><span class="sxs-lookup"><span data-stu-id="beb0e-2859">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="beb0e-2860">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="beb0e-2860">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="beb0e-2861">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2861">March 27, 2018</span></span>

<span data-ttu-id="beb0e-2862">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="beb0e-2862">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2863">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2863">Core</span></span>

* <span data-ttu-id="beb0e-2864">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="beb0e-2864">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2865">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2865">ACS</span></span>

* <span data-ttu-id="beb0e-2866">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="beb0e-2866">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2867">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2867">Appservice</span></span>

* <span data-ttu-id="beb0e-2868">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2868">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="beb0e-2869">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2869">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-2870">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-2870">Backup</span></span>

* <span data-ttu-id="beb0e-2871">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2871">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="beb0e-2872">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-2872">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="beb0e-2873">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2873">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="beb0e-2874">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2874">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2875">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2875">Container</span></span>

* <span data-ttu-id="beb0e-2876">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-2876">Added `container exec` command.</span></span> <span data-ttu-id="beb0e-2877">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="beb0e-2877">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="beb0e-2878">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2878">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2879">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2879">Extension</span></span>

* <span data-ttu-id="beb0e-2880">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-2880">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="beb0e-2881">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2881">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="beb0e-2882">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2882">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2883">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2883">Interactive</span></span>

* <span data-ttu-id="beb0e-2884">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2884">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="beb0e-2885">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2885">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="beb0e-2886">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2886">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="beb0e-2887">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="beb0e-2887">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="beb0e-2888">Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-2888">Lab</span></span>

* <span data-ttu-id="beb0e-2889">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2889">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-2890">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2890">Monitor</span></span>

* <span data-ttu-id="beb0e-2891">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2891">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="beb0e-2892">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="beb0e-2892">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="beb0e-2893">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2893">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2894">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2894">Network</span></span>

* <span data-ttu-id="beb0e-2895">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="beb0e-2895">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-2896">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-2896">Profile</span></span>

* <span data-ttu-id="beb0e-2897">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2897">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2898">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2898">RDBMS</span></span>

* <span data-ttu-id="beb0e-2899">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-2899">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2900">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2900">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="beb0e-2902">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2902">Role</span></span>

* <span data-ttu-id="beb0e-2903">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2903">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="beb0e-2904">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="beb0e-2904">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="beb0e-2905">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2905">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="beb0e-2906">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2906">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="beb0e-2907">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2907">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2908">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2908">Storage</span></span>

* <span data-ttu-id="beb0e-2909">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="beb0e-2909">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="beb0e-2910">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="beb0e-2910">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2911">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2911">VM</span></span>

* <span data-ttu-id="beb0e-2912">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="beb0e-2912">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="beb0e-2913">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2913">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="beb0e-2914">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2914">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="beb0e-2915">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="beb0e-2915">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="beb0e-2916">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2916">March 13, 2018</span></span>

<span data-ttu-id="beb0e-2917">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="beb0e-2917">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-2918">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-2918">ACR</span></span>

* <span data-ttu-id="beb0e-2919">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2919">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="beb0e-2920">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2920">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="beb0e-2921">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2921">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2922">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2922">ACS</span></span>

* <span data-ttu-id="beb0e-2923">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="beb0e-2923">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="beb0e-2924">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="beb0e-2924">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="beb0e-2925">Supervisor</span><span class="sxs-lookup"><span data-stu-id="beb0e-2925">Advisor</span></span>

* <span data-ttu-id="beb0e-2926">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2926">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="beb0e-2927">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2927">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="beb0e-2928">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2928">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="beb0e-2929">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2929">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="beb0e-2930">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2930">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2931">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2931">Appservice</span></span>

* <span data-ttu-id="beb0e-2932">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2932">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="beb0e-2933">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2933">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="beb0e-2934">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2934">Eventhubs</span></span>

* <span data-ttu-id="beb0e-2935">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2935">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-2936">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2936">Extension</span></span>

* <span data-ttu-id="beb0e-2937">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="beb0e-2937">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-2938">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2938">Interactive</span></span>

* <span data-ttu-id="beb0e-2939">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-2939">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="beb0e-2940">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2940">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="beb0e-2941">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="beb0e-2941">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="beb0e-2942">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="beb0e-2942">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-2943">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2943">Monitor</span></span>

* <span data-ttu-id="beb0e-2944">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2944">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="beb0e-2945">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2945">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="beb0e-2946">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2946">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="beb0e-2947">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2947">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2948">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2948">Network</span></span>

* <span data-ttu-id="beb0e-2949">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2949">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="beb0e-2950">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="beb0e-2950">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="beb0e-2951">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-2951">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="beb0e-2952">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2952">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-2953">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-2953">Profile</span></span>

* <span data-ttu-id="beb0e-2954">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2954">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="beb0e-2955">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2955">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-2956">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2956">RDBMS</span></span>

* <span data-ttu-id="beb0e-2957">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="beb0e-2957">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="beb0e-2958">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2958">Service Bus</span></span>

* <span data-ttu-id="beb0e-2959">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-2959">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2960">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2960">Storage</span></span>

* <span data-ttu-id="beb0e-2961">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-2961">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="beb0e-2962">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="beb0e-2962">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2963">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2963">VM</span></span>

* <span data-ttu-id="beb0e-2964">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="beb0e-2964">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="beb0e-2965">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2965">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="beb0e-2966">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2966">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="beb0e-2967">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="beb0e-2967">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="beb0e-2968">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-2968">February 27, 2018</span></span>

<span data-ttu-id="beb0e-2969">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="beb0e-2969">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-2970">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2970">Core</span></span>

* <span data-ttu-id="beb0e-2971">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="beb0e-2971">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="beb0e-2972">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="beb0e-2972">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="beb0e-2973">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2973">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-2974">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-2974">ACS</span></span>

* <span data-ttu-id="beb0e-2975">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-2975">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="beb0e-2976">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2976">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="beb0e-2977">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2977">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="beb0e-2978">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2978">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-2979">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-2979">Appservice</span></span>

* <span data-ttu-id="beb0e-2980">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="beb0e-2980">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="beb0e-2981">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="beb0e-2981">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="beb0e-2982">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2982">Cognitive Services</span></span>

* <span data-ttu-id="beb0e-2983">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-2983">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-2984">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-2984">Consumption</span></span>

* <span data-ttu-id="beb0e-2985">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="beb0e-2985">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="beb0e-2986">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="beb0e-2986">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-2987">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-2987">Container</span></span>

* <span data-ttu-id="beb0e-2988">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="beb0e-2988">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-2989">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-2989">Network</span></span>

* <span data-ttu-id="beb0e-2990">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2990">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-2991">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-2991">Resource</span></span>

* <span data-ttu-id="beb0e-2992">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="beb0e-2992">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-2993">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-2993">Role</span></span>

* <span data-ttu-id="beb0e-2994">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-2994">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-2995">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-2995">SQL</span></span>

* <span data-ttu-id="beb0e-2996">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-2996">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-2997">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-2997">Storage</span></span>

* <span data-ttu-id="beb0e-2998">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-2998">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-2999">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-2999">VM</span></span>

* <span data-ttu-id="beb0e-3000">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3000">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="beb0e-3001">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-3001">February 13, 2018</span></span>

<span data-ttu-id="beb0e-3002">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="beb0e-3002">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3003">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3003">Core</span></span>

* <span data-ttu-id="beb0e-3004">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-3004">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3005">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3005">ACS</span></span>

* <span data-ttu-id="beb0e-3006">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3006">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="beb0e-3007">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3007">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="beb0e-3008">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3008">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="beb0e-3009">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3009">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="beb0e-3010">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3010">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="beb0e-3011">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3011">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="beb0e-3012">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3012">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="beb0e-3013">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3013">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3014">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3014">Appservice</span></span>

* <span data-ttu-id="beb0e-3015">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="beb0e-3015">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="beb0e-3016">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3016">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-3017">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3017">CDN</span></span>

* <span data-ttu-id="beb0e-3018">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3018">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-3019">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3019">Container</span></span>

* <span data-ttu-id="beb0e-3020">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="beb0e-3020">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="beb0e-3021">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3021">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-3022">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3022">CosmosDB</span></span>

* <span data-ttu-id="beb0e-3023">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3023">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-3024">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3024">Extension</span></span>

* <span data-ttu-id="beb0e-3025">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3025">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="beb0e-3026">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3026">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="beb0e-3027">Comentários</span><span class="sxs-lookup"><span data-stu-id="beb0e-3027">Feedback</span></span>

* <span data-ttu-id="beb0e-3028">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="beb0e-3028">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-3029">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3029">Interactive</span></span>

* <span data-ttu-id="beb0e-3030">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="beb0e-3030">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="beb0e-3031">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3031">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-3032">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3032">IoT</span></span>

* <span data-ttu-id="beb0e-3033">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3033">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="beb0e-3034">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3034">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="beb0e-3035">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3035">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="beb0e-3036">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="beb0e-3036">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3037">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3037">Monitor</span></span>

* <span data-ttu-id="beb0e-3038">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3038">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3039">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3039">Network</span></span>

* <span data-ttu-id="beb0e-3040">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3040">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="beb0e-3041">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3041">Profile</span></span>

* <span data-ttu-id="beb0e-3042">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3042">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3043">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3043">Resource</span></span>

* <span data-ttu-id="beb0e-3044">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3044">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-3045">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3045">Role</span></span>

* <span data-ttu-id="beb0e-3046">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3046">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3047">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3047">SQL</span></span>

* <span data-ttu-id="beb0e-3048">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3048">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="beb0e-3049">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3049">Added `sql db rename`</span></span>
* <span data-ttu-id="beb0e-3050">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="beb0e-3050">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3051">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3051">Storage</span></span>

* <span data-ttu-id="beb0e-3052">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="beb0e-3052">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3053">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3053">VM</span></span>

* <span data-ttu-id="beb0e-3054">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3054">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="beb0e-3055">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-3055">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="beb0e-3056">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3056">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="beb0e-3057">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-3057">January 31, 2018</span></span>

<span data-ttu-id="beb0e-3058">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="beb0e-3058">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3059">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3059">Core</span></span>

* <span data-ttu-id="beb0e-3060">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-3060">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="beb0e-3061">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="beb0e-3061">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="beb0e-3062">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3062">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="beb0e-3063">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="beb0e-3063">Use `--verbose` to see</span></span>
* <span data-ttu-id="beb0e-3064">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="beb0e-3064">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3065">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3065">ACS</span></span>

* <span data-ttu-id="beb0e-3066">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-3066">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="beb0e-3067">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3067">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3068">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3068">Appservice</span></span>

* <span data-ttu-id="beb0e-3069">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3069">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="beb0e-3070">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="beb0e-3070">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-3071">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3071">CDN</span></span>

* <span data-ttu-id="beb0e-3072">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3072">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-3073">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3073">CosmosDB</span></span>

* <span data-ttu-id="beb0e-3074">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="beb0e-3074">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-3075">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3075">Interactive</span></span>

* <span data-ttu-id="beb0e-3076">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="beb0e-3076">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3077">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3077">Network</span></span>

* <span data-ttu-id="beb0e-3078">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3078">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="beb0e-3079">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3079">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="beb0e-3080">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3080">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="beb0e-3081">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3081">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="beb0e-3082">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3082">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="beb0e-3083">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3083">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="beb0e-3084">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3084">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="beb0e-3085">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="beb0e-3085">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="beb0e-3086">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3086">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="beb0e-3087">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3087">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3088">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3088">Profile</span></span>

* <span data-ttu-id="beb0e-3089">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="beb0e-3089">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3090">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3090">Resource</span></span>

* <span data-ttu-id="beb0e-3091">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3091">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3092">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3092">Storage</span></span>

* <span data-ttu-id="beb0e-3093">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="beb0e-3093">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="beb0e-3094">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="beb0e-3094">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="beb0e-3095">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3095">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="beb0e-3096">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3096">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="beb0e-3097">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="beb0e-3097">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3098">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3098">VM</span></span>

* <span data-ttu-id="beb0e-3099">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-3099">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="beb0e-3100">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3100">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="beb0e-3101">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3101">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="beb0e-3102">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3102">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="beb0e-3103">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="beb0e-3103">January 17, 2018</span></span>

<span data-ttu-id="beb0e-3104">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="beb0e-3104">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-3105">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3105">ACR</span></span>

* <span data-ttu-id="beb0e-3106">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-3106">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="beb0e-3107">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="beb0e-3107">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3108">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3108">ACS</span></span>

* <span data-ttu-id="beb0e-3109">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3109">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="beb0e-3110">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3110">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3111">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3111">Appservice</span></span>

* <span data-ttu-id="beb0e-3112">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3112">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="beb0e-3113">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3113">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="beb0e-3114">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3114">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-3115">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-3115">Backup</span></span>

* <span data-ttu-id="beb0e-3116">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="beb0e-3116">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="beb0e-3117">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3117">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="beb0e-3118">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3118">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="beb0e-3119">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="beb0e-3119">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="beb0e-3120">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3120">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-3121">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3121">Batch</span></span>

* <span data-ttu-id="beb0e-3122">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="beb0e-3122">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="beb0e-3123">Nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3123">Cloud</span></span>

* <span data-ttu-id="beb0e-3124">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3124">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-3125">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3125">Consumption</span></span>

* <span data-ttu-id="beb0e-3126">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3126">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="beb0e-3127">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3127">Event Grid</span></span>

* <span data-ttu-id="beb0e-3128">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3128">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="beb0e-3129">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3129">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="beb0e-3130">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3130">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="beb0e-3131">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3131">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="beb0e-3132">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3132">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="beb0e-3133">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3133">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="beb0e-3134">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3134">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="beb0e-3135">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3135">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-3136">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3136">Interactive</span></span>

* <span data-ttu-id="beb0e-3137">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="beb0e-3137">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="beb0e-3138">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="beb0e-3138">Fixed errors on startup</span></span>
* <span data-ttu-id="beb0e-3139">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3139">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-3140">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3140">IoT</span></span>

* <span data-ttu-id="beb0e-3141">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3141">Added support for device provisioning service</span></span>
* <span data-ttu-id="beb0e-3142">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-3142">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="beb0e-3143">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3143">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3144">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3144">Monitor</span></span>

* <span data-ttu-id="beb0e-3145">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3145">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="beb0e-3146">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3146">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="beb0e-3147">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3147">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3148">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3148">Network</span></span>

* <span data-ttu-id="beb0e-3149">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3149">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="beb0e-3150">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3150">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3151">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3151">Profile</span></span>

* <span data-ttu-id="beb0e-3152">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-3152">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-3153">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3153">Role</span></span>

* <span data-ttu-id="beb0e-3154">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3154">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="beb0e-3155">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-3155">Service Fabric</span></span>

* <span data-ttu-id="beb0e-3156">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="beb0e-3156">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="beb0e-3157">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3157">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3158">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3158">VM</span></span>

* <span data-ttu-id="beb0e-3159">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3159">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="beb0e-3160">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="beb0e-3160">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="beb0e-3161">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="beb0e-3161">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="beb0e-3162">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="beb0e-3162">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="beb0e-3163">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3163">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="beb0e-3164">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3164">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="beb0e-3165">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3165">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="beb0e-3166">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3166">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="beb0e-3167">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3167">December 19, 2017</span></span>

<span data-ttu-id="beb0e-3168">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="beb0e-3168">Version 2.0.23</span></span>

* <span data-ttu-id="beb0e-3169">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="beb0e-3169">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-3170">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3170">Container</span></span>

* <span data-ttu-id="beb0e-3171">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3171">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3172">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3172">Network</span></span>

* <span data-ttu-id="beb0e-3173">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3173">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="beb0e-3174">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3174">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3175">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3175">Storage</span></span>

* <span data-ttu-id="beb0e-3176">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="beb0e-3176">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3177">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3177">VM</span></span>

* <span data-ttu-id="beb0e-3178">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3178">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="beb0e-3179">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3179">December 5, 2017</span></span>

<span data-ttu-id="beb0e-3180">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="beb0e-3180">Version 2.0.22</span></span>

* <span data-ttu-id="beb0e-3181">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3181">Removed `az component` commands.</span></span> <span data-ttu-id="beb0e-3182">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3182">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3183">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3183">Core</span></span>
* <span data-ttu-id="beb0e-3184">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="beb0e-3184">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="beb0e-3185">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3185">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3186">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3186">ACS</span></span>

* <span data-ttu-id="beb0e-3187">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3187">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="beb0e-3188">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3188">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="beb0e-3189">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3189">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="beb0e-3190">Supervisor</span><span class="sxs-lookup"><span data-stu-id="beb0e-3190">Advisor</span></span>

* <span data-ttu-id="beb0e-3191">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-3191">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3192">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3192">Appservice</span></span>

* <span data-ttu-id="beb0e-3193">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3193">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="beb0e-3194">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3194">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="beb0e-3195">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3195">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="beb0e-3196">Consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3196">Consumption</span></span>

* <span data-ttu-id="beb0e-3197">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3197">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-3198">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3198">Container</span></span>

* <span data-ttu-id="beb0e-3199">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3199">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3200">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3200">Monitor</span></span>

* <span data-ttu-id="beb0e-3201">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3201">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3202">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3202">Resource</span></span>

* <span data-ttu-id="beb0e-3203">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3203">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-3204">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3204">Role</span></span>

* <span data-ttu-id="beb0e-3205">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3205">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="beb0e-3206">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="beb0e-3206">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="beb0e-3207">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3207">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3208">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3208">SQL</span></span>

* <span data-ttu-id="beb0e-3209">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3209">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="beb0e-3210">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3210">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3211">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3211">VM</span></span>

* <span data-ttu-id="beb0e-3212">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3212">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="beb0e-3213">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3213">November 14, 2017</span></span>

<span data-ttu-id="beb0e-3214">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="beb0e-3214">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-3215">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3215">ACR</span></span>

* <span data-ttu-id="beb0e-3216">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="beb0e-3216">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="beb0e-3217">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3217">ACS</span></span>

* <span data-ttu-id="beb0e-3218">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3218">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="beb0e-3219">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3219">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="beb0e-3220">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3220">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="beb0e-3221">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-3221">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="beb0e-3222">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="beb0e-3222">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3223">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3223">Appservice</span></span>

* <span data-ttu-id="beb0e-3224">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="beb0e-3224">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="beb0e-3225">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3225">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="beb0e-3226">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3226">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="beb0e-3227">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3227">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="beb0e-3228">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-3228">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="beb0e-3229">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3229">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-3230">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3230">Batch</span></span>

* <span data-ttu-id="beb0e-3231">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3231">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-3232">Batchai</span><span class="sxs-lookup"><span data-stu-id="beb0e-3232">Batchai</span></span>

* <span data-ttu-id="beb0e-3233">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3233">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="beb0e-3234">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3234">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="beb0e-3235">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3235">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="beb0e-3236">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3236">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="beb0e-3237">Nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3237">Cloud</span></span>

* <span data-ttu-id="beb0e-3238">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="beb0e-3238">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-3239">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3239">Container</span></span>

* <span data-ttu-id="beb0e-3240">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3240">Added support to open multiple ports</span></span>
* <span data-ttu-id="beb0e-3241">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3241">Added container group restart policy</span></span>
* <span data-ttu-id="beb0e-3242">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="beb0e-3242">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="beb0e-3243">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3243">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="beb0e-3244">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-3244">Data Lake Analytics</span></span>

* <span data-ttu-id="beb0e-3245">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3245">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="beb0e-3246">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3246">Data Lake Store</span></span>

* <span data-ttu-id="beb0e-3247">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3247">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-3248">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3248">Extension</span></span>

* <span data-ttu-id="beb0e-3249">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="beb0e-3249">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="beb0e-3250">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="beb0e-3250">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-3251">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3251">IoT</span></span>

* <span data-ttu-id="beb0e-3252">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3252">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3253">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3253">Monitor</span></span>

* <span data-ttu-id="beb0e-3254">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3254">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3255">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3255">Network</span></span>

* <span data-ttu-id="beb0e-3256">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="beb0e-3256">Added support for CAA DNS records</span></span>
* <span data-ttu-id="beb0e-3257">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3257">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="beb0e-3258">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3258">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="beb0e-3259">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3259">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="beb0e-3260">Reservas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3260">Reservations</span></span>

* <span data-ttu-id="beb0e-3261">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-3261">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3262">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3262">Resource</span></span>

* <span data-ttu-id="beb0e-3263">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3263">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3264">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3264">SQL</span></span>

* <span data-ttu-id="beb0e-3265">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3265">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3266">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3266">Storage</span></span>

* <span data-ttu-id="beb0e-3267">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3267">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="beb0e-3268">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="beb0e-3268">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="beb0e-3269">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3269">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="beb0e-3270">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3270">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="beb0e-3271">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3271">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="beb0e-3272">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3272">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="beb0e-3273">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3273">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3274">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3274">VM</span></span>

* <span data-ttu-id="beb0e-3275">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3275">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="beb0e-3276">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="beb0e-3276">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="beb0e-3277">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3277">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="beb0e-3278">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3278">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="beb0e-3279">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3279">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="beb0e-3280">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3280">October 24, 2017</span></span>

<span data-ttu-id="beb0e-3281">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="beb0e-3281">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3282">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3282">Core</span></span>

* <span data-ttu-id="beb0e-3283">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3283">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-3284">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3284">ACR</span></span>

* <span data-ttu-id="beb0e-3285">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3285">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="beb0e-3286">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3286">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="beb0e-3287">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="beb0e-3287">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3288">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3288">ACS</span></span>

* <span data-ttu-id="beb0e-3289">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3289">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="beb0e-3290">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="beb0e-3290">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3291">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3291">Appservice</span></span>

* <span data-ttu-id="beb0e-3292">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3292">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="beb0e-3293">Componente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3293">Component</span></span>

* <span data-ttu-id="beb0e-3294">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="beb0e-3294">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3295">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3295">Monitor</span></span>

* <span data-ttu-id="beb0e-3296">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3296">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3297">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3297">Resource</span></span>

* <span data-ttu-id="beb0e-3298">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3298">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="beb0e-3299">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3299">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3300">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3300">VM</span></span>

* <span data-ttu-id="beb0e-3301">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3301">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="beb0e-3302">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3302">October 9, 2017</span></span>

<span data-ttu-id="beb0e-3303">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="beb0e-3303">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3304">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3304">Core</span></span>

* <span data-ttu-id="beb0e-3305">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="beb0e-3305">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3306">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3306">Appservice</span></span>

* <span data-ttu-id="beb0e-3307">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3307">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-3308">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3308">Batch</span></span>

* <span data-ttu-id="beb0e-3309">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-3309">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="beb0e-3310">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="beb0e-3310">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="beb0e-3311">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3311">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="beb0e-3312">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3312">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="beb0e-3313">Batchai</span><span class="sxs-lookup"><span data-stu-id="beb0e-3313">Batchai</span></span>

* <span data-ttu-id="beb0e-3314">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3314">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-3315">Keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-3315">Keyvault</span></span>

* <span data-ttu-id="beb0e-3316">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3316">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="beb0e-3317">(#4448)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3317">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="beb0e-3318">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3318">Network</span></span>

* <span data-ttu-id="beb0e-3319">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="beb0e-3319">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="beb0e-3320">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3320">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3321">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3321">Resource</span></span>

* <span data-ttu-id="beb0e-3322">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3322">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="beb0e-3323">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-3323">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="beb0e-3324">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3324">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="beb0e-3325">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3325">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3326">Sql</span><span class="sxs-lookup"><span data-stu-id="beb0e-3326">Sql</span></span>

* <span data-ttu-id="beb0e-3327">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="beb0e-3327">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="beb0e-3328">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3328">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="beb0e-3329">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3329">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3330">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3330">Storage</span></span>

* <span data-ttu-id="beb0e-3331">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3331">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3332">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3332">Vm</span></span>

* <span data-ttu-id="beb0e-3333">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3333">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="beb0e-3334">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3334">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="beb0e-3335">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3335">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="beb0e-3336">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3336">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="beb0e-3337">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3337">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="beb0e-3338">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3338">September 22, 2017</span></span>

<span data-ttu-id="beb0e-3339">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="beb0e-3339">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3340">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3340">Resource</span></span>

* <span data-ttu-id="beb0e-3341">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3341">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="beb0e-3342">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="beb0e-3342">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="beb0e-3343">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3343">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="beb0e-3344">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3344">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3345">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3345">Network</span></span>

* <span data-ttu-id="beb0e-3346">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3346">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="beb0e-3347">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3347">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="beb0e-3348">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3348">Added `asg` application security group commands</span></span>
* <span data-ttu-id="beb0e-3349">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3349">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="beb0e-3350">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3350">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="beb0e-3351">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3351">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="beb0e-3352">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3352">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3353">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3353">Storage</span></span>

* <span data-ttu-id="beb0e-3354">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="beb0e-3354">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="beb0e-3355">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3355">Eventgrid</span></span>

* <span data-ttu-id="beb0e-3356">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="beb0e-3356">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3357">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3357">SQL</span></span>

* <span data-ttu-id="beb0e-3358">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3358">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="beb0e-3359">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3359">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="beb0e-3360">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3360">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-3361">Keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-3361">Keyvault</span></span>

* <span data-ttu-id="beb0e-3362">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="beb0e-3362">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3363">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3363">VM</span></span>

* <span data-ttu-id="beb0e-3364">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3364">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="beb0e-3365">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="beb0e-3365">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="beb0e-3366">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3366">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="beb0e-3367">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3367">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="beb0e-3368">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3368">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="beb0e-3369">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3369">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3370">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3370">ACS</span></span>

* <span data-ttu-id="beb0e-3371">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3371">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3372">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3372">Appservice</span></span>

* <span data-ttu-id="beb0e-3373">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3373">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="beb0e-3374">Backup</span><span class="sxs-lookup"><span data-stu-id="beb0e-3374">Backup</span></span>

* <span data-ttu-id="beb0e-3375">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-3375">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="beb0e-3376">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3376">September 11, 2017</span></span>

<span data-ttu-id="beb0e-3377">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="beb0e-3377">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="beb0e-3378">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3378">Core</span></span>

* <span data-ttu-id="beb0e-3379">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="beb0e-3379">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="beb0e-3380">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3380">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3381">Acs</span><span class="sxs-lookup"><span data-stu-id="beb0e-3381">Acs</span></span>

* <span data-ttu-id="beb0e-3382">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3382">Added `acs list-locations` command</span></span>
* <span data-ttu-id="beb0e-3383">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3383">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3384">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3384">Appservice</span></span>

* <span data-ttu-id="beb0e-3385">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3385">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-3386">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3386">CDN</span></span>

* <span data-ttu-id="beb0e-3387">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3387">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="beb0e-3388">Extensão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3388">Extension</span></span>

* <span data-ttu-id="beb0e-3389">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-3389">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-3390">Keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-3390">Keyvault</span></span>

* <span data-ttu-id="beb0e-3391">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3391">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3392">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3392">Network</span></span>

* <span data-ttu-id="beb0e-3393">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3393">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="beb0e-3394">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3394">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="beb0e-3395">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3395">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="beb0e-3396">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3396">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="beb0e-3397">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3397">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3398">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3398">Resource</span></span>

* <span data-ttu-id="beb0e-3399">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3399">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="beb0e-3400">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3400">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="beb0e-3401">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="beb0e-3401">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="beb0e-3402">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3402">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3403">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3403">SQL</span></span>

* <span data-ttu-id="beb0e-3404">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3404">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3405">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3405">VM</span></span>

* <span data-ttu-id="beb0e-3406">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="beb0e-3406">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="beb0e-3407">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="beb0e-3407">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="beb0e-3408">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3408">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="beb0e-3409">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3409">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="beb0e-3410">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="beb0e-3410">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="beb0e-3411">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3411">August 31, 2017</span></span>

<span data-ttu-id="beb0e-3412">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="beb0e-3412">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-3413">Keyvault</span><span class="sxs-lookup"><span data-stu-id="beb0e-3413">Keyvault</span></span>

* <span data-ttu-id="beb0e-3414">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3414">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="beb0e-3415">Sf</span><span class="sxs-lookup"><span data-stu-id="beb0e-3415">Sf</span></span>

* <span data-ttu-id="beb0e-3416">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3416">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3417">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3417">Storage</span></span>

* <span data-ttu-id="beb0e-3418">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="beb0e-3418">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="beb0e-3419">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3419">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="beb0e-3420">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3420">August 28, 2017</span></span>

<span data-ttu-id="beb0e-3421">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="beb0e-3421">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="beb0e-3422">CLI</span><span class="sxs-lookup"><span data-stu-id="beb0e-3422">CLI</span></span>

* <span data-ttu-id="beb0e-3423">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3423">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3424">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3424">ACS</span></span>

* <span data-ttu-id="beb0e-3425">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-3425">Corrected preview regions</span></span>
* <span data-ttu-id="beb0e-3426">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3426">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="beb0e-3427">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3427">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3428">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3428">Appservice</span></span>

* <span data-ttu-id="beb0e-3429">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3429">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="beb0e-3430">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3430">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="beb0e-3431">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3431">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="beb0e-3432">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3432">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="beb0e-3433">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3433">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-3434">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3434">IoT</span></span>

* <span data-ttu-id="beb0e-3435">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3435">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3436">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3436">Network</span></span>

* <span data-ttu-id="beb0e-3437">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3437">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="beb0e-3438">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3438">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="beb0e-3439">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3439">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="beb0e-3440">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3440">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="beb0e-3441">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3441">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3442">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3442">Profile</span></span>

* <span data-ttu-id="beb0e-3443">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="beb0e-3443">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="beb0e-3444">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-3444">Service Fabric</span></span>

* <span data-ttu-id="beb0e-3445">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="beb0e-3445">Preview release</span></span>
* <span data-ttu-id="beb0e-3446">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-3446">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="beb0e-3447">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="beb0e-3447">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="beb0e-3448">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="beb0e-3448">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3449">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3449">Storage</span></span>

* <span data-ttu-id="beb0e-3450">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="beb0e-3450">Enabled setting blob tier</span></span>
* <span data-ttu-id="beb0e-3451">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="beb0e-3451">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="beb0e-3452">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="beb0e-3452">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="beb0e-3453">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3453">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="beb0e-3454">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3454">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="beb0e-3455">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="beb0e-3455">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3456">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3456">VM</span></span>

* <span data-ttu-id="beb0e-3457">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3457">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="beb0e-3458">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3458">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="beb0e-3459">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3459">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="beb0e-3460">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3460">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="beb0e-3461">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="beb0e-3461">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="beb0e-3462">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3462">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="beb0e-3463">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3463">August 15, 2017</span></span>

<span data-ttu-id="beb0e-3464">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="beb0e-3464">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3465">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3465">ACS</span></span>

* <span data-ttu-id="beb0e-3466">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3466">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3467">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3467">Appservice</span></span>

* <span data-ttu-id="beb0e-3468">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="beb0e-3468">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="beb0e-3469">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3469">Event Grid</span></span>

* <span data-ttu-id="beb0e-3470">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="beb0e-3470">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="beb0e-3471">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3471">August 11, 2017</span></span>

<span data-ttu-id="beb0e-3472">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="beb0e-3472">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3473">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3473">ACS</span></span>

* <span data-ttu-id="beb0e-3474">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-3474">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-3475">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3475">Batch</span></span>

* <span data-ttu-id="beb0e-3476">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-3476">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="beb0e-3477">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-3477">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="beb0e-3478">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3478">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="beb0e-3479">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3479">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="beb0e-3480">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="beb0e-3480">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="beb0e-3481">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="beb0e-3481">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="beb0e-3482">Componente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3482">Component</span></span>

* <span data-ttu-id="beb0e-3483">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="beb0e-3483">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="beb0e-3484">Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3484">Container</span></span>

* <span data-ttu-id="beb0e-3485">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3485">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="beb0e-3486">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3486">Data Lake Store</span></span>

* <span data-ttu-id="beb0e-3487">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3487">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="beb0e-3488">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3488">Event Grid</span></span>

* <span data-ttu-id="beb0e-3489">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="beb0e-3489">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3490">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3490">Network</span></span>

* <span data-ttu-id="beb0e-3491">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3491">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="beb0e-3492">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3492">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="beb0e-3493">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3493">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="beb0e-3494">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3494">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3495">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3495">Profile</span></span>

* <span data-ttu-id="beb0e-3496">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="beb0e-3496">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3497">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3497">Storage</span></span>

* <span data-ttu-id="beb0e-3498">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="beb0e-3498">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3499">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3499">VM</span></span>

* <span data-ttu-id="beb0e-3500">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3500">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="beb0e-3501">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3501">Exposed `list-skus` command</span></span>
* <span data-ttu-id="beb0e-3502">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3502">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="beb0e-3503">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3503">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="beb0e-3504">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3504">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="beb0e-3505">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3505">July 28, 2017</span></span>

<span data-ttu-id="beb0e-3506">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="beb0e-3506">Version 2.0.12</span></span>

* <span data-ttu-id="beb0e-3507">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3507">Added container commands</span></span>
* <span data-ttu-id="beb0e-3508">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3508">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="beb0e-3509">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3509">Core</span></span>

* <span data-ttu-id="beb0e-3510">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3510">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="beb0e-3511">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="beb0e-3511">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="beb0e-3512">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="beb0e-3512">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="beb0e-3513">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3513">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="beb0e-3514">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-3514">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="beb0e-3515">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3515">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="beb0e-3516">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3516">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="beb0e-3517">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3517">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="beb0e-3518">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3518">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="beb0e-3519">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="beb0e-3519">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="beb0e-3520">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3520">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="beb0e-3521">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3521">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="beb0e-3522">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3522">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="beb0e-3523">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="beb0e-3523">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="beb0e-3524">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="beb0e-3524">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="beb0e-3525">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3525">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="beb0e-3526">ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3526">ACR</span></span>

* <span data-ttu-id="beb0e-3527">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3527">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="beb0e-3528">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3528">Support SKU update for managed registries</span></span>
* <span data-ttu-id="beb0e-3529">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3529">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="beb0e-3530">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3530">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="beb0e-3531">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3531">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="beb0e-3532">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="beb0e-3532">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3533">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3533">ACS</span></span>

* <span data-ttu-id="beb0e-3534">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="beb0e-3534">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3535">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3535">Appservice</span></span>

* <span data-ttu-id="beb0e-3536">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3536">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="beb0e-3537">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="beb0e-3537">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="beb0e-3538">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3538">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="beb0e-3539">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3539">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="beb0e-3540">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3540">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="beb0e-3541">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3541">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="beb0e-3542">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3542">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="beb0e-3543">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3543">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="beb0e-3544">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3544">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="beb0e-3545">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3545">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="beb0e-3546">Lote</span><span class="sxs-lookup"><span data-stu-id="beb0e-3546">Batch</span></span>

* <span data-ttu-id="beb0e-3547">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="beb0e-3547">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="beb0e-3548">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3548">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="beb0e-3549">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3549">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="beb0e-3550">CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3550">CDN</span></span>

* <span data-ttu-id="beb0e-3551">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="beb0e-3551">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="beb0e-3552">Nuvem</span><span class="sxs-lookup"><span data-stu-id="beb0e-3552">Cloud</span></span>

* <span data-ttu-id="beb0e-3553">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="beb0e-3553">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="beb0e-3554">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="beb0e-3554">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="beb0e-3555">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3555">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="beb0e-3556">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="beb0e-3556">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="beb0e-3557">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3557">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-3558">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3558">CosmosDB</span></span>

* <span data-ttu-id="beb0e-3559">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3559">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="beb0e-3560">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="beb0e-3560">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="beb0e-3561">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-3561">Data Lake Analytics</span></span>

* <span data-ttu-id="beb0e-3562">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3562">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="beb0e-3563">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3563">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="beb0e-3564">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3564">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="beb0e-3565">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3565">Data Lake Store</span></span>

* <span data-ttu-id="beb0e-3566">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3566">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="beb0e-3567">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="beb0e-3567">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="beb0e-3568">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3568">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="beb0e-3569">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3569">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="beb0e-3570">Interativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3570">Interactive</span></span>

* <span data-ttu-id="beb0e-3571">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="beb0e-3571">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="beb0e-3572">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="beb0e-3572">Increased test coverage</span></span>
* <span data-ttu-id="beb0e-3573">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="beb0e-3573">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="beb0e-3574">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3574">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="beb0e-3575">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3575">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="beb0e-3576">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3576">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="beb0e-3577">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3577">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="beb0e-3578">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3578">Added `--progress` flag</span></span>
* <span data-ttu-id="beb0e-3579">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="beb0e-3579">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="beb0e-3580">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3580">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="beb0e-3581">IoT</span><span class="sxs-lookup"><span data-stu-id="beb0e-3581">IoT</span></span>

* <span data-ttu-id="beb0e-3582">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3582">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="beb0e-3583">(#3934)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3583">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="beb0e-3584">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="beb0e-3584">Key vault</span></span>

* <span data-ttu-id="beb0e-3585">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3585">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="beb0e-3586">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3586">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="beb0e-3587">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3587">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="beb0e-3588">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3588">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="beb0e-3589">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3589">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="beb0e-3590">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3590">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="beb0e-3591">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3591">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="beb0e-3592">(#3307)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3592">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="beb0e-3593">Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3593">Lab</span></span>

* <span data-ttu-id="beb0e-3594">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3594">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="beb0e-3595">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3595">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3596">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3596">Monitor</span></span>

* <span data-ttu-id="beb0e-3597">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3597">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="beb0e-3598">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3598">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="beb0e-3599">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3599">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="beb0e-3600">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3600">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="beb0e-3601">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3601">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="beb0e-3602">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3602">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="beb0e-3603">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="beb0e-3603">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="beb0e-3604">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="beb0e-3604">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="beb0e-3605">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="beb0e-3605">`location` no longer required</span></span>
  * <span data-ttu-id="beb0e-3606">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="beb0e-3606">Add name and ID support for target</span></span>
  * <span data-ttu-id="beb0e-3607">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3607">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="beb0e-3608">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="beb0e-3608">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="beb0e-3609">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="beb0e-3609">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="beb0e-3610">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="beb0e-3610">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="beb0e-3611">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3611">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="beb0e-3612">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3612">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3613">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3613">Network</span></span>

* <span data-ttu-id="beb0e-3614">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3614">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="beb0e-3615">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3615">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="beb0e-3616">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="beb0e-3616">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="beb0e-3617">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="beb0e-3617">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="beb0e-3618">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3618">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="beb0e-3619">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3619">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="beb0e-3620">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3620">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="beb0e-3621">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3621">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="beb0e-3622">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3622">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="beb0e-3623">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3623">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="beb0e-3624">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3624">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="beb0e-3625">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3625">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="beb0e-3626">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3626">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="beb0e-3627">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3627">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="beb0e-3628">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3628">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="beb0e-3629">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3629">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="beb0e-3630">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="beb0e-3630">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="beb0e-3631">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3631">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="beb0e-3632">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3632">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="beb0e-3633">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3633">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="beb0e-3634">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3634">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="beb0e-3635">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3635">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="beb0e-3636">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3636">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="beb0e-3637">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="beb0e-3637">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="beb0e-3638">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="beb0e-3638">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="beb0e-3639">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="beb0e-3639">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="beb0e-3640">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="beb0e-3640">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3641">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3641">Profile</span></span>

* <span data-ttu-id="beb0e-3642">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3642">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="beb0e-3643">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="beb0e-3643">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="beb0e-3644">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3644">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="beb0e-3645">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="beb0e-3645">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="beb0e-3646">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3646">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="beb0e-3647">RDBMS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3647">RDBMS</span></span>

* <span data-ttu-id="beb0e-3648">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3648">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="beb0e-3649">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3649">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="beb0e-3650">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3650">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="beb0e-3651">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3651">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3652">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3652">Resource</span></span>

* <span data-ttu-id="beb0e-3653">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3653">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="beb0e-3654">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3654">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="beb0e-3655">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3655">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="beb0e-3656">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3656">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="beb0e-3657">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3657">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="beb0e-3658">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3658">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="beb0e-3659">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3659">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="beb0e-3660">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3660">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-3661">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3661">Role</span></span>

* <span data-ttu-id="beb0e-3662">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3662">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="beb0e-3663">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3663">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="beb0e-3664">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3664">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="beb0e-3665">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3665">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="beb0e-3666">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3666">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="beb0e-3667">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-3667">Service Fabric</span></span>
* <span data-ttu-id="beb0e-3668">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3668">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="beb0e-3669">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3669">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="beb0e-3670">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3670">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3671">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3671">SQL</span></span>

* <span data-ttu-id="beb0e-3672">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="beb0e-3672">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="beb0e-3673">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3673">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="beb0e-3674">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3674">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3675">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3675">Storage</span></span>

* <span data-ttu-id="beb0e-3676">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3676">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="beb0e-3677">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="beb0e-3677">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="beb0e-3678">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3678">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="beb0e-3679">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3679">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="beb0e-3680">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3680">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="beb0e-3681">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3681">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3682">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3682">VM</span></span>

* <span data-ttu-id="beb0e-3683">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="beb0e-3683">Support configuring nsg</span></span>
* <span data-ttu-id="beb0e-3684">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3684">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="beb0e-3685">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3685">Support managed service identities</span></span>
* <span data-ttu-id="beb0e-3686">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3686">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="beb0e-3687">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="beb0e-3687">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="beb0e-3688">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3688">May 10, 2017</span></span>

<span data-ttu-id="beb0e-3689">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="beb0e-3689">Version 2.0.6</span></span>

* <span data-ttu-id="beb0e-3690">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3690">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="beb0e-3691">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3691">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="beb0e-3692">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3692">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="beb0e-3693">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3693">Include Cognitive Services module</span></span>
* <span data-ttu-id="beb0e-3694">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="beb0e-3694">Include Service Fabric module</span></span>
* <span data-ttu-id="beb0e-3695">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3695">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="beb0e-3696">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3696">Add support for CDN commands</span></span>
* <span data-ttu-id="beb0e-3697">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="beb0e-3697">Remove Container module</span></span>
* <span data-ttu-id="beb0e-3698">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3698">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="beb0e-3699">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3699">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="beb0e-3700">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3700">Core</span></span>

* <span data-ttu-id="beb0e-3701">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="beb0e-3701">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="beb0e-3702">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3702">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="beb0e-3703">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3703">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="beb0e-3704">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3704">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="beb0e-3705">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3705">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="beb0e-3706">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3706">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="beb0e-3707">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3707">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="beb0e-3708">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3708">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="beb0e-3709">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3709">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="beb0e-3710">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="beb0e-3710">core: Improved performance</span></span>
* <span data-ttu-id="beb0e-3711">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="beb0e-3711">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="beb0e-3712">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="beb0e-3712">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3713">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3713">ACS</span></span>

* <span data-ttu-id="beb0e-3714">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="beb0e-3714">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="beb0e-3715">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="beb0e-3715">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="beb0e-3716">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="beb0e-3716">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="beb0e-3717">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3717">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3718">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3718">AppService</span></span>

* <span data-ttu-id="beb0e-3719">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3719">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="beb0e-3720">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3720">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="beb0e-3721">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3721">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="beb0e-3722">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="beb0e-3722">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="beb0e-3723">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3723">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="beb0e-3724">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3724">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="beb0e-3725">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="beb0e-3725">support slot swap with preview</span></span>
* <span data-ttu-id="beb0e-3726">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3726">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="beb0e-3727">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3727">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="beb0e-3728">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3728">CosmosDB</span></span>

* <span data-ttu-id="beb0e-3729">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3729">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="beb0e-3730">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="beb0e-3730">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="beb0e-3731">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="beb0e-3731">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="beb0e-3732">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="beb0e-3732">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="beb0e-3733">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-3733">Data Lake Analytics</span></span>

* <span data-ttu-id="beb0e-3734">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="beb0e-3734">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="beb0e-3735">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3735">Add support for new catalog item type: package.</span></span> <span data-ttu-id="beb0e-3736">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3736">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="beb0e-3737">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="beb0e-3737">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="beb0e-3738">Tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-3738">Table</span></span>
  * <span data-ttu-id="beb0e-3739">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-3739">Table valued function</span></span>
  * <span data-ttu-id="beb0e-3740">Visualizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-3740">View</span></span>
  * <span data-ttu-id="beb0e-3741">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3741">Table Statistics.</span></span> <span data-ttu-id="beb0e-3742">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="beb0e-3742">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="beb0e-3743">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3743">Data Lake Store</span></span>

* <span data-ttu-id="beb0e-3744">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="beb0e-3744">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="beb0e-3745">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3745">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="beb0e-3746">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3746">missed help for access show.</span></span> <span data-ttu-id="beb0e-3747">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3747">adding it.</span></span> <span data-ttu-id="beb0e-3748">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3748">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="beb0e-3749">Localizar</span><span class="sxs-lookup"><span data-stu-id="beb0e-3749">Find</span></span>

* <span data-ttu-id="beb0e-3750">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="beb0e-3750">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="beb0e-3751">KeyVault</span><span class="sxs-lookup"><span data-stu-id="beb0e-3751">KeyVault</span></span>

* <span data-ttu-id="beb0e-3752">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="beb0e-3752">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="beb0e-3753">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="beb0e-3753">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="beb0e-3754">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="beb0e-3754">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="beb0e-3755">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3755">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="beb0e-3756">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3756">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="beb0e-3757">Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3757">Lab</span></span>

* <span data-ttu-id="beb0e-3758">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3758">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="beb0e-3759">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3759">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="beb0e-3760">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3760">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="beb0e-3761">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3761">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="beb0e-3762">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="beb0e-3762">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="beb0e-3763">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3763">Monitor</span></span>

* <span data-ttu-id="beb0e-3764">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3764">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="beb0e-3765">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3765">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="beb0e-3766">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3766">Network</span></span>

* <span data-ttu-id="beb0e-3767">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3767">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="beb0e-3768">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3768">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="beb0e-3769">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3769">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="beb0e-3770">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3770">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="beb0e-3771">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="beb0e-3771">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="beb0e-3772">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="beb0e-3772">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="beb0e-3773">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3773">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="beb0e-3774">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="beb0e-3774">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="beb0e-3775">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3775">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="beb0e-3776">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="beb0e-3776">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="beb0e-3777">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3777">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="beb0e-3778">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3778">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="beb0e-3779">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3779">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="beb0e-3780">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="beb0e-3780">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="beb0e-3781">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="beb0e-3781">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="beb0e-3782">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3782">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="beb0e-3783">Perfil</span><span class="sxs-lookup"><span data-stu-id="beb0e-3783">Profile</span></span>

* <span data-ttu-id="beb0e-3784">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3784">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="beb0e-3785">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3785">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="beb0e-3786">Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-3786">Redis</span></span>

* <span data-ttu-id="beb0e-3787">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="beb0e-3787">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="beb0e-3788">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="beb0e-3788">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="beb0e-3789">Recurso</span><span class="sxs-lookup"><span data-stu-id="beb0e-3789">Resource</span></span>

* <span data-ttu-id="beb0e-3790">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3790">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="beb0e-3791">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3791">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="beb0e-3792">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3792">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="beb0e-3793">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3793">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="beb0e-3794">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3794">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="beb0e-3795">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3795">Add docs for az lock update.</span></span> <span data-ttu-id="beb0e-3796">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3796">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="beb0e-3797">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3797">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="beb0e-3798">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3798">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="beb0e-3799">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3799">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="beb0e-3800">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3800">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="beb0e-3801">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3801">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="beb0e-3802">Função</span><span class="sxs-lookup"><span data-stu-id="beb0e-3802">Role</span></span>

* <span data-ttu-id="beb0e-3803">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3803">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="beb0e-3804">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3804">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="beb0e-3805">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3805">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="beb0e-3806">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="beb0e-3806">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="beb0e-3807">SQL</span><span class="sxs-lookup"><span data-stu-id="beb0e-3807">SQL</span></span>

* <span data-ttu-id="beb0e-3808">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="beb0e-3808">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="beb0e-3809">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3809">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="beb0e-3810">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3810">Storage</span></span>

* <span data-ttu-id="beb0e-3811">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3811">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="beb0e-3812">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="beb0e-3812">Add support for incremental blob copy</span></span>
* <span data-ttu-id="beb0e-3813">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="beb0e-3813">Add support for large block blob upload</span></span>
* <span data-ttu-id="beb0e-3814">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3814">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3815">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3815">VM</span></span>

* <span data-ttu-id="beb0e-3816">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="beb0e-3816">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="beb0e-3817">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3817">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="beb0e-3818">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="beb0e-3818">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="beb0e-3819">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="beb0e-3819">az vm/vmss disk</span></span>
  3. <span data-ttu-id="beb0e-3820">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="beb0e-3820">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="beb0e-3821">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="beb0e-3821">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="beb0e-3822">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3822">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="beb0e-3823">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3823">April 3, 2017</span></span>

<span data-ttu-id="beb0e-3824">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="beb0e-3824">Version 2.0.2</span></span>

<span data-ttu-id="beb0e-3825">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3825">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="beb0e-3826">Núcleo</span><span class="sxs-lookup"><span data-stu-id="beb0e-3826">Core</span></span>

* <span data-ttu-id="beb0e-3827">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3827">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="beb0e-3828">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3828">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="beb0e-3829">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3829">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="beb0e-3830">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3830">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="beb0e-3831">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3831">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="beb0e-3832">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3832">Add prompting for missing template parameters.</span></span> <span data-ttu-id="beb0e-3833">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3833">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="beb0e-3834">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="beb0e-3834">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="beb0e-3835">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="beb0e-3835">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="beb0e-3836">ACS</span><span class="sxs-lookup"><span data-stu-id="beb0e-3836">ACS</span></span>

* <span data-ttu-id="beb0e-3837">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3837">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="beb0e-3838">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3838">Add support for ssh key password prompting.</span></span> <span data-ttu-id="beb0e-3839">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3839">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="beb0e-3840">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3840">Add support for windows clusters.</span></span> <span data-ttu-id="beb0e-3841">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3841">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="beb0e-3842">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3842">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="beb0e-3843">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3843">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="beb0e-3844">AppService</span><span class="sxs-lookup"><span data-stu-id="beb0e-3844">AppService</span></span>

* <span data-ttu-id="beb0e-3845">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3845">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="beb0e-3846">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3846">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="beb0e-3847">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3847">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="beb0e-3848">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3848">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="beb0e-3849">DataLake</span><span class="sxs-lookup"><span data-stu-id="beb0e-3849">DataLake</span></span>

* <span data-ttu-id="beb0e-3850">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="beb0e-3850">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="beb0e-3851">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="beb0e-3851">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="beb0e-3852">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="beb0e-3852">DocuemntDB</span></span>

* <span data-ttu-id="beb0e-3853">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3853">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="beb0e-3854">VM</span><span class="sxs-lookup"><span data-stu-id="beb0e-3854">VM</span></span>

* <span data-ttu-id="beb0e-3855">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3855">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="beb0e-3856">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3856">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="beb0e-3857">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3857">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="beb0e-3858">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3858">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="beb0e-3859">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3859">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="beb0e-3860">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3860">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="beb0e-3861">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="beb0e-3861">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="beb0e-3862">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="beb0e-3862">February 27, 2017</span></span>

<span data-ttu-id="beb0e-3863">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="beb0e-3863">Version 2.0.0</span></span>

<span data-ttu-id="beb0e-3864">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3864">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="beb0e-3865">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3865">Container Service (acs)</span></span>
- <span data-ttu-id="beb0e-3866">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3866">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="beb0e-3867">Rede</span><span class="sxs-lookup"><span data-stu-id="beb0e-3867">Networking</span></span>
- <span data-ttu-id="beb0e-3868">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="beb0e-3868">Storage</span></span>

<span data-ttu-id="beb0e-3869">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3869">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="beb0e-3870">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-3870">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="beb0e-3871">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="beb0e-3871">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="beb0e-3872">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="beb0e-3872">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="beb0e-3873">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3873">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="beb0e-3874">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="beb0e-3874">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="beb0e-3875">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3875">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="beb0e-3876">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="beb0e-3876">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="beb0e-3877">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="beb0e-3877">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="beb0e-3878">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="beb0e-3878">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="beb0e-3879">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="beb0e-3879">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="beb0e-3880">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="beb0e-3880">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="beb0e-3881">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="beb0e-3881">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="beb0e-3882">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3882">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="beb0e-3883">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3883">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="beb0e-3884">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3884">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="beb0e-3885">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3885">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="beb0e-3886">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3886">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="beb0e-3887">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="beb0e-3887">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="beb0e-3888">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="beb0e-3888">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
