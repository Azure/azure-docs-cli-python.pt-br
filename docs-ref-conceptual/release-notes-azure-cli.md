---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 08/06/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: f81f5a69bd5806d2081a8eaa9b62a5b00b56edf9
ms.sourcegitcommit: 04d3b43d7c960ff0e6188c9672d27046b45da6ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87855926"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="e5954-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="e5954-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="e5954-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="august-11-2020"></a><span data-ttu-id="e5954-105">11 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-105">August 11, 2020</span></span>

<span data-ttu-id="e5954-106">Versão 2.10.1</span><span class="sxs-lookup"><span data-stu-id="e5954-106">Version 2.10.1</span></span>

### <a name="app-service"></a><span data-ttu-id="e5954-107">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-107">App Service</span></span>

* <span data-ttu-id="e5954-108">Correção nº 9887 webapp e functionapp, dar suporte à atribuição/remoção de identidade gerenciada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-108">Fix #9887 webapp and functionapp, support assigning/removing user managed identity</span></span>
* <span data-ttu-id="e5954-109">Correção nº 1382, 14055: atualizar mensagens de erro para az webapp create e az webapp config container set</span><span class="sxs-lookup"><span data-stu-id="e5954-109">Fix #1382, #14055: Update error messages for az webapp create and az webapp config container set</span></span>
* <span data-ttu-id="e5954-110">`az webapp up`: corrigir a lógica de seleção padrão do ASP quando o parâmetro --plan não é fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-110">`az webapp up`: Fix default ASP selection logic when --plan parameter is not provided</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-111">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-111">AppConfig</span></span>

* <span data-ttu-id="e5954-112">Dar suporte para habilitar/desabilitar PublicNetworkAccess durante a criação da loja</span><span class="sxs-lookup"><span data-stu-id="e5954-112">Support enabling/disabling PublicNetworkAccess during store creation</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-113">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-113">Compute</span></span>

* <span data-ttu-id="e5954-114">Dar suporte à associação de disco e instantâneo com um recurso de acesso a disco</span><span class="sxs-lookup"><span data-stu-id="e5954-114">Support associating disk and snapshot with a disk-access resource</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-115">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-115">Lab</span></span>

* <span data-ttu-id="e5954-116">Correção do problema nº 7904: bug de validação de data na criação de VM do laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-116">Fix for issue #7904 date validation bug in lab vm creation</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-117">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-117">Storage</span></span>

* <span data-ttu-id="e5954-118">`az storage blob upload-batch`: correção do problema nº 14660 com argumentos não posicionais</span><span class="sxs-lookup"><span data-stu-id="e5954-118">`az storage blob upload-batch`: Fix issue #14660 with unpositional arguments</span></span>

## <a name="august-04-2020"></a><span data-ttu-id="e5954-119">04 de agosto de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-119">August 04, 2020</span></span>

<span data-ttu-id="e5954-120">Versão 2.10.0</span><span class="sxs-lookup"><span data-stu-id="e5954-120">Version 2.10.0</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-121">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-121">AKS</span></span>

* <span data-ttu-id="e5954-122">`az aks update`: Alteração do argumento --enable-aad para migrar um cluster não AAD habilitado para RBAC para um cluster AAD gerenciado por AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-122">`az aks update`: Change --enable-aad argument to migrate a RBAC-enabled non-AAD cluster to a AKS-managed AAD cluster</span></span>
* <span data-ttu-id="e5954-123">`az aks install-cli`: Adição de argumentos --kubelogin-version e --kubelogin-install-location para instalar o kubelogin</span><span class="sxs-lookup"><span data-stu-id="e5954-123">`az aks install-cli`: Add --kubelogin-version and --kubelogin-install-location arguments to install kubelogin</span></span>
* <span data-ttu-id="e5954-124">Adição do comando az aks nodepool get-upgrades</span><span class="sxs-lookup"><span data-stu-id="e5954-124">Add az aks nodepool get-upgrades command</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-125">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-125">AMS</span></span>

* <span data-ttu-id="e5954-126">Correção nº 14021: az ams account sp não é idempotente</span><span class="sxs-lookup"><span data-stu-id="e5954-126">Fix #14021: az ams account sp is not idempotent</span></span>

### <a name="apim"></a><span data-ttu-id="e5954-127">APIM</span><span class="sxs-lookup"><span data-stu-id="e5954-127">APIM</span></span>

* <span data-ttu-id="e5954-128">importação da API de APIM: suporte à importação de API e aprimoramento de outros comandos da CLI de nível da API</span><span class="sxs-lookup"><span data-stu-id="e5954-128">apim api import: support API import and enchance other api level cli commands</span></span>

### <a name="app-service"></a><span data-ttu-id="e5954-129">Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-129">App Service</span></span>

* <span data-ttu-id="e5954-130">Correção nº 13035: Adição de validação para az webapp config access-restriction para evitar a adição de duplicatas</span><span class="sxs-lookup"><span data-stu-id="e5954-130">Fix #13035: Add validation for az webapp config access-restriction to avoid adding duplicates</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-131">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-131">AppConfig</span></span>

* <span data-ttu-id="e5954-132">Adoção de SKU padrão se não for especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-132">Default to standard sku if not specified</span></span>
* <span data-ttu-id="e5954-133">[ALTERAÇÃO SIGNIFICATIVA] Configurações de suporte com tipo de conteúdo JSON</span><span class="sxs-lookup"><span data-stu-id="e5954-133">[BREAKING CHANGE] Support settings with JSON content type</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-134">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-134">ARM</span></span>

* <span data-ttu-id="e5954-135">`az resource tag`: Correção do bug de marcação managedApp e alguns problemas de teste relacionados</span><span class="sxs-lookup"><span data-stu-id="e5954-135">`az resource tag`: Fix the bug of managedApp tagging and some related test issues</span></span>
* <span data-ttu-id="e5954-136">`az deployment mg/tenant what-if`: Adição de suporte ao grupo de gerenciamento e à implantação de nível de locatário What-If</span><span class="sxs-lookup"><span data-stu-id="e5954-136">`az deployment mg/tenant what-if`: Add support to management group and tenant level deployment What-If</span></span>
* <span data-ttu-id="e5954-137">`az deployment mg/tenant create`: Adição do parâmetro --confirm-with-what-if/-c.</span><span class="sxs-lookup"><span data-stu-id="e5954-137">`az deployment mg/tenant create`: Add --confirm-with-what-if/-c parameter.</span></span>
* <span data-ttu-id="e5954-138">`az deployment mg/tenant create`: Adição do parâmetro --what-if-result-format/-r.</span><span class="sxs-lookup"><span data-stu-id="e5954-138">`az deployment mg/tenant create`: Add --what-if-result-format/-r parameter.</span></span>
* <span data-ttu-id="e5954-139">`az deployment mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="e5954-139">`az deployment mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="e5954-140">`az tag`: az tag support para parâmetro ID de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-140">`az tag`: az tag support for resource id parameter</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-141">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-141">Backup</span></span>

* <span data-ttu-id="e5954-142">Disparar a descoberta de contêiner/item AFS somente quando necessário</span><span class="sxs-lookup"><span data-stu-id="e5954-142">Trigger AFS container/item discovery only when needed</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-143">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-143">CDN</span></span>

* <span data-ttu-id="e5954-144">Adicionar campos de link privado à origem</span><span class="sxs-lookup"><span data-stu-id="e5954-144">Add private link fields to origin</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-145">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-145">Compute</span></span>

* <span data-ttu-id="e5954-146">`az vm/vmss create`: Selecione um nome de usuário válido para usuário se o nome de usuário padrão for inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-146">`az vm/vmss create`: Select a valid username for user if the default username is invalid</span></span>
* <span data-ttu-id="e5954-147">`az vm update`: suporte à imagem entre locatários</span><span class="sxs-lookup"><span data-stu-id="e5954-147">`az vm update`: support cross tenant image</span></span>
* <span data-ttu-id="e5954-148">`az disk-access`: Adicionar novo grupo de comandos para operar o recurso de acesso ao disco</span><span class="sxs-lookup"><span data-stu-id="e5954-148">`az disk-access`: Add new command group to operate disk access resource</span></span>
* <span data-ttu-id="e5954-149">Suporte ao posicionamento automático do grupo de hosts dedicado</span><span class="sxs-lookup"><span data-stu-id="e5954-149">Support dedicated host group automatic placement</span></span>
* <span data-ttu-id="e5954-150">Suporte a PPG e SPG no modo de orquestração de VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-150">Support ppg and spg in VMSS orchestration mode</span></span>

### <a name="config"></a><span data-ttu-id="e5954-151">Config</span><span class="sxs-lookup"><span data-stu-id="e5954-151">Config</span></span>

* <span data-ttu-id="e5954-152">`az config`: Adição do novo módulo de comando `config`</span><span class="sxs-lookup"><span data-stu-id="e5954-152">`az config`: Add new `config` command module</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-153">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-153">Extension</span></span>

* <span data-ttu-id="e5954-154">Suporte à instalação automática de uma extensão se a extensão de um comando não estiver instalada</span><span class="sxs-lookup"><span data-stu-id="e5954-154">Support automatically installing an extension if the extension of a command is not installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-155">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-155">HDInsight</span></span>

* <span data-ttu-id="e5954-156">Adição de três parâmetros ao comando `az hdinsight create` para compatibilidade com o link privado e o recurso de criptografia em trânsito:</span><span class="sxs-lookup"><span data-stu-id="e5954-156">Add 3 parameters to the command `az hdinsight create` to support private link and encryption in transit feature:</span></span>

### <a name="iot-hub"></a><span data-ttu-id="e5954-157">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-157">Iot Hub</span></span>

* <span data-ttu-id="e5954-158">Correção nº 7792: A criação do Hub IoT não é idempotente</span><span class="sxs-lookup"><span data-stu-id="e5954-158">Fix #7792: IoT Hub Create is not idempotent</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5954-159">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-159">IoT Central</span></span>

* <span data-ttu-id="e5954-160">Adição de lista de opções de parâmetros para IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-160">Add paramater option list for iot central</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-161">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-161">KeyVault</span></span>

* <span data-ttu-id="e5954-162">`az keyvault key encrypt/decrypt`: adição de parâmetro `--data-type` para especificar explicitamente o tipo de dado original</span><span class="sxs-lookup"><span data-stu-id="e5954-162">`az keyvault key encrypt/decrypt`: add parameter `--data-type` for explicitly specifing the type of original data</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-163">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-163">Monitor</span></span>

* <span data-ttu-id="e5954-164">`az monitor log-analytics workspace data-export`: suporte ao namespace do hub de eventos como o destino.</span><span class="sxs-lookup"><span data-stu-id="e5954-164">`az monitor log-analytics workspace data-export`: support event hub namespace as the destination.</span></span>
* <span data-ttu-id="e5954-165">`az monitor autoscale`: suporte a namespace e dimensões para --condition</span><span class="sxs-lookup"><span data-stu-id="e5954-165">`az monitor autoscale`: support namespace and dimensions for --condition</span></span>

### <a name="netappfiles"></a><span data-ttu-id="e5954-166">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="e5954-166">NetAppFiles</span></span>

* <span data-ttu-id="e5954-167">`az volume revert`:  Adição de Reversão de Volume para reverter um volume para um de seus instantâneos.</span><span class="sxs-lookup"><span data-stu-id="e5954-167">`az volume revert`:  Add Volume Revert to revert a volume to one of its snapshots.</span></span>
* <span data-ttu-id="e5954-168">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `az netappfiles mount-target`.</span><span class="sxs-lookup"><span data-stu-id="e5954-168">[BREAKING CHANGE] Remove `az netappfiles mount-target`.</span></span>
* <span data-ttu-id="e5954-169">`az volume show`: Adição de site para Propriedades do Active Directory</span><span class="sxs-lookup"><span data-stu-id="e5954-169">`az volume show`: Add site to Active Directory Properties</span></span>

### <a name="network"></a><span data-ttu-id="e5954-170">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-170">Network</span></span>

* <span data-ttu-id="e5954-171">`az application-gateway private-link add`: suporte para especificar uma sub-rede existente por ID</span><span class="sxs-lookup"><span data-stu-id="e5954-171">`az application-gateway private-link add`: support to specify an existing subnet by ID</span></span>
* <span data-ttu-id="e5954-172">`az network application-gateway waf-policy create`: versão e tipo de suporte</span><span class="sxs-lookup"><span data-stu-id="e5954-172">`az network application-gateway waf-policy create`: support version and type</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-173">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-173">Storage</span></span>

* <span data-ttu-id="e5954-174">Correção nº 10302: Suporte à estimativa de tipo de conteúdo ao sincronizar arquivos</span><span class="sxs-lookup"><span data-stu-id="e5954-174">Fix #10302: Support guess content-type when synchronizing files</span></span>
* <span data-ttu-id="e5954-175">`az storage blob lease`: Aplicação de nova versão de API para operações de concessão de blob</span><span class="sxs-lookup"><span data-stu-id="e5954-175">`az storage blob lease`: Apply new api version for blob lease operations</span></span>
* <span data-ttu-id="e5954-176">`az storage fs access`: Suporte a credencial do AAD no gerenciamento de controle de acesso para conta do ADLS Gen2</span><span class="sxs-lookup"><span data-stu-id="e5954-176">`az storage fs access`: Support AAD credential in managing access control for ADLS Gen2 account</span></span>
* <span data-ttu-id="e5954-177">`az storage share-rm create/update`: adição de --access-tier para dar suporte à camada de acesso</span><span class="sxs-lookup"><span data-stu-id="e5954-177">`az storage share-rm create/update`: add --access-tier to support access tier</span></span>

## <a name="july-16-2020"></a><span data-ttu-id="e5954-178">16 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-178">July 16, 2020</span></span>

<span data-ttu-id="e5954-179">Versão 2.9.1</span><span class="sxs-lookup"><span data-stu-id="e5954-179">Version 2.9.1</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-180">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-180">AKS</span></span>

* <span data-ttu-id="e5954-181">Remove a configuração explícita de VMSS no comando de exemplo do Windows, pois ele agora é padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-181">Remove explicit setting of VMSS in Windows example command since it is now default</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-182">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-182">IoT</span></span>

* <span data-ttu-id="e5954-183">[ALTERAÇÃO DA FALHA] `az iot pnp`: Remove comandos de versão prévia do IoT PNP da CLI principal</span><span class="sxs-lookup"><span data-stu-id="e5954-183">[BREAKING CHANGE] `az iot pnp`: Remove IoT PNP preview commands from core CLI</span></span>

### <a name="rest"></a><span data-ttu-id="e5954-184">REST</span><span class="sxs-lookup"><span data-stu-id="e5954-184">REST</span></span>

* <span data-ttu-id="e5954-185">Correção nº14152: `az rest`: aceita URLs do ARM sem a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-185">Fix #14152: `az rest`: Accept ARM URLs without subscription ID</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-186">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-186">Storage</span></span>

* <span data-ttu-id="e5954-187">Correção nº 14138: torna algumas permissões opcionais</span><span class="sxs-lookup"><span data-stu-id="e5954-187">Fix #14138: Make some permissions optional</span></span>

## <a name="july-14-2020"></a><span data-ttu-id="e5954-188">14 de julho de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-188">July 14, 2020</span></span>

<span data-ttu-id="e5954-189">Versão 2.9.0</span><span class="sxs-lookup"><span data-stu-id="e5954-189">Version 2.9.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-190">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-190">ACR</span></span>

* <span data-ttu-id="e5954-191">Manipular o link do artefato de log do Registro para os logs de fluxo</span><span class="sxs-lookup"><span data-stu-id="e5954-191">Handle log artifact link from Registry to stream logs</span></span>
* <span data-ttu-id="e5954-192">Substituir comandos helm2</span><span class="sxs-lookup"><span data-stu-id="e5954-192">Deprecate helm2 commands</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-193">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-193">AKS</span></span>

* <span data-ttu-id="e5954-194">`az aks create`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="e5954-194">`az aks create`: add --enable-aad argument</span></span>
* <span data-ttu-id="e5954-195">`az aks update`: adiciona o argumento --enable-aad</span><span class="sxs-lookup"><span data-stu-id="e5954-195">`az aks update`: add --enable-aad argument</span></span>

### <a name="apim"></a><span data-ttu-id="e5954-196">APIM</span><span class="sxs-lookup"><span data-stu-id="e5954-196">APIM</span></span>

* <span data-ttu-id="e5954-197">Comandos az apim api gerais adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-197">Added general az apim api commands</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-198">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-198">AppConfig</span></span>

* <span data-ttu-id="e5954-199">Adicionar exemplo para usar --fields na revisão do appconfig</span><span class="sxs-lookup"><span data-stu-id="e5954-199">Add example for using --fields in appconfig revision</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-200">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-200">AppService</span></span>

* <span data-ttu-id="e5954-201">`az functionapp create`: Suporte para Java 11 e PowerShell 7 adicionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-201">`az functionapp create`: Added support for Java 11 and Powershell 7.</span></span> <span data-ttu-id="e5954-202">Suporte à API de pilhas adicionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-202">Added Stacks API Support.</span></span>
* <span data-ttu-id="e5954-203">Correção nº 14208 falha na criação de um aplicativo com vários contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-203">Fix #14208 multi-container app creation fails</span></span>
* <span data-ttu-id="e5954-204">Corrige az webapp create – usa pilhas de runtime embutidas em código</span><span class="sxs-lookup"><span data-stu-id="e5954-204">Fix az webapp create - use hardcoded runtime stacks</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-205">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-205">ARM</span></span>

* <span data-ttu-id="e5954-206">`az resource tag`: corrige o problema de marcar recursos com o tipo de recurso `Microsoft.ContainerInstance/containerGroups`</span><span class="sxs-lookup"><span data-stu-id="e5954-206">`az resource tag`: Fix the problem of tagging resources with resource type `Microsoft.ContainerInstance/containerGroups`</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-207">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-207">Compute</span></span>

* <span data-ttu-id="e5954-208">Avançar os discos de versão 2020-05-01, computação 2020-06-01</span><span class="sxs-lookup"><span data-stu-id="e5954-208">Bump version disks 2020-05-01, compute 2020-06-01</span></span>
* <span data-ttu-id="e5954-209">Criptografia dupla do conjunto de criptografia de disco</span><span class="sxs-lookup"><span data-stu-id="e5954-209">Double encryption of disk encryption set</span></span>
* <span data-ttu-id="e5954-210">`az vmss update`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="e5954-210">`az vmss update`: support specify cross tenant image.</span></span>
* <span data-ttu-id="e5954-211">`az sig image-version create`: dá suporte à especificação de imagem entre locatários.</span><span class="sxs-lookup"><span data-stu-id="e5954-211">`az sig image-version create`: support specify cross tenant image.</span></span>
* <span data-ttu-id="e5954-212">vm/vmss create: Criptografia de cache e dados em trânsito para discos do sistema operacional/de dados e discos temporários para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-212">vm/vmss create: Encryption of cache & data-in-transit for OS/Data disks and temp disks for VM & VMSS</span></span>
* <span data-ttu-id="e5954-213">Adicionar operação de remoção simulada para VM e VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-213">Add simulate-eviction operation for VM and VMSS</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-214">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-214">CosmosDB</span></span>

* <span data-ttu-id="e5954-215">Recursos recentes: Autoscale, IpRules, EnableFreeTier e EnableAnalyticalStorage</span><span class="sxs-lookup"><span data-stu-id="e5954-215">Recent features: Autoscale, IpRules, EnableFreeTier and EnableAnalyticalStorage</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5954-216">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e5954-216">EventGrid</span></span>

* <span data-ttu-id="e5954-217">Adicionar suporte de CLI para 2020-04-01-preview e marcar a versão prévia dos recursos com is_Preview=True</span><span class="sxs-lookup"><span data-stu-id="e5954-217">Add CLI support for 2020-04-01-preview and mark preview features with is_Preview=True</span></span>

### <a name="find"></a><span data-ttu-id="e5954-218">Localizar</span><span class="sxs-lookup"><span data-stu-id="e5954-218">Find</span></span>

* <span data-ttu-id="e5954-219">Correção nº 14094 az find Corrige consultas que falhavam quando não estavam conectadas e quando a telemetria estava desabilitada</span><span class="sxs-lookup"><span data-stu-id="e5954-219">Fix #14094 az find Fix Queries failing when not logged in and when telemetry is disabled</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-220">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-220">HDInsight</span></span>

* <span data-ttu-id="e5954-221">Adicionar dois comandos para dar suporte ao recurso de reinicialização do nó do hdinsight</span><span class="sxs-lookup"><span data-stu-id="e5954-221">Add two commands to support hdinsight node reboot feature</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-222">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-222">Monitor</span></span>

* <span data-ttu-id="e5954-223">Remover sinalizador de visualização para comandos no workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-223">Remove preview flag for commands under Log Analytics workspace</span></span>
* <span data-ttu-id="e5954-224">`az monitor diagnostic-settings subscription`: Dar suporte às configurações de diagnóstico para a assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-224">`az monitor diagnostic-settings subscription`: Support diagnositc settings for subscription</span></span>
* <span data-ttu-id="e5954-225">`az monitor metrics`: dá suporte para ', ' e '|' no nome da métrica</span><span class="sxs-lookup"><span data-stu-id="e5954-225">`az monitor metrics`: support ',' and '|' in metric name</span></span>
* <span data-ttu-id="e5954-226">`az monitor log-analytics workspace data-export`: suporte à exportação de dados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-226">`az monitor log-analytics workspace data-export`: support log analytics data export</span></span>

### <a name="network"></a><span data-ttu-id="e5954-227">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-227">Network</span></span>

* <span data-ttu-id="e5954-228">`az network application-gateway frontend-ip update`: Substituir o parâmetro --public-ip-address</span><span class="sxs-lookup"><span data-stu-id="e5954-228">`az network application-gateway frontend-ip update`: Deprecating the --public-ip-address parameter</span></span>
* <span data-ttu-id="e5954-229">Avançar azure-mgmt-network para 11.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-229">Bump azure-mgmt-network to 11.0.0</span></span>
* <span data-ttu-id="e5954-230">`az network express-route gateway connection`: dá suporte à configuração de roteamento</span><span class="sxs-lookup"><span data-stu-id="e5954-230">`az network express-route gateway connection`: support routing configuration</span></span>
* <span data-ttu-id="e5954-231">`az network virtual-appliance`: dá suporte à solução de virtualização de rede do Azure.</span><span class="sxs-lookup"><span data-stu-id="e5954-231">`az network virtual-appliance`: Support Azure network virtual appliance.</span></span>
* <span data-ttu-id="e5954-232">Recurso de link privado de suporte do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-232">Application Gateway support private link feature</span></span>

### <a name="policyinsights"></a><span data-ttu-id="e5954-233">PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e5954-233">PolicyInsights</span></span>

* <span data-ttu-id="e5954-234">`az policy state`: adiciona o comando trigger-scan para disparar avaliações de conformidade de política</span><span class="sxs-lookup"><span data-stu-id="e5954-234">`az policy state`: add trigger-scan command to trigger policy compliance evaluations</span></span>
* <span data-ttu-id="e5954-235">`az policy state list`: expõe versões de entidades de política em cada registro de conformidade</span><span class="sxs-lookup"><span data-stu-id="e5954-235">`az policy state list`: expose versions of policy entities in each compliance record</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-236">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-236">Profile</span></span>

* <span data-ttu-id="e5954-237">`az account get-access-token`: Mostra expiresOn para Identidade Gerenciada</span><span class="sxs-lookup"><span data-stu-id="e5954-237">`az account get-access-token`: Show expiresOn for Managed Identity</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-238">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-238">RDBMS</span></span>

* <span data-ttu-id="e5954-239">Dar suporte à versão mínima do TLS</span><span class="sxs-lookup"><span data-stu-id="e5954-239">Support Minimum TLS version</span></span>
* <span data-ttu-id="e5954-240">Adicionar criptografia de infraestrutura para o Azure Postgres e MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-240">Add Infrastructure Encryption for Azure Postgres and MySQL</span></span>

### <a name="security"></a><span data-ttu-id="e5954-241">Segurança</span><span class="sxs-lookup"><span data-stu-id="e5954-241">Security</span></span>

* <span data-ttu-id="e5954-242">Adicionar comandos allowed_connections</span><span class="sxs-lookup"><span data-stu-id="e5954-242">Add allowed_connections commands</span></span>
* <span data-ttu-id="e5954-243">Adicionar comandos hardeningss da rede adaptável</span><span class="sxs-lookup"><span data-stu-id="e5954-243">Add Adaptive network hardeningss commands</span></span>
* <span data-ttu-id="e5954-244">Adicionar comandos adaptive_application_controls</span><span class="sxs-lookup"><span data-stu-id="e5954-244">Add adaptive_application_controls commands</span></span>
* <span data-ttu-id="e5954-245">Adição de az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST à CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-245">Addition of az security iot-solution/ iot-alerts/iot-recommendations/iot-analytics REST to Azure CLI</span></span>
* <span data-ttu-id="e5954-246">Adicionar CLI de conformidade regulatória</span><span class="sxs-lookup"><span data-stu-id="e5954-246">Add regulatory compliance CLI</span></span>

### <a name="signalr"></a><span data-ttu-id="e5954-247">SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-247">SignalR</span></span>

* <span data-ttu-id="e5954-248">Adicionar recursos, incluindo o gerenciamento de conexões de ponto de extremidade privado, regras de rede e upstream</span><span class="sxs-lookup"><span data-stu-id="e5954-248">Add features including managing private endpoint connections, network rules and upstream</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-249">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-249">SQL</span></span>

* <span data-ttu-id="e5954-250">`az sql mi create`, `az sql mi update`: adiciona o parâmetro `--tags` para dar suporte à marcação de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-250">`az sql mi create`, `az sql mi update`: Add `--tags` parameter to support resource tagging</span></span>
* <span data-ttu-id="e5954-251">`az sql mi failover`: dá suporte ao failover de um ponto primário ou secundário</span><span class="sxs-lookup"><span data-stu-id="e5954-251">`az sql mi failover`: Support failover from primary or secondary point</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-252">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-252">Storage</span></span>

* <span data-ttu-id="e5954-253">`az storage account create/update`: adiciona --allow-blob-public-access para permitir ou não permitir acesso público para blob e contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-253">`az storage account create/update`: Add --allow-blob-public-access to allow or disallow public access for blob and containers</span></span>
* <span data-ttu-id="e5954-254">`az storage account create/update`: adiciona `--min-tls-version` para dar suporte à definição da versão mínima do TLS a ser permitida em solicitações de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-254">`az storage account create/update`: Add `--min-tls-version` to support setting the minimum TLS version to be permitted on requests to storage.</span></span>
* <span data-ttu-id="e5954-255">Remover credencial de token de check-in</span><span class="sxs-lookup"><span data-stu-id="e5954-255">Remove check in token credential</span></span>
* <span data-ttu-id="e5954-256">Corrigir o nome da conta de armazenamento em exemplos</span><span class="sxs-lookup"><span data-stu-id="e5954-256">Fix the storage account name in examples</span></span>

### <a name="webapp"></a><span data-ttu-id="e5954-257">Webapp</span><span class="sxs-lookup"><span data-stu-id="e5954-257">Webapp</span></span>

* <span data-ttu-id="e5954-258">Bugfix: az webapp log deployment show – retorna logs de implantação em vez de metadados de log</span><span class="sxs-lookup"><span data-stu-id="e5954-258">Bugfix: az webapp log deployment show - return deployment logs instead of log metadata</span></span>
* <span data-ttu-id="e5954-259">Bugfix: az webapp vnet-integration add – corrige o tratamento de erro se o nome da VNet é inadequado, dá suporte à ID do recurso da vnet</span><span class="sxs-lookup"><span data-stu-id="e5954-259">Bugfix: az webapp vnet-integration add - fix error handling if bad vnet name, support vnet resource ID</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="e5954-260">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-260">June 23, 2020</span></span>

<span data-ttu-id="e5954-261">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="e5954-261">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-262">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-262">ACR</span></span>

* <span data-ttu-id="e5954-263">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="e5954-263">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="e5954-264">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="e5954-264">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-265">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-265">ACS</span></span>

* <span data-ttu-id="e5954-266">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="e5954-266">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-267">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-267">AKS</span></span>

* <span data-ttu-id="e5954-268">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="e5954-268">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="e5954-269">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="e5954-269">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="e5954-270">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="e5954-270">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="e5954-271">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="e5954-271">Fix typo in az aks update command</span></span>
* <span data-ttu-id="e5954-272">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="e5954-272">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="e5954-273">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-273">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-274">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-274">AMS</span></span>

* <span data-ttu-id="e5954-275">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="e5954-275">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-276">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-276">AppService</span></span>

* <span data-ttu-id="e5954-277">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="e5954-277">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="e5954-278">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="e5954-278">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="e5954-279">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-279">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="e5954-280">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="e5954-280">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="e5954-281">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="e5954-281">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="e5954-282">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="e5954-282">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="e5954-283">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-283">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="e5954-284">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="e5954-284">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="e5954-285">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-285">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="e5954-286">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="e5954-286">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="e5954-287">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="e5954-287">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-288">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-288">ARM</span></span>

* <span data-ttu-id="e5954-289">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="e5954-289">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="e5954-290">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="e5954-290">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="e5954-291">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="e5954-291">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="e5954-292">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="e5954-292">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="e5954-293">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="e5954-293">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="e5954-294">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="e5954-294">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="e5954-295">ARO</span><span class="sxs-lookup"><span data-stu-id="e5954-295">ARO</span></span>

* <span data-ttu-id="e5954-296">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="e5954-296">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-297">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-297">Batch</span></span>

* <span data-ttu-id="e5954-298">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="e5954-298">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="e5954-299">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="e5954-299">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="e5954-300">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="e5954-300">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="e5954-301">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="e5954-301">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="e5954-302">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e5954-302">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="e5954-303">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="e5954-303">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="e5954-304">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="e5954-304">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="e5954-305">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="e5954-305">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-306">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-306">CDN</span></span>

* <span data-ttu-id="e5954-307">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="e5954-307">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="e5954-308">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e5954-308">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5954-309">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-309">Cognitive Services</span></span>

* <span data-ttu-id="e5954-310">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="e5954-310">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="e5954-311">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="e5954-311">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-312">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-312">Compute</span></span>

* <span data-ttu-id="e5954-313">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="e5954-313">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="e5954-314">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="e5954-314">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="e5954-315">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-315">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="e5954-316">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="e5954-316">New command `az image builder cancel`</span></span>
* <span data-ttu-id="e5954-317">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="e5954-317">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-318">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-318">Cosmos DB</span></span>

* <span data-ttu-id="e5954-319">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-319">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="e5954-320">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="e5954-320">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5954-321">EventHub</span><span class="sxs-lookup"><span data-stu-id="e5954-321">EventHub</span></span>

* <span data-ttu-id="e5954-322">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e5954-322">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-323">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-323">Extension</span></span>

* <span data-ttu-id="e5954-324">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="e5954-324">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="e5954-325">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="e5954-325">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="e5954-326">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-326">Iot Hub</span></span>

* <span data-ttu-id="e5954-327">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-327">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-328">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-328">KeyVault</span></span>

* <span data-ttu-id="e5954-329">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="e5954-329">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="e5954-330">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="e5954-330">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-331">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-331">Monitor</span></span>

* <span data-ttu-id="e5954-332">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-332">Support no wait for cluster creation</span></span>
* <span data-ttu-id="e5954-333">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="e5954-333">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="e5954-334">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-334">Network</span></span>

* <span data-ttu-id="e5954-335">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="e5954-335">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="e5954-336">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="e5954-336">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="e5954-337">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="e5954-337">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="e5954-338">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="e5954-338">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-339">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-339">RBAC</span></span>

* <span data-ttu-id="e5954-340">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="e5954-340">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="e5954-341">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-341">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="e5954-342">Segurança</span><span class="sxs-lookup"><span data-stu-id="e5954-342">Security</span></span>

* <span data-ttu-id="e5954-343">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="e5954-343">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-344">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-344">SQL</span></span>

* <span data-ttu-id="e5954-345">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="e5954-345">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-346">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-346">Storage</span></span>

* <span data-ttu-id="e5954-347">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="e5954-347">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="e5954-348">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="e5954-348">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="e5954-349">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="e5954-349">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="e5954-350">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="e5954-350">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="e5954-351">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="e5954-351">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="e5954-352">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="e5954-352">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="e5954-353">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="e5954-353">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="e5954-354">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="e5954-354">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="e5954-355">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="e5954-355">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="e5954-356">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="e5954-356">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="e5954-357">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-357">June 02, 2020</span></span>

<span data-ttu-id="e5954-358">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="e5954-358">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-359">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-359">ACR</span></span>

* <span data-ttu-id="e5954-360">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="e5954-360">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-361">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-361">AKS</span></span>

* <span data-ttu-id="e5954-362">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="e5954-362">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="e5954-363">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="e5954-363">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-364">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-364">AppService</span></span>

* <span data-ttu-id="e5954-365">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="e5954-365">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-366">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-366">ARM</span></span>

* <span data-ttu-id="e5954-367">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="e5954-367">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="e5954-368">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="e5954-368">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="e5954-369">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-369">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="e5954-370">ARO</span><span class="sxs-lookup"><span data-stu-id="e5954-370">ARO</span></span>

* <span data-ttu-id="e5954-371">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="e5954-371">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5954-372">EventHub</span><span class="sxs-lookup"><span data-stu-id="e5954-372">EventHub</span></span>

* <span data-ttu-id="e5954-373">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="e5954-373">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-374">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-374">HDInsight</span></span>

* <span data-ttu-id="e5954-375">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="e5954-375">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-376">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-376">Monitor</span></span>

* <span data-ttu-id="e5954-377">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-377">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="e5954-378">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="e5954-378">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="e5954-379">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="e5954-379">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="e5954-380">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-380">Network</span></span>

* <span data-ttu-id="e5954-381">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="e5954-381">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="e5954-382">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="e5954-382">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="e5954-383">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="e5954-383">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="e5954-384">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-384">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="e5954-385">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-385">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-386">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-386">Packaging</span></span>

* <span data-ttu-id="e5954-387">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="e5954-387">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-388">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-388">RBAC</span></span>

* <span data-ttu-id="e5954-389">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="e5954-389">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-390">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-390">Redis</span></span>

* <span data-ttu-id="e5954-391">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="e5954-391">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-392">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-392">Storage</span></span>

* <span data-ttu-id="e5954-393">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="e5954-393">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="e5954-394">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-394">Enable local context for storage account</span></span>
* <span data-ttu-id="e5954-395">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="e5954-395">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="e5954-396">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-396">May 19, 2020</span></span>

<span data-ttu-id="e5954-397">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="e5954-397">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-398">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-398">ACR</span></span>

* <span data-ttu-id="e5954-399">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-399">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="e5954-400">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="e5954-400">Support disable public network access</span></span>
* <span data-ttu-id="e5954-401">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="e5954-401">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="e5954-402">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="e5954-402">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-403">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-403">ACS</span></span>

* <span data-ttu-id="e5954-404">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="e5954-404">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-405">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-405">AKS</span></span>

* <span data-ttu-id="e5954-406">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="e5954-406">Update uptime-sla command help context</span></span>
* <span data-ttu-id="e5954-407">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="e5954-407">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="e5954-408">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-408">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-409">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-409">AMS</span></span>

* <span data-ttu-id="e5954-410">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="e5954-410">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="e5954-411">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="e5954-411">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-412">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-412">AppConfig</span></span>

* <span data-ttu-id="e5954-413">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="e5954-413">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-414">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-414">AppService</span></span>

* <span data-ttu-id="e5954-415">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="e5954-415">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="e5954-416">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="e5954-416">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="e5954-417">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="e5954-417">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="e5954-418">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-418">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-419">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-419">ARM</span></span>

* <span data-ttu-id="e5954-420">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="e5954-420">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="e5954-421">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="e5954-421">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="e5954-422">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="e5954-422">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="e5954-423">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="e5954-423">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="e5954-424">ARO</span><span class="sxs-lookup"><span data-stu-id="e5954-424">ARO</span></span>

* <span data-ttu-id="e5954-425">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="e5954-425">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="e5954-426">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="e5954-426">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-427">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-427">Backup</span></span>

* <span data-ttu-id="e5954-428">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="e5954-428">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="e5954-429">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="e5954-429">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="e5954-430">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="e5954-430">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="e5954-431">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="e5954-431">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="e5954-432">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-432">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="e5954-433">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="e5954-433">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="e5954-434">CI</span><span class="sxs-lookup"><span data-stu-id="e5954-434">CI</span></span>

* <span data-ttu-id="e5954-435">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="e5954-435">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-436">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-436">Compute</span></span>

* <span data-ttu-id="e5954-437">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="e5954-437">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="e5954-438">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="e5954-438">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="e5954-439">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-439">Core</span></span>

* <span data-ttu-id="e5954-440">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="e5954-440">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-441">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-441">Extension</span></span>

* <span data-ttu-id="e5954-442">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="e5954-442">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="e5954-443">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="e5954-443">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-444">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-444">IoT</span></span>

* <span data-ttu-id="e5954-445">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="e5954-445">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="e5954-446">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-446">IoT Hub</span></span>

* <span data-ttu-id="e5954-447">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="e5954-447">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="e5954-448">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="e5954-448">NetAppFiles</span></span>

* <span data-ttu-id="e5954-449">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="e5954-449">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="e5954-450">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-450">Network</span></span>

* <span data-ttu-id="e5954-451">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="e5954-451">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="e5954-452">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="e5954-452">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="e5954-453">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="e5954-453">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="e5954-454">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="e5954-454">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="e5954-455">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e5954-455">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="e5954-456">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="e5954-456">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="e5954-457">Saída</span><span class="sxs-lookup"><span data-stu-id="e5954-457">Output</span></span>

* <span data-ttu-id="e5954-458">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="e5954-458">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-459">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-459">Packaging</span></span>

* <span data-ttu-id="e5954-460">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="e5954-460">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-461">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-461">RBAC</span></span>

* <span data-ttu-id="e5954-462">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="e5954-462">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-463">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-463">Storage</span></span>

* <span data-ttu-id="e5954-464">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-464">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="e5954-465">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="e5954-465">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="e5954-466">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="e5954-466">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="e5954-467">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="e5954-467">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="e5954-468">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="e5954-468">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="e5954-469">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-469">April 30, 2020</span></span>

<span data-ttu-id="e5954-470">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="e5954-470">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-471">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-471">ACR</span></span>

* <span data-ttu-id="e5954-472">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-472">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-473">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-473">Compute</span></span>

* <span data-ttu-id="e5954-474">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="e5954-474">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="e5954-475">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-475">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="e5954-476">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="e5954-476">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-477">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-477">Cosmos DB</span></span>

* <span data-ttu-id="e5954-478">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="e5954-478">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-479">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-479">Extension</span></span>

* <span data-ttu-id="e5954-480">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="e5954-480">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-481">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-481">Packaging</span></span>

* <span data-ttu-id="e5954-482">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-482">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-483">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-483">SQL</span></span>

* <span data-ttu-id="e5954-484">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="e5954-484">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-485">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-485">Storage</span></span>

* <span data-ttu-id="e5954-486">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="e5954-486">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="e5954-487">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-487">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="e5954-488">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="e5954-488">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="e5954-489">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="e5954-489">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="e5954-490">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-490">April 28, 2020</span></span>

<span data-ttu-id="e5954-491">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="e5954-491">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-492">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-492">ACS</span></span>

* <span data-ttu-id="e5954-493">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="e5954-493">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="e5954-494">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="e5954-494">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="e5954-495">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="e5954-495">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="e5954-496">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="e5954-496">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-497">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-497">AKS</span></span>

* <span data-ttu-id="e5954-498">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-498">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-499">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-499">AppService</span></span>

* <span data-ttu-id="e5954-500">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="e5954-500">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-501">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-501">ARM</span></span>

* <span data-ttu-id="e5954-502">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="e5954-502">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="e5954-503">ARO</span><span class="sxs-lookup"><span data-stu-id="e5954-503">ARO</span></span>

* <span data-ttu-id="e5954-504">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-504">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="e5954-505">CI</span><span class="sxs-lookup"><span data-stu-id="e5954-505">CI</span></span>

* <span data-ttu-id="e5954-506">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="e5954-506">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-507">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-507">Compute</span></span>

* <span data-ttu-id="e5954-508">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="e5954-508">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="e5954-509">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="e5954-509">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="e5954-510">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-510">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-511">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-511">KeyVault</span></span>

* <span data-ttu-id="e5954-512">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="e5954-512">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-513">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-513">Monitor</span></span>

* <span data-ttu-id="e5954-514">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="e5954-514">Support LA cluster CMK features</span></span>
* <span data-ttu-id="e5954-515">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="e5954-515">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="e5954-516">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-516">Network</span></span>

* <span data-ttu-id="e5954-517">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="e5954-517">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="e5954-518">Privatedns</span><span class="sxs-lookup"><span data-stu-id="e5954-518">Privatedns</span></span>

* <span data-ttu-id="e5954-519">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="e5954-519">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="e5954-520">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-520">April 21, 2020</span></span>

<span data-ttu-id="e5954-521">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="e5954-521">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-522">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-522">ACR</span></span>

* <span data-ttu-id="e5954-523">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-523">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="e5954-524">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="e5954-524">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-525">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-525">AKS</span></span>

* <span data-ttu-id="e5954-526">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="e5954-526">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="e5954-527">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="e5954-527">Add --uptime-sla</span></span>
* <span data-ttu-id="e5954-528">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="e5954-528">Update containerservice package</span></span>
* <span data-ttu-id="e5954-529">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="e5954-529">Add node public IP support</span></span>
* <span data-ttu-id="e5954-530">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-530">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-531">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-531">AppConfig</span></span>

* <span data-ttu-id="e5954-532">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="e5954-532">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="e5954-533">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="e5954-533">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-534">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-534">AppService</span></span>

* <span data-ttu-id="e5954-535">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="e5954-535">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="e5954-536">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="e5954-536">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="e5954-537">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="e5954-537">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="e5954-538">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="e5954-538">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="e5954-539">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="e5954-539">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-540">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-540">ARM</span></span>

* <span data-ttu-id="e5954-541">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="e5954-541">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="e5954-542">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-542">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="e5954-543">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="e5954-543">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="e5954-544">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="e5954-544">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="e5954-545">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="e5954-545">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="e5954-546">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="e5954-546">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="e5954-547">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="e5954-547">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="e5954-548">ARO</span><span class="sxs-lookup"><span data-stu-id="e5954-548">ARO</span></span>

* <span data-ttu-id="e5954-549">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="e5954-549">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-550">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-550">Batch</span></span>

* <span data-ttu-id="e5954-551">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-551">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-552">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-552">Compute</span></span>

* <span data-ttu-id="e5954-553">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="e5954-553">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="e5954-554">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="e5954-554">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="e5954-555">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="e5954-555">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="e5954-556">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="e5954-556">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="e5954-557">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="e5954-557">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="e5954-558">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="e5954-558">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-559">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-559">CosmosDB</span></span>

* <span data-ttu-id="e5954-560">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="e5954-560">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5954-561">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-561">IoT Central</span></span>

* <span data-ttu-id="e5954-562">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="e5954-562">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="e5954-563">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="e5954-563">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-564">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-564">Monitor</span></span>

* <span data-ttu-id="e5954-565">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-565">Support private link scenario for monitor</span></span>
* <span data-ttu-id="e5954-566">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="e5954-566">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="e5954-567">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-567">Network</span></span>

* <span data-ttu-id="e5954-568">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="e5954-568">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="e5954-569">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="e5954-569">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="e5954-570">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="e5954-570">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="e5954-571">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="e5954-571">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-572">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-572">Packaging</span></span>

* <span data-ttu-id="e5954-573">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="e5954-573">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-574">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-574">RBAC</span></span>

* <span data-ttu-id="e5954-575">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5954-575">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-576">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-576">RDBMS</span></span>

* <span data-ttu-id="e5954-577">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-577">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5954-578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-578">Service Fabric</span></span>

* <span data-ttu-id="e5954-579">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="e5954-579">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="e5954-580">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="e5954-580">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-581">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-581">SQL</span></span>

* <span data-ttu-id="e5954-582">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="e5954-582">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="e5954-583">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="e5954-583">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-584">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-584">Storage</span></span>

* <span data-ttu-id="e5954-585">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-585">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="e5954-586">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-586">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="e5954-587">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="e5954-587">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="e5954-588">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="e5954-588">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="e5954-589">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-589">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="e5954-590">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="e5954-590">Survey</span></span>

* <span data-ttu-id="e5954-591">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="e5954-591">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="e5954-592">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-592">April 01, 2020</span></span>

<span data-ttu-id="e5954-593">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="e5954-593">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-594">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-594">ACR</span></span>

* <span data-ttu-id="e5954-595">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-595">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-596">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-596">Profile</span></span>

* <span data-ttu-id="e5954-597">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="e5954-597">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="e5954-598">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-598">March 31, 2020</span></span>

<span data-ttu-id="e5954-599">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="e5954-599">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-600">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-600">ACR</span></span>

* <span data-ttu-id="e5954-601">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="e5954-601">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="e5954-602">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="e5954-602">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="e5954-603">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="e5954-603">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="e5954-604">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="e5954-604">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="e5954-605">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-605">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="e5954-606">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="e5954-606">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="e5954-607">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-607">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-608">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-608">AKS</span></span>

* <span data-ttu-id="e5954-609">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="e5954-609">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="e5954-610">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="e5954-610">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="e5954-611">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="e5954-611">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-612">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-612">AMS</span></span>

* <span data-ttu-id="e5954-613">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="e5954-613">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-614">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-614">AppConfig</span></span>

* <span data-ttu-id="e5954-615">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="e5954-615">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-616">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-616">AppService</span></span>

* <span data-ttu-id="e5954-617">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-617">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="e5954-618">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="e5954-618">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="e5954-619">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-619">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-620">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-620">ARM</span></span>

* <span data-ttu-id="e5954-621">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-621">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="e5954-622">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-622">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="e5954-623">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="e5954-623">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="e5954-624">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="e5954-624">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-625">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-625">Backup</span></span>

* <span data-ttu-id="e5954-626">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="e5954-626">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="e5954-627">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="e5954-627">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="e5954-628">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="e5954-628">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-629">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-629">Compute</span></span>

* <span data-ttu-id="e5954-630">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="e5954-630">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="e5954-631">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="e5954-631">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="e5954-632">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="e5954-632">az vm update: Support --workspace</span></span>
* <span data-ttu-id="e5954-633">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="e5954-633">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="e5954-634">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="e5954-634">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="e5954-635">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="e5954-635">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="e5954-636">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="e5954-636">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="e5954-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="e5954-637">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-638">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-638">Cosmos DB</span></span>

* <span data-ttu-id="e5954-639">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="e5954-639">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="e5954-640">Docker</span><span class="sxs-lookup"><span data-stu-id="e5954-640">Docker</span></span>

* <span data-ttu-id="e5954-641">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="e5954-641">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-642">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-642">Extension</span></span>

* <span data-ttu-id="e5954-643">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="e5954-643">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-644">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-644">HDInsight</span></span>

* <span data-ttu-id="e5954-645">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="e5954-645">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="e5954-646">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="e5954-646">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-647">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-647">IoT</span></span>

* <span data-ttu-id="e5954-648">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="e5954-648">Add codeowner</span></span>
* <span data-ttu-id="e5954-649">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="e5954-649">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="e5954-650">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="e5954-650">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e5954-651">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-651">IoTCentral</span></span>

* <span data-ttu-id="e5954-652">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="e5954-652">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-653">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-653">KeyVault</span></span>

* <span data-ttu-id="e5954-654">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="e5954-654">Support certificate backup/restore</span></span>
* <span data-ttu-id="e5954-655">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="e5954-655">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="e5954-656">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="e5954-656">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="e5954-657">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="e5954-657">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="e5954-658">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="e5954-658">Lock</span></span>

* <span data-ttu-id="e5954-659">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e5954-659">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-660">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-660">Monitor</span></span>

* <span data-ttu-id="e5954-661">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="e5954-661">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="e5954-662">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="e5954-662">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="e5954-663">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="e5954-663">NetAppFiles</span></span>

* <span data-ttu-id="e5954-664">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="e5954-664">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="e5954-665">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-665">Network</span></span>

* <span data-ttu-id="e5954-666">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="e5954-666">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="e5954-667">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="e5954-667">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="e5954-668">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-668">support host names in application gateway listener</span></span>
* <span data-ttu-id="e5954-669">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="e5954-669">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="e5954-670">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="e5954-670">Support vpn gateway generation</span></span>
* <span data-ttu-id="e5954-671">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="e5954-671">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-672">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-672">Packaging</span></span>

* <span data-ttu-id="e5954-673">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="e5954-673">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-674">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-674">Profile</span></span>

* <span data-ttu-id="e5954-675">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="e5954-675">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-676">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-676">RDBMS</span></span>

* <span data-ttu-id="e5954-677">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-677">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="e5954-678">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-678">March 10, 2020</span></span>

<span data-ttu-id="e5954-679">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="e5954-679">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-680">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-680">ACR</span></span>

* <span data-ttu-id="e5954-681">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-681">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="e5954-682">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="e5954-682">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="e5954-683">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="e5954-683">Add private link and CMK support</span></span>
* <span data-ttu-id="e5954-684">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="e5954-684">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-685">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-685">AKS</span></span>

* <span data-ttu-id="e5954-686">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5954-686">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="e5954-687">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="e5954-687">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="e5954-688">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-688">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="e5954-689">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-689">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="e5954-690">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="e5954-690">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="e5954-691">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-691">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="e5954-692">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-692">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="e5954-693">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="e5954-693">add missing / in the dashboard url</span></span>
* <span data-ttu-id="e5954-694">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e5954-694">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="e5954-695">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="e5954-695">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="e5954-696">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="e5954-696">az aks: Add aad session key support</span></span>
* <span data-ttu-id="e5954-697">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="e5954-697">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="e5954-698">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="e5954-698">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-699">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-699">AppConfig</span></span>

* <span data-ttu-id="e5954-700">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="e5954-700">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-701">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-701">AppService</span></span>

* <span data-ttu-id="e5954-702">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="e5954-702">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="e5954-703">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="e5954-703">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="e5954-704">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="e5954-704">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="e5954-705">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-705">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="e5954-706">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-706">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="e5954-707">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="e5954-707">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-708">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-708">ARM</span></span>

* <span data-ttu-id="e5954-709">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-709">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="e5954-710">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="e5954-710">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="e5954-711">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="e5954-711">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="e5954-712">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="e5954-712">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="e5954-713">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="e5954-713">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="e5954-714">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="e5954-714">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="e5954-715">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-715">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="e5954-716">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="e5954-716">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="e5954-717">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="e5954-717">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="e5954-718">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="e5954-718">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-719">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-719">CDN</span></span>

* <span data-ttu-id="e5954-720">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-720">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-721">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-721">Compute</span></span>

* <span data-ttu-id="e5954-722">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="e5954-722">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="e5954-723">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="e5954-723">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="e5954-724">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="e5954-724">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="e5954-725">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="e5954-725">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="e5954-726">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="e5954-726">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-727">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-727">Cosmos DB</span></span>

* <span data-ttu-id="e5954-728">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="e5954-728">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="e5954-729">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="e5954-729">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-730">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-730">KeyVault</span></span>

* <span data-ttu-id="e5954-731">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-731">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-732">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-732">Monitor</span></span>

* <span data-ttu-id="e5954-733">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="e5954-733">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-734">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-734">Network</span></span>

* <span data-ttu-id="e5954-735">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="e5954-735">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="e5954-736">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="e5954-736">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="e5954-737">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="e5954-737">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="e5954-738">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="e5954-738">az network bastion: support bastion</span></span>
* <span data-ttu-id="e5954-739">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="e5954-739">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="e5954-740">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="e5954-740">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="e5954-741">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-741">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="e5954-742">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="e5954-742">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="e5954-743">Política</span><span class="sxs-lookup"><span data-stu-id="e5954-743">Policy</span></span>

* <span data-ttu-id="e5954-744">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="e5954-744">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-745">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-745">RBAC</span></span>

* <span data-ttu-id="e5954-746">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="e5954-746">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-747">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-747">RDBMS</span></span>

* <span data-ttu-id="e5954-748">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-748">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="e5954-749">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="e5954-749">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="e5954-750">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="e5954-750">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="e5954-751">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-751">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="e5954-752">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-752">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="e5954-753">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="e5954-753">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="e5954-754">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="e5954-754">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="e5954-755">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-755">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-756">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-756">SQL</span></span>

* <span data-ttu-id="e5954-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="e5954-757">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="e5954-758">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="e5954-758">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="e5954-759">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="e5954-759">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="e5954-760">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-760">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-761">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-761">Storage</span></span>

* <span data-ttu-id="e5954-762">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="e5954-762">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="e5954-763">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="e5954-763">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="e5954-764">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="e5954-764">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="e5954-765">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-765">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="e5954-766">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="e5954-766">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="e5954-767">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-767">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="e5954-768">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="e5954-768">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="e5954-769">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="e5954-769">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="e5954-770">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="e5954-770">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="e5954-771">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-771">February 18, 2020</span></span>

<span data-ttu-id="e5954-772">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="e5954-772">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-773">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-773">ACR</span></span>

* <span data-ttu-id="e5954-774">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="e5954-774">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="e5954-775">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="e5954-775">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="e5954-776">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="e5954-776">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-777">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-777">ACS</span></span>

* <span data-ttu-id="e5954-778">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="e5954-778">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="e5954-779">Aladdin</span><span class="sxs-lookup"><span data-stu-id="e5954-779">Aladdin</span></span>

* <span data-ttu-id="e5954-780">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="e5954-780">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-781">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-781">AMS</span></span>

* <span data-ttu-id="e5954-782">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="e5954-782">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-783">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-783">AppConfig</span></span>

* <span data-ttu-id="e5954-784">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="e5954-784">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="e5954-785">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="e5954-785">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="e5954-786">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="e5954-786">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-787">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-787">AppService</span></span>

* <span data-ttu-id="e5954-788">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="e5954-788">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="e5954-789">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="e5954-789">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="e5954-790">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="e5954-790">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-791">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-791">ARM</span></span>

* <span data-ttu-id="e5954-792">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-792">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="e5954-793">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="e5954-793">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-794">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-794">Backup</span></span>

* <span data-ttu-id="e5954-795">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="e5954-795">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="e5954-796">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="e5954-796">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-797">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-797">Compute</span></span>

* <span data-ttu-id="e5954-798">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="e5954-798">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="e5954-799">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="e5954-799">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="e5954-800">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="e5954-800">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="e5954-801">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="e5954-801">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="e5954-802">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="e5954-802">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5954-803">Eventhub</span><span class="sxs-lookup"><span data-stu-id="e5954-803">Eventhub</span></span>

* <span data-ttu-id="e5954-804">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="e5954-804">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-805">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-805">KeyVault</span></span>

* <span data-ttu-id="e5954-806">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="e5954-806">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="e5954-807">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="e5954-807">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="e5954-808">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="e5954-808">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="e5954-809">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-809">Network</span></span>

* <span data-ttu-id="e5954-810">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-810">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="e5954-811">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="e5954-811">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="e5954-812">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="e5954-812">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-813">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-813">Packaging</span></span>

* <span data-ttu-id="e5954-814">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="e5954-814">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-815">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-815">Profile</span></span>

* <span data-ttu-id="e5954-816">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="e5954-816">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="e5954-817">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="e5954-817">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="e5954-818">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="e5954-818">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="e5954-819">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="e5954-819">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="e5954-820">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-820">Role</span></span>

* <span data-ttu-id="e5954-821">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="e5954-821">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-822">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-822">SQL</span></span>

* <span data-ttu-id="e5954-823">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="e5954-823">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-824">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-824">Storage</span></span>

* <span data-ttu-id="e5954-825">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="e5954-825">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="e5954-826">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-826">February 04, 2020</span></span>

<span data-ttu-id="e5954-827">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="e5954-827">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-828">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-828">ACS</span></span>

* <span data-ttu-id="e5954-829">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="e5954-829">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="e5954-830">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="e5954-830">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-831">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-831">ACR</span></span>

* <span data-ttu-id="e5954-832">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="e5954-832">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="e5954-833">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="e5954-833">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="e5954-834">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="e5954-834">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-835">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-835">AKS</span></span>

* <span data-ttu-id="e5954-836">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="e5954-836">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-837">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-837">AppConfig</span></span>

* <span data-ttu-id="e5954-838">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="e5954-838">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="e5954-839">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="e5954-839">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="e5954-840">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="e5954-840">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="e5954-841">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="e5954-841">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="e5954-842">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="e5954-842">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-843">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-843">AppService</span></span>

* <span data-ttu-id="e5954-844">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="e5954-844">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="e5954-845">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-845">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-846">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-846">ARM</span></span>

* <span data-ttu-id="e5954-847">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-847">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="e5954-848">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="e5954-848">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="e5954-849">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="e5954-849">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="e5954-850">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="e5954-850">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="e5954-851">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="e5954-851">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="e5954-852">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-852">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="e5954-853">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-853">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-854">BotService</span><span class="sxs-lookup"><span data-stu-id="e5954-854">BotService</span></span>

* <span data-ttu-id="e5954-855">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="e5954-855">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="e5954-856">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="e5954-856">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-857">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-857">CDN</span></span>

* <span data-ttu-id="e5954-858">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="e5954-858">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="e5954-859">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="e5954-859">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="e5954-860">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="e5954-860">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="e5954-861">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-861">Deployment Manager</span></span>

* <span data-ttu-id="e5954-862">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="e5954-862">Add list operation for all resources.</span></span>
* <span data-ttu-id="e5954-863">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="e5954-863">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="e5954-864">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="e5954-864">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-865">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-865">IoT</span></span>

* <span data-ttu-id="e5954-866">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="e5954-866">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5954-867">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-867">IoT Central</span></span>

* <span data-ttu-id="e5954-868">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="e5954-868">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-869">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-869">Key Vault</span></span>

* <span data-ttu-id="e5954-870">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="e5954-870">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="e5954-871">Diversos</span><span class="sxs-lookup"><span data-stu-id="e5954-871">Misc</span></span>

* <span data-ttu-id="e5954-872">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="e5954-872">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="e5954-873">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-873">Network</span></span>

* <span data-ttu-id="e5954-874">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="e5954-874">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="e5954-875">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="e5954-875">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="e5954-876">Política</span><span class="sxs-lookup"><span data-stu-id="e5954-876">Policy</span></span>

* <span data-ttu-id="e5954-877">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="e5954-877">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="e5954-878">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="e5954-878">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-879">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-879">Profile</span></span>

* <span data-ttu-id="e5954-880">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-880">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-881">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-881">RBAC</span></span>

* <span data-ttu-id="e5954-882">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="e5954-882">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="e5954-883">Segurança</span><span class="sxs-lookup"><span data-stu-id="e5954-883">Security</span></span>

* <span data-ttu-id="e5954-884">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-884">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-885">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-885">SQL</span></span>

* <span data-ttu-id="e5954-886">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="e5954-886">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="e5954-887">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="e5954-887">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="e5954-888">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="e5954-888">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="e5954-889">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="e5954-889">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="e5954-890">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="e5954-890">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="e5954-891">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="e5954-891">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-892">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-892">Storage</span></span>

* <span data-ttu-id="e5954-893">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="e5954-893">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="e5954-894">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="e5954-894">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="e5954-895">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="e5954-895">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="e5954-896">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="e5954-896">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="e5954-897">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="e5954-897">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="e5954-898">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="e5954-898">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e5954-899">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e5954-899">ServiceFabric</span></span>

* <span data-ttu-id="e5954-900">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="e5954-900">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="e5954-901">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-901">January 13, 2020</span></span>

<span data-ttu-id="e5954-902">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="e5954-902">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-903">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-903">Compute</span></span>

* <span data-ttu-id="e5954-904">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="e5954-904">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="e5954-905">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="e5954-905">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-906">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-906">Storage</span></span>

* <span data-ttu-id="e5954-907">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="e5954-907">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="e5954-908">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="e5954-908">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="e5954-909">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-909">January 07, 2020</span></span>

<span data-ttu-id="e5954-910">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="e5954-910">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-911">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-911">ACR</span></span>

* <span data-ttu-id="e5954-912">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="e5954-912">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="e5954-913">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="e5954-913">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-914">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-914">AppConfig</span></span>

* <span data-ttu-id="e5954-915">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-915">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="e5954-916">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-916">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="e5954-917">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="e5954-917">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-918">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-918">AppService</span></span>

* <span data-ttu-id="e5954-919">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="e5954-919">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="e5954-920">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="e5954-920">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="e5954-921">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="e5954-921">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-922">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-922">ARM</span></span>

* <span data-ttu-id="e5954-923">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="e5954-923">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-924">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-924">Backup</span></span>

* <span data-ttu-id="e5954-925">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="e5954-925">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="e5954-926">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="e5954-926">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="e5954-927">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="e5954-927">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-928">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-928">Compute</span></span>

* <span data-ttu-id="e5954-929">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e5954-929">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="e5954-930">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="e5954-930">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="e5954-931">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="e5954-931">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-932">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-932">HDInsight</span></span>

* <span data-ttu-id="e5954-933">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="e5954-933">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="e5954-934">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="e5954-934">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="e5954-935">Diversos.</span><span class="sxs-lookup"><span data-stu-id="e5954-935">Misc.</span></span>

* <span data-ttu-id="e5954-936">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="e5954-936">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="e5954-937">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-937">Event Hubs</span></span>

* <span data-ttu-id="e5954-938">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="e5954-938">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="e5954-939">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="e5954-939">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5954-940">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-940">Service Bus</span></span>

* <span data-ttu-id="e5954-941">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="e5954-941">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="e5954-942">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="e5954-942">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-943">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-943">RBAC</span></span>

* <span data-ttu-id="e5954-944">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="e5954-944">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-945">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-945">Storage</span></span>

* <span data-ttu-id="e5954-946">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="e5954-946">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="e5954-947">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="e5954-947">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="e5954-948">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="e5954-948">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="e5954-949">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-949">December 17, 2019</span></span>

<span data-ttu-id="e5954-950">2.0.78</span><span class="sxs-lookup"><span data-stu-id="e5954-950">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-951">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-951">ACR</span></span>

* <span data-ttu-id="e5954-952">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="e5954-952">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-953">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-953">ACS</span></span>

* <span data-ttu-id="e5954-954">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="e5954-954">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-955">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-955">AMS</span></span>

* <span data-ttu-id="e5954-956">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="e5954-956">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-957">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-957">AppConfig</span></span>

* <span data-ttu-id="e5954-958">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5954-958">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="e5954-959">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="e5954-959">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="e5954-960">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="e5954-960">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-961">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-961">AppService</span></span>

* <span data-ttu-id="e5954-962">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="e5954-962">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="e5954-963">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="e5954-963">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="e5954-964">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="e5954-964">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="e5954-965">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="e5954-965">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-966">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-966">ARM</span></span>

* <span data-ttu-id="e5954-967">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-967">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="e5954-968">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="e5954-968">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="e5954-969">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="e5954-969">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-970">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-970">Backup</span></span>

* <span data-ttu-id="e5954-971">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="e5954-971">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-972">BotService</span><span class="sxs-lookup"><span data-stu-id="e5954-972">BotService</span></span>

* <span data-ttu-id="e5954-973">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="e5954-973">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="e5954-974">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="e5954-974">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="e5954-975">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="e5954-975">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="e5954-976">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="e5954-976">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="e5954-977">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="e5954-977">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="e5954-978">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="e5954-978">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="e5954-979">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="e5954-979">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="e5954-980">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="e5954-980">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="e5954-981">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="e5954-981">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-982">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-982">Compute</span></span>

* <span data-ttu-id="e5954-983">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-983">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="e5954-984">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-984">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="e5954-985">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-985">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="e5954-986">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="e5954-986">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="e5954-987">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="e5954-987">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="e5954-988">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="e5954-988">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="e5954-989">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-989">Core</span></span>

* <span data-ttu-id="e5954-990">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="e5954-990">Removed support for Python 3.4</span></span>
* <span data-ttu-id="e5954-991">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-991">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="e5954-992">DLS</span><span class="sxs-lookup"><span data-stu-id="e5954-992">DLS</span></span>

* <span data-ttu-id="e5954-993">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="e5954-993">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="e5954-994">Instalar</span><span class="sxs-lookup"><span data-stu-id="e5954-994">Install</span></span>

* <span data-ttu-id="e5954-995">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="e5954-995">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-996">IOT</span><span class="sxs-lookup"><span data-stu-id="e5954-996">IOT</span></span>

* <span data-ttu-id="e5954-997">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="e5954-997">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="e5954-998">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="e5954-998">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-999">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-999">Key Vault</span></span>

* <span data-ttu-id="e5954-1000">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-1000">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="e5954-1001">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="e5954-1001">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="e5954-1002">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="e5954-1002">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="e5954-1003">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="e5954-1003">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="e5954-1004">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="e5954-1004">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1005">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1005">Network</span></span>

* <span data-ttu-id="e5954-1006">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="e5954-1006">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="e5954-1007">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1007">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="e5954-1008">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-1008">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="e5954-1009">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1009">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="e5954-1010">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="e5954-1010">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-1011">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1011">Packaging</span></span>

* <span data-ttu-id="e5954-1012">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="e5954-1012">Added back edge builds for pip install</span></span>
* <span data-ttu-id="e5954-1013">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-1013">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="e5954-1014">Política</span><span class="sxs-lookup"><span data-stu-id="e5954-1014">Policy</span></span>

* <span data-ttu-id="e5954-1015">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="e5954-1015">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="e5954-1016">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5954-1016">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-1017">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-1017">Redis</span></span>

* <span data-ttu-id="e5954-1018">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1018">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="e5954-1019">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="e5954-1019">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e5954-1020">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e5954-1020">ServiceFabric</span></span>

* <span data-ttu-id="e5954-1021">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-1021">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="e5954-1022">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="e5954-1022">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1023">SQL</span></span>

* <span data-ttu-id="e5954-1024">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="e5954-1024">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1025">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1025">Storage</span></span>

* <span data-ttu-id="e5954-1026">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1026">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="e5954-1027">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="e5954-1027">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="e5954-1028">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-1028">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="e5954-1029">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1029">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="e5954-1030">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="e5954-1030">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="e5954-1031">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1031">November 26, 2019</span></span>

<span data-ttu-id="e5954-1032">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="e5954-1032">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1033">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1033">ACR</span></span>

* <span data-ttu-id="e5954-1034">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1034">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="e5954-1035">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-1035">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="e5954-1036">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1036">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="e5954-1037">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1037">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-1038">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1038">AKS</span></span>

* <span data-ttu-id="e5954-1039">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="e5954-1039">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-1040">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-1040">AppConfig</span></span>

* <span data-ttu-id="e5954-1041">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="e5954-1041">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="e5954-1042">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="e5954-1042">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="e5954-1043">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="e5954-1043">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="e5954-1044">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1044">AppService</span></span>

* <span data-ttu-id="e5954-1045">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1045">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="e5954-1046">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="e5954-1046">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="e5954-1047">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="e5954-1047">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-1048">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-1048">Backup</span></span>

* <span data-ttu-id="e5954-1049">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="e5954-1049">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="e5954-1050">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="e5954-1050">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1051">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1051">Compute</span></span>

* <span data-ttu-id="e5954-1052">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="e5954-1052">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="e5954-1053">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="e5954-1053">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="e5954-1054">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="e5954-1054">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="e5954-1055">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="e5954-1055">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="e5954-1056">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-1056">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="e5954-1057">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="e5954-1057">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="e5954-1058">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-1058">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="e5954-1059">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="e5954-1059">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="e5954-1060">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="e5954-1060">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="e5954-1061">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="e5954-1061">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1062">IOT</span><span class="sxs-lookup"><span data-stu-id="e5954-1062">IOT</span></span>

* <span data-ttu-id="e5954-1063">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="e5954-1063">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="e5954-1064">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-1064">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="e5954-1065">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="e5954-1065">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-1066">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1066">Key Vault</span></span>

* <span data-ttu-id="e5954-1067">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="e5954-1067">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="e5954-1068">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="e5954-1068">NetAppFiles</span></span>

* <span data-ttu-id="e5954-1069">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="e5954-1069">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1070">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1070">Network</span></span>

* <span data-ttu-id="e5954-1071">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-1071">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="e5954-1072">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-1072">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="e5954-1073">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="e5954-1073">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="e5954-1074">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="e5954-1074">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="e5954-1075">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="e5954-1075">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="e5954-1076">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="e5954-1076">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="e5954-1077">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1077">Packaging</span></span>

* <span data-ttu-id="e5954-1078">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="e5954-1078">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="e5954-1079">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="e5954-1079">Added support for Python 3.8</span></span>
* <span data-ttu-id="e5954-1080">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="e5954-1080">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1081">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1081">Profile</span></span>

* <span data-ttu-id="e5954-1082">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="e5954-1082">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="e5954-1083">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="e5954-1083">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="e5954-1084">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="e5954-1084">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="e5954-1085">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="e5954-1085">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="e5954-1086">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="e5954-1086">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1087">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1087">RBAC</span></span>

* <span data-ttu-id="e5954-1088">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-1088">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-1089">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-1089">Redis</span></span>

* <span data-ttu-id="e5954-1090">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="e5954-1090">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="e5954-1091">Reservas</span><span class="sxs-lookup"><span data-stu-id="e5954-1091">Reservations</span></span>

* <span data-ttu-id="e5954-1092">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="e5954-1092">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="e5954-1093">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="e5954-1093">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="e5954-1094">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="e5954-1094">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="e5954-1095">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="e5954-1095">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="e5954-1096">Rest</span><span class="sxs-lookup"><span data-stu-id="e5954-1096">Rest</span></span>
* <span data-ttu-id="e5954-1097">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="e5954-1097">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1098">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1098">SQL</span></span>

* <span data-ttu-id="e5954-1099">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="e5954-1099">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1100">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1100">Storage</span></span>

* <span data-ttu-id="e5954-1101">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="e5954-1101">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="e5954-1102">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="e5954-1102">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="e5954-1103">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="e5954-1103">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="e5954-1104">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="e5954-1104">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="e5954-1105">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1105">November 4, 2019</span></span>

<span data-ttu-id="e5954-1106">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="e5954-1106">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1107">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1107">ACR</span></span>

* <span data-ttu-id="e5954-1108">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1108">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="e5954-1109">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="e5954-1109">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="e5954-1110">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="e5954-1110">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-1111">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1111">AKS</span></span>

* <span data-ttu-id="e5954-1112">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="e5954-1112">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="e5954-1113">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="e5954-1113">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="e5954-1114">AppConfig</span><span class="sxs-lookup"><span data-stu-id="e5954-1114">AppConfig</span></span>

* <span data-ttu-id="e5954-1115">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e5954-1115">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="e5954-1116">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="e5954-1116">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="e5954-1117">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="e5954-1117">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1118">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1118">AppService</span></span>

* <span data-ttu-id="e5954-1119">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="e5954-1119">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="e5954-1120">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1120">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="e5954-1121">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="e5954-1121">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="e5954-1122">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-1122">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="e5954-1123">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1123">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-1124">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-1124">ARM</span></span>

* <span data-ttu-id="e5954-1125">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="e5954-1125">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="e5954-1126">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="e5954-1126">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-1127">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-1127">Backup</span></span>

* <span data-ttu-id="e5954-1128">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-1128">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1129">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1129">Compute</span></span>

* <span data-ttu-id="e5954-1130">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="e5954-1130">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="e5954-1131">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="e5954-1131">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="e5954-1132">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="e5954-1132">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="e5954-1133">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-1133">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="e5954-1134">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="e5954-1134">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="e5954-1135">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1135">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="e5954-1136">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e5954-1136">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="e5954-1137">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="e5954-1137">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-1138">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-1138">CosmosDB</span></span>

* <span data-ttu-id="e5954-1139">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="e5954-1139">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="e5954-1140">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="e5954-1140">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="e5954-1141">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1141">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="e5954-1142">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="e5954-1142">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="e5954-1143">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1143">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="e5954-1144">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="e5954-1144">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="e5954-1145">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-1145">Fixed typo in help message</span></span>
* <span data-ttu-id="e5954-1146">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-1146">database: Added deprecation information</span></span>
* <span data-ttu-id="e5954-1147">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-1147">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1148">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1148">IoT</span></span>

* <span data-ttu-id="e5954-1149">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="e5954-1149">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="e5954-1150">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1150">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-1151">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1151">Key Vault</span></span>

* <span data-ttu-id="e5954-1152">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="e5954-1152">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="e5954-1153">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-1153">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="e5954-1154">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="e5954-1154">NetAppFiles</span></span>

* <span data-ttu-id="e5954-1155">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="e5954-1155">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="e5954-1156">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="e5954-1156">This new API version includes:</span></span>

    - <span data-ttu-id="e5954-1157">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="e5954-1157">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="e5954-1158">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="e5954-1158">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="e5954-1159">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="e5954-1159">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="e5954-1160">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="e5954-1160">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1161">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1161">Network</span></span>

* <span data-ttu-id="e5954-1162">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="e5954-1162">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="e5954-1163">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="e5954-1163">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="e5954-1164">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="e5954-1164">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="e5954-1165">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="e5954-1165">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="e5954-1166">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="e5954-1166">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="e5954-1167">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="e5954-1167">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1168">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1168">Profile</span></span>

* <span data-ttu-id="e5954-1169">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-1169">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="e5954-1170">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="e5954-1170">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1171">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1171">RBAC</span></span>

* <span data-ttu-id="e5954-1172">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-1172">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e5954-1173">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e5954-1173">ServiceFabric</span></span>

* <span data-ttu-id="e5954-1174">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-1174">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1175">SQL</span></span>

* <span data-ttu-id="e5954-1176">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="e5954-1176">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1177">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1177">Storage</span></span>

* <span data-ttu-id="e5954-1178">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-1178">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="e5954-1179">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-1179">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="e5954-1180">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1180">October 15, 2019</span></span>

<span data-ttu-id="e5954-1181">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="e5954-1181">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-1182">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1182">AKS</span></span>

* <span data-ttu-id="e5954-1183">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-1183">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="e5954-1184">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-1184">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1185">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1185">AMS</span></span>

* <span data-ttu-id="e5954-1186">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1186">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="e5954-1187">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="e5954-1187">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1188">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1188">AppService</span></span>

* <span data-ttu-id="e5954-1189">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="e5954-1189">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="e5954-1190">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-1190">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="e5954-1191">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1191">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-1192">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-1192">ARM</span></span>

* <span data-ttu-id="e5954-1193">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="e5954-1193">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1194">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1194">Compute</span></span>

* <span data-ttu-id="e5954-1195">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1195">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="e5954-1196">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="e5954-1196">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="e5954-1197">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-1197">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="e5954-1198">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-1198">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="e5954-1199">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="e5954-1199">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="e5954-1200">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="e5954-1200">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1201">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1201">Core</span></span>

* <span data-ttu-id="e5954-1202">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e5954-1202">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1203">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1203">IoT</span></span>

* <span data-ttu-id="e5954-1204">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="e5954-1204">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1205">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1205">Monitor</span></span>

* <span data-ttu-id="e5954-1206">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="e5954-1206">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1207">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1207">Network</span></span>

* <span data-ttu-id="e5954-1208">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1208">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="e5954-1209">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-1209">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1210">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1210">SQL</span></span>

* <span data-ttu-id="e5954-1211">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="e5954-1211">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1212">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1212">Storage</span></span>

* <span data-ttu-id="e5954-1213">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1213">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="e5954-1214">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1214">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="e5954-1215">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1215">September 24, 2019</span></span>

<span data-ttu-id="e5954-1216">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="e5954-1216">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1217">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1217">ACR</span></span>

* <span data-ttu-id="e5954-1218">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1218">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="e5954-1219">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="e5954-1219">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-1220">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1220">AKS</span></span>

* <span data-ttu-id="e5954-1221">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="e5954-1221">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="e5954-1222">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="e5954-1222">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="e5954-1223">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="e5954-1223">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-1224">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-1224">ARM</span></span>

* <span data-ttu-id="e5954-1225">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="e5954-1225">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1226">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1226">Compute</span></span>

* <span data-ttu-id="e5954-1227">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="e5954-1227">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="e5954-1228">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="e5954-1228">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="e5954-1229">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1229">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="e5954-1230">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="e5954-1230">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="e5954-1231">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1231">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-1232">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-1232">Cosmos DB</span></span>

* <span data-ttu-id="e5954-1233">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="e5954-1233">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="e5954-1234">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="e5954-1234">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="e5954-1235">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-1235">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5954-1236">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e5954-1236">EventGrid</span></span>

* <span data-ttu-id="e5954-1237">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="e5954-1237">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-1238">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1238">Key Vault</span></span>

* <span data-ttu-id="e5954-1239">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1239">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1240">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1240">Monitor</span></span>

* <span data-ttu-id="e5954-1241">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1241">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="e5954-1242">Política</span><span class="sxs-lookup"><span data-stu-id="e5954-1242">Policy</span></span>

* <span data-ttu-id="e5954-1243">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1243">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="e5954-1244">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1244">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1245">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1245">Storage</span></span>

* <span data-ttu-id="e5954-1246">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1246">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="e5954-1247">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1247">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1248">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1248">ACR</span></span>

* <span data-ttu-id="e5954-1249">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="e5954-1249">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-1250">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1250">AKS</span></span>

* <span data-ttu-id="e5954-1251">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e5954-1251">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="e5954-1252">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1252">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="e5954-1253">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1253">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-1254">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-1254">ARM</span></span>

* <span data-ttu-id="e5954-1255">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="e5954-1255">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1256">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1256">Batch</span></span>

* <span data-ttu-id="e5954-1257">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-1257">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="e5954-1258">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="e5954-1258">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="e5954-1259">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="e5954-1259">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="e5954-1260">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="e5954-1260">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="e5954-1261">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="e5954-1261">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="e5954-1262">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="e5954-1262">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="e5954-1263">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="e5954-1263">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1264">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1264">HDInsight</span></span>

* <span data-ttu-id="e5954-1265">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="e5954-1265">GA release</span></span>
* <span data-ttu-id="e5954-1266">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5954-1266">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-1267">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1267">Key Vault</span></span>

* <span data-ttu-id="e5954-1268">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1268">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="e5954-1269">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1269">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1270">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1270">Network</span></span>

* <span data-ttu-id="e5954-1271">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="e5954-1271">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="e5954-1272">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="e5954-1272">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="e5954-1273">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="e5954-1273">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="e5954-1274">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1274">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="e5954-1275">Política</span><span class="sxs-lookup"><span data-stu-id="e5954-1275">Policy</span></span>

* <span data-ttu-id="e5954-1276">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="e5954-1276">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="e5954-1277">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1277">August 27, 2019</span></span>

<span data-ttu-id="e5954-1278">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="e5954-1278">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1279">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1279">ACR</span></span>

* <span data-ttu-id="e5954-1280">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="e5954-1280">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="e5954-1281">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="e5954-1281">API Management</span></span>

* <span data-ttu-id="e5954-1282">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="e5954-1282">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1283">AppService</span></span>

* <span data-ttu-id="e5954-1284">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="e5954-1284">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="e5954-1285">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-1285">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-1286">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-1286">Keyvault</span></span>

* <span data-ttu-id="e5954-1287">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="e5954-1287">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1288">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1288">Network</span></span>

* <span data-ttu-id="e5954-1289">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="e5954-1289">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="e5954-1290">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="e5954-1290">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="e5954-1291">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="e5954-1291">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="e5954-1292">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1292">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1293">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1293">RBAC</span></span>

* <span data-ttu-id="e5954-1294">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="e5954-1294">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e5954-1295">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e5954-1295">ServiceFabric</span></span>

* <span data-ttu-id="e5954-1296">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-1296">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="e5954-1297">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1297">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="e5954-1298">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="e5954-1298">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="e5954-1299">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-1299">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="e5954-1300">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-1300">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="e5954-1301">SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-1301">SignalR</span></span>

* <span data-ttu-id="e5954-1302">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="e5954-1302">Added new commands:</span></span>
  * <span data-ttu-id="e5954-1303">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-1303">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="e5954-1304">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-1304">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="e5954-1305">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-1305">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="e5954-1306">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1306">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1307">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1307">Storage</span></span>

* <span data-ttu-id="e5954-1308">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="e5954-1308">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="e5954-1309">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1309">August 13, 2019</span></span>

<span data-ttu-id="e5954-1310">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="e5954-1310">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1311">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1311">AppService</span></span>

* <span data-ttu-id="e5954-1312">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-1312">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1313">BotService</span><span class="sxs-lookup"><span data-stu-id="e5954-1313">BotService</span></span>

* <span data-ttu-id="e5954-1314">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-1314">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="e5954-1315">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e5954-1315">CognitiveServices</span></span>

* <span data-ttu-id="e5954-1316">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1316">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-1317">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-1317">Cosmos DB</span></span>

* <span data-ttu-id="e5954-1318">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="e5954-1318">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="e5954-1319">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1319">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1320">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1320">HDInsight</span></span>

<span data-ttu-id="e5954-1321">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="e5954-1321">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="e5954-1322">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-1322">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="e5954-1323">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="e5954-1323">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="e5954-1324">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="e5954-1324">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="e5954-1325">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-1325">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="e5954-1326">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="e5954-1326">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="e5954-1327">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-1327">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="e5954-1328">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="e5954-1328">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="e5954-1329">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="e5954-1329">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="e5954-1330">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="e5954-1330">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="e5954-1331">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="e5954-1331">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="e5954-1332">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-1332">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="e5954-1333">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="e5954-1333">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="e5954-1334">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="e5954-1334">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="e5954-1335">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="e5954-1335">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="e5954-1336">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="e5954-1336">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="e5954-1337">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="e5954-1337">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="e5954-1338">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="e5954-1338">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="e5954-1339">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-1339">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="e5954-1340">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="e5954-1340">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="e5954-1341">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="e5954-1341">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="e5954-1342">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-1342">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="e5954-1343">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-1343">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="e5954-1344">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="e5954-1344">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-1345">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1345">Interactive</span></span>

* <span data-ttu-id="e5954-1346">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-1346">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="e5954-1347">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-1347">Kubernetes</span></span>

* <span data-ttu-id="e5954-1348">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="e5954-1348">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1349">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1349">Network</span></span>

* <span data-ttu-id="e5954-1350">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-1350">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1351">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1351">Profile</span></span>

* <span data-ttu-id="e5954-1352">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1352">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="e5954-1353">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e5954-1353">ServiceFabric</span></span>

* <span data-ttu-id="e5954-1354">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="e5954-1354">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="e5954-1355">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="e5954-1355">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1356">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1356">Storage</span></span>

* <span data-ttu-id="e5954-1357">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1357">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="e5954-1358">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1358">July 30, 2019</span></span>

<span data-ttu-id="e5954-1359">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="e5954-1359">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1360">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1360">ACR</span></span>

* <span data-ttu-id="e5954-1361">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="e5954-1361">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="e5954-1362">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="e5954-1362">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1363">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1363">Appservice</span></span>

* <span data-ttu-id="e5954-1364">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="e5954-1364">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="e5954-1365">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="e5954-1365">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="e5954-1366">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="e5954-1366">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1367">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1367">Network</span></span>

* <span data-ttu-id="e5954-1368">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="e5954-1368">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="e5954-1369">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="e5954-1369">Fixes #9604.</span></span> <span data-ttu-id="e5954-1370">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="e5954-1370">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="e5954-1371">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="e5954-1371">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1372">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1372">RBAC</span></span>

* <span data-ttu-id="e5954-1373">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1373">Added `user update` command</span></span>
* <span data-ttu-id="e5954-1374">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-1374">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="e5954-1375">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="e5954-1375">Use replacement argument `--id`</span></span>
* <span data-ttu-id="e5954-1376">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-1376">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1377">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1377">SQL</span></span>

* <span data-ttu-id="e5954-1378">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="e5954-1378">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1379">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1379">Storage</span></span>

* <span data-ttu-id="e5954-1380">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="e5954-1380">Added `storage remove` command</span></span>
* <span data-ttu-id="e5954-1381">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1381">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1382">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1382">VM</span></span>

* <span data-ttu-id="e5954-1383">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="e5954-1383">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="e5954-1384">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1384">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="e5954-1385">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1385">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="e5954-1386">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="e5954-1386">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="e5954-1387">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1387">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="e5954-1388">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1388">July 16, 2019</span></span>

<span data-ttu-id="e5954-1389">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="e5954-1389">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1390">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1390">Appservice</span></span>

* <span data-ttu-id="e5954-1391">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-1391">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="e5954-1392">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-1392">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="e5954-1393">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1393">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1394">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1394">Core</span></span>

* <span data-ttu-id="e5954-1395">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="e5954-1395">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1396">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1396">Batch</span></span>

* <span data-ttu-id="e5954-1397">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="e5954-1397">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="e5954-1398">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="e5954-1398">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="e5954-1399">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1399">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="e5954-1400">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="e5954-1400">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e5954-1401">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-1401">Eventhubs</span></span>

* <span data-ttu-id="e5954-1402">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1402">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-1403">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1403">RDBMS</span></span>

* <span data-ttu-id="e5954-1404">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="e5954-1404">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="e5954-1405">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1405">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="e5954-1406">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="e5954-1406">Relay</span></span>

* <span data-ttu-id="e5954-1407">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="e5954-1407">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="e5954-1408">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1408">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="e5954-1409">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1409">Servicebus</span></span>

* <span data-ttu-id="e5954-1410">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1410">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1411">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1411">Storage</span></span>

* <span data-ttu-id="e5954-1412">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1412">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="e5954-1413">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="e5954-1413">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="e5954-1414">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1414">July 2, 2019</span></span>

<span data-ttu-id="e5954-1415">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="e5954-1415">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1416">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1416">Core</span></span>

* <span data-ttu-id="e5954-1417">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="e5954-1417">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="e5954-1418">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="e5954-1418">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="e5954-1419">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="e5954-1419">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1420">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1420">ACR</span></span>

* <span data-ttu-id="e5954-1421">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="e5954-1421">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1422">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1422">Appservice</span></span>

* <span data-ttu-id="e5954-1423">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-1423">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="e5954-1424">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="e5954-1424">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="e5954-1425">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="e5954-1425">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="e5954-1426">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="e5954-1426">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-1427">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-1427">Cosmos DB</span></span>

* <span data-ttu-id="e5954-1428">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="e5954-1428">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="e5954-1429">DLS</span><span class="sxs-lookup"><span data-stu-id="e5954-1429">DLS</span></span>

* <span data-ttu-id="e5954-1430">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="e5954-1430">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="e5954-1431">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5954-1431">Feedback</span></span>

* <span data-ttu-id="e5954-1432">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="e5954-1432">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1433">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1433">HDInsight</span></span>

* <span data-ttu-id="e5954-1434">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="e5954-1434">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="e5954-1435">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="e5954-1435">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="e5954-1436">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="e5954-1436">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="e5954-1437">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="e5954-1437">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="e5954-1438">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="e5954-1438">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="e5954-1439">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1439">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="e5954-1440">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="e5954-1440">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="e5954-1441">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="e5954-1441">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="e5954-1442">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1442">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="e5954-1443">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-1443">Managed Services</span></span>

* <span data-ttu-id="e5954-1444">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-1444">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1445">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1445">Profile</span></span>
* <span data-ttu-id="e5954-1446">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="e5954-1446">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1447">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1447">RBAC</span></span>

* <span data-ttu-id="e5954-1448">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e5954-1448">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="e5954-1449">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="e5954-1449">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="e5954-1450">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="e5954-1450">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="e5954-1451">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1451">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-1452">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1452">RDBMS</span></span>

* <span data-ttu-id="e5954-1453">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="e5954-1453">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1454">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1454">SQL</span></span>

* <span data-ttu-id="e5954-1455">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-1455">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1456">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1456">Storage</span></span>

* <span data-ttu-id="e5954-1457">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="e5954-1457">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="e5954-1458">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="e5954-1458">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="e5954-1459">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1459">VM</span></span>

* <span data-ttu-id="e5954-1460">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-1460">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="e5954-1461">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1461">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="e5954-1462">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1462">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="e5954-1463">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="e5954-1463">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="e5954-1464">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1464">June 18, 2019</span></span>

<span data-ttu-id="e5954-1465">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="e5954-1465">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1466">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1466">Core</span></span>

<span data-ttu-id="e5954-1467">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="e5954-1467">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="e5954-1468">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="e5954-1468">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="e5954-1469">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="e5954-1469">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="e5954-1470">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="e5954-1470">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="e5954-1471">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="e5954-1471">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="e5954-1472">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="e5954-1472">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="e5954-1473">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="e5954-1473">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1474">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1474">ACR</span></span>
* <span data-ttu-id="e5954-1475">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="e5954-1475">Added 'acr check-health' command</span></span>
* <span data-ttu-id="e5954-1476">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="e5954-1476">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1477">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1477">ACS</span></span>
* <span data-ttu-id="e5954-1478">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-1478">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1479">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1479">AMS</span></span>
* <span data-ttu-id="e5954-1480">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="e5954-1480">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1481">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1481">AppService</span></span>
* <span data-ttu-id="e5954-1482">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="e5954-1482">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="e5954-1483">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5954-1483">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="e5954-1484">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="e5954-1484">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="e5954-1485">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1485">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="e5954-1486">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="e5954-1486">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="e5954-1487">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="e5954-1487">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1488">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1488">Batch</span></span>
* <span data-ttu-id="e5954-1489">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="e5954-1489">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-1490">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e5954-1490">BatchAI</span></span>
* <span data-ttu-id="e5954-1491">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="e5954-1491">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1492">BotService</span><span class="sxs-lookup"><span data-stu-id="e5954-1492">BotService</span></span>
* <span data-ttu-id="e5954-1493">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="e5954-1493">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-1494">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-1494">CosmosDB</span></span>
* <span data-ttu-id="e5954-1495">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="e5954-1495">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="e5954-1496">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="e5954-1496">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="e5954-1497">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="e5954-1497">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="e5954-1498">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-1498">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5954-1499">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e5954-1499">EventGrid</span></span>
* <span data-ttu-id="e5954-1500">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="e5954-1500">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="e5954-1501">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="e5954-1501">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="e5954-1502">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="e5954-1502">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="e5954-1503">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="e5954-1503">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="e5954-1504">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1504">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1505">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1505">HDInsight</span></span>
* <span data-ttu-id="e5954-1506">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1506">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1507">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1507">IoT</span></span>
* <span data-ttu-id="e5954-1508">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="e5954-1508">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="e5954-1509">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="e5954-1509">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1510">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1510">Network</span></span>
* <span data-ttu-id="e5954-1511">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="e5954-1511">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="e5954-1512">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="e5954-1512">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="e5954-1513">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="e5954-1513">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="e5954-1514">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="e5954-1514">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1515">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1515">Resource</span></span>
* <span data-ttu-id="e5954-1516">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="e5954-1516">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="e5954-1517">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="e5954-1517">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="e5954-1518">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e5954-1518">ServiceBus</span></span>
* <span data-ttu-id="e5954-1519">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="e5954-1519">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1520">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1520">SQL</span></span>
* <span data-ttu-id="e5954-1521">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-1521">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="e5954-1522">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="e5954-1522">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="e5954-1523">SQLVm</span><span class="sxs-lookup"><span data-stu-id="e5954-1523">SQLVm</span></span>
* <span data-ttu-id="e5954-1524">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="e5954-1524">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="e5954-1525">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1525">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1526">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1526">Storage</span></span>
* <span data-ttu-id="e5954-1527">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="e5954-1527">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="e5954-1528">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-1528">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1529">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1529">VM</span></span>
* <span data-ttu-id="e5954-1530">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1530">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="e5954-1531">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1531">June 4, 2019</span></span>

<span data-ttu-id="e5954-1532">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="e5954-1532">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1533">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1533">Core</span></span>
* <span data-ttu-id="e5954-1534">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="e5954-1534">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1535">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1535">ACR</span></span>
* <span data-ttu-id="e5954-1536">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="e5954-1536">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1537">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1537">ACS</span></span>
* <span data-ttu-id="e5954-1538">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-1538">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="e5954-1539">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-1539">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1540">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1540">Batch</span></span>
* <span data-ttu-id="e5954-1541">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="e5954-1541">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1542">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1542">IoT</span></span>
* <span data-ttu-id="e5954-1543">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="e5954-1543">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1544">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1544">Network</span></span>
* <span data-ttu-id="e5954-1545">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="e5954-1545">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="e5954-1546">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1546">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="e5954-1547">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1547">Resource</span></span>
* <span data-ttu-id="e5954-1548">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="e5954-1548">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1549">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1549">Role</span></span>
* <span data-ttu-id="e5954-1550">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="e5954-1550">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1551">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1551">Compute</span></span>
* <span data-ttu-id="e5954-1552">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="e5954-1552">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="e5954-1553">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1553">May 21, 2019</span></span>

<span data-ttu-id="e5954-1554">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="e5954-1554">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1555">Core</span></span>
* <span data-ttu-id="e5954-1556">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="e5954-1556">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="e5954-1557">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1557">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="e5954-1558">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="e5954-1558">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1559">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1559">ACR</span></span>
* <span data-ttu-id="e5954-1560">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="e5954-1560">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1561">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1561">ACS</span></span>
* <span data-ttu-id="e5954-1562">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="e5954-1562">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1563">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1563">AppService</span></span>
* <span data-ttu-id="e5954-1564">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="e5954-1564">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="e5954-1565">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="e5954-1565">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="e5954-1566">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="e5954-1566">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="e5954-1567">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="e5954-1567">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="e5954-1568">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-1568">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="e5954-1569">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="e5954-1569">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="e5954-1570">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-1570">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1571">BotService</span><span class="sxs-lookup"><span data-stu-id="e5954-1571">BotService</span></span>
* <span data-ttu-id="e5954-1572">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-1572">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="e5954-1573">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="e5954-1573">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-1574">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-1574">Consumption</span></span>
* <span data-ttu-id="e5954-1575">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-1575">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1576">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1576">IoT</span></span>
* <span data-ttu-id="e5954-1577">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="e5954-1577">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1578">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1578">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="e5954-1580">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="e5954-1580">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="e5954-1581">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="e5954-1581">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-1582">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1582">RDBMS</span></span>
* <span data-ttu-id="e5954-1583">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="e5954-1583">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-1584">RBAC</span><span class="sxs-lookup"><span data-stu-id="e5954-1584">RBAC</span></span>
* <span data-ttu-id="e5954-1585">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="e5954-1585">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1586">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1586">Storage</span></span>
* <span data-ttu-id="e5954-1587">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="e5954-1587">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="e5954-1588">Computação</span><span class="sxs-lookup"><span data-stu-id="e5954-1588">Compute</span></span>
* <span data-ttu-id="e5954-1589">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1589">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="e5954-1590">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="e5954-1590">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="e5954-1591">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="e5954-1591">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="e5954-1592">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="e5954-1592">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="e5954-1593">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1593">May 6, 2019</span></span>

<span data-ttu-id="e5954-1594">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="e5954-1594">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1595">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1595">ACS</span></span>
* <span data-ttu-id="e5954-1596">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="e5954-1596">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="e5954-1597">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="e5954-1597">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="e5954-1598">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1598">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="e5954-1599">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1599">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1600">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1600">Appservice</span></span>
* <span data-ttu-id="e5954-1601">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-1601">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="e5954-1602">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="e5954-1602">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="e5954-1603">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-1603">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="e5954-1604">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="e5954-1604">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="e5954-1605">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-1605">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="e5954-1606">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="e5954-1606">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="e5954-1607">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-1607">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="e5954-1608">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="e5954-1608">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="e5954-1609">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-1609">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="e5954-1610">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="e5954-1610">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1611">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1611">Batch</span></span>
* <span data-ttu-id="e5954-1612">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="e5954-1612">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1613">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="e5954-1613">Botservice</span></span>
* <span data-ttu-id="e5954-1614">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="e5954-1614">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="e5954-1615">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="e5954-1615">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="e5954-1616">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="e5954-1616">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="e5954-1617">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="e5954-1617">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="e5954-1618">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="e5954-1618">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="e5954-1619">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="e5954-1619">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="e5954-1620">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1620">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="e5954-1621">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="e5954-1621">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="e5954-1622">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="e5954-1622">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="e5954-1623">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="e5954-1623">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="e5954-1624">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="e5954-1624">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="e5954-1625">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="e5954-1625">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="e5954-1626">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="e5954-1626">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="e5954-1627">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="e5954-1627">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="e5954-1628">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-1628">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="e5954-1629">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="e5954-1629">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="e5954-1630">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1630">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="e5954-1631">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="e5954-1631">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="e5954-1632">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="e5954-1632">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="e5954-1633">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="e5954-1633">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="e5954-1634">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="e5954-1634">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="e5954-1635">Configurar</span><span class="sxs-lookup"><span data-stu-id="e5954-1635">Configure</span></span>
* <span data-ttu-id="e5954-1636">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="e5954-1636">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e5954-1637">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-1637">Eventhubs</span></span>
* <span data-ttu-id="e5954-1638">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1638">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="e5954-1639">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1639">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1640">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1640">Network</span></span>
* <span data-ttu-id="e5954-1641">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1641">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="e5954-1642">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="e5954-1642">Policy Insights</span></span>
* <span data-ttu-id="e5954-1643">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1643">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1644">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1644">Role</span></span>
* <span data-ttu-id="e5954-1645">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1645">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5954-1646">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1646">Service Bus</span></span>
* <span data-ttu-id="e5954-1647">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1647">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="e5954-1648">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1648">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="e5954-1649">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="e5954-1649">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1650">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1650">SQL</span></span>
* <span data-ttu-id="e5954-1651">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1651">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1652">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1652">VM</span></span>
* <span data-ttu-id="e5954-1653">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-1653">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="e5954-1654">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-1654">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="e5954-1655">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-1655">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="e5954-1656">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="e5954-1656">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="e5954-1657">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="e5954-1657">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="e5954-1658">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1658">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="e5954-1659">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1659">April 23, 2019</span></span>

<span data-ttu-id="e5954-1660">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="e5954-1660">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1661">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1661">ACS</span></span>
* <span data-ttu-id="e5954-1662">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="e5954-1662">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="e5954-1663">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="e5954-1663">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1664">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1664">AMS</span></span>
* <span data-ttu-id="e5954-1665">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1665">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1666">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1666">AppService</span></span>
* <span data-ttu-id="e5954-1667">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="e5954-1667">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="e5954-1668">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e5954-1668">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="e5954-1669">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="e5954-1669">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="e5954-1670">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="e5954-1670">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="e5954-1671">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="e5954-1671">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="e5954-1672">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-1672">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="e5954-1673">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="e5954-1673">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="e5954-1674">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="e5954-1674">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="e5954-1675">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="e5954-1675">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="e5954-1676">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-1676">Deployment Manager</span></span>
* <span data-ttu-id="e5954-1677">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="e5954-1677">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-1678">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-1678">Lab</span></span>
* <span data-ttu-id="e5954-1679">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-1679">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1680">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1680">Network</span></span>
* <span data-ttu-id="e5954-1681">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="e5954-1681">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1682">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1682">Resource</span></span>
* <span data-ttu-id="e5954-1683">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="e5954-1683">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="e5954-1684">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="e5954-1684">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="e5954-1685">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="e5954-1685">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="e5954-1686">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="e5954-1686">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1687">SQL</span></span>
* <span data-ttu-id="e5954-1688">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="e5954-1688">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="e5954-1689">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1689">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="e5954-1690">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1690">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="e5954-1691">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-1691">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1692">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1692">Storage</span></span>
* <span data-ttu-id="e5954-1693">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="e5954-1693">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1694">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1694">VM</span></span>
* <span data-ttu-id="e5954-1695">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1695">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="e5954-1696">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="e5954-1696">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="e5954-1697">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="e5954-1697">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="e5954-1698">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1698">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1699">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1699">Core</span></span>
* <span data-ttu-id="e5954-1700">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="e5954-1700">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1701">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1701">ACR</span></span>
* <span data-ttu-id="e5954-1702">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="e5954-1702">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1703">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1703">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="e5954-1706">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1706">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="e5954-1707">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1707">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1708">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1708">AppService</span></span>
* <span data-ttu-id="e5954-1709">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-1709">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="e5954-1710">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="e5954-1710">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="e5954-1711">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1711">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="e5954-1712">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="e5954-1712">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="e5954-1713">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-1713">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="e5954-1714">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="e5954-1714">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="e5954-1715">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="e5954-1715">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-1716">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-1716">CDN</span></span>
* <span data-ttu-id="e5954-1717">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="e5954-1717">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="e5954-1718">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5954-1718">Feedback</span></span>
* <span data-ttu-id="e5954-1719">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="e5954-1719">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="e5954-1720">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="e5954-1720">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="e5954-1721">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="e5954-1721">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1722">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1722">Monitor</span></span>
* <span data-ttu-id="e5954-1723">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1723">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="e5954-1724">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1724">Network</span></span>
* <span data-ttu-id="e5954-1725">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="e5954-1725">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="e5954-1726">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-1726">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="e5954-1727">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="e5954-1727">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="e5954-1728">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1728">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="e5954-1729">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="e5954-1729">PrivateDNS</span></span>
* <span data-ttu-id="e5954-1730">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="e5954-1730">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1731">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1731">Resource</span></span>
* <span data-ttu-id="e5954-1732">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="e5954-1732">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1733">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1733">Role</span></span>
* <span data-ttu-id="e5954-1734">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="e5954-1734">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="e5954-1735">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="e5954-1735">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-1736">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1736">SQL</span></span>
* <span data-ttu-id="e5954-1737">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="e5954-1737">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1738">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1738">Storage</span></span>
* <span data-ttu-id="e5954-1739">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-1739">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="e5954-1740">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="e5954-1740">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="e5954-1741">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="e5954-1741">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="e5954-1742">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="e5954-1742">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="e5954-1743">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1743">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="e5954-1744">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1744">Core</span></span>
* <span data-ttu-id="e5954-1745">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="e5954-1745">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="e5954-1746">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="e5954-1746">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="e5954-1747">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-1747">Cloud</span></span>
* <span data-ttu-id="e5954-1748">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="e5954-1748">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1749">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1749">ACR</span></span>
* <span data-ttu-id="e5954-1750">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="e5954-1750">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="e5954-1751">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1751">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="e5954-1752">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="e5954-1752">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="e5954-1753">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="e5954-1753">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1754">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1754">AppService</span></span>
* <span data-ttu-id="e5954-1755">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="e5954-1755">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="e5954-1756">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="e5954-1756">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="e5954-1757">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="e5954-1757">BOT Service</span></span>
* <span data-ttu-id="e5954-1758">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="e5954-1758">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="e5954-1759">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="e5954-1759">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="e5954-1760">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="e5954-1760">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="e5954-1761">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="e5954-1761">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-1762">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-1762">CDN</span></span>
* <span data-ttu-id="e5954-1763">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1763">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="e5954-1765">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="e5954-1765">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e5954-1766">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-1766">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-1767">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="e5954-1767">Cosmosdb</span></span>
* <span data-ttu-id="e5954-1768">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="e5954-1768">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="e5954-1769">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-1769">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-1770">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1770">Interactive</span></span>
* <span data-ttu-id="e5954-1771">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="e5954-1771">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1772">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1772">Monitor</span></span>
* <span data-ttu-id="e5954-1773">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1773">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1774">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1774">Network</span></span>
* <span data-ttu-id="e5954-1775">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="e5954-1775">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1776">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1776">Profile</span></span>
* <span data-ttu-id="e5954-1777">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="e5954-1777">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="e5954-1778">Postgres</span><span class="sxs-lookup"><span data-stu-id="e5954-1778">Postgres</span></span> 
* <span data-ttu-id="e5954-1779">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="e5954-1779">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="e5954-1780">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="e5954-1780">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1781">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1781">Resource</span></span>
* <span data-ttu-id="e5954-1782">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1782">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="e5954-1783">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="e5954-1783">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="e5954-1784">Grafo</span><span class="sxs-lookup"><span data-stu-id="e5954-1784">Graph</span></span>
* <span data-ttu-id="e5954-1785">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="e5954-1785">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="e5954-1786">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="e5954-1786">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="e5954-1787">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="e5954-1787">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="e5954-1788">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-1788">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="e5954-1789">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-1789">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1790">armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1790">storage</span></span>
* <span data-ttu-id="e5954-1791">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1791">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="e5954-1792">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="e5954-1792">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="e5954-1793">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="e5954-1793">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="e5954-1794">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="e5954-1794">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1795">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1795">VM</span></span>
* <span data-ttu-id="e5954-1796">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1796">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="e5954-1797">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1797">March 12, 2019</span></span>

<span data-ttu-id="e5954-1798">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="e5954-1798">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1799">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1799">Core</span></span>

* <span data-ttu-id="e5954-1800">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="e5954-1800">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1801">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1801">ACR</span></span>

* <span data-ttu-id="e5954-1802">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="e5954-1802">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1803">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1803">ACS</span></span>

* <span data-ttu-id="e5954-1804">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="e5954-1804">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="e5954-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1805">AppService</span></span>

* <span data-ttu-id="e5954-1806">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="e5954-1806">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="e5954-1807">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1807">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="e5954-1808">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="e5954-1808">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="e5954-1809">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="e5954-1809">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1810">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="e5954-1810">Botservice</span></span>

* <span data-ttu-id="e5954-1811">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="e5954-1811">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e5954-1812">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="e5954-1812">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e5954-1813">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="e5954-1813">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="e5954-1814">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="e5954-1814">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="e5954-1815">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-1815">Container</span></span>

* <span data-ttu-id="e5954-1816">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1816">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5954-1817">EventHub</span><span class="sxs-lookup"><span data-stu-id="e5954-1817">EventHub</span></span>

* <span data-ttu-id="e5954-1818">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="e5954-1818">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="e5954-1819">Localizar</span><span class="sxs-lookup"><span data-stu-id="e5954-1819">Find</span></span>

* <span data-ttu-id="e5954-1820">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="e5954-1820">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1821">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1821">HDInsight</span></span>

* <span data-ttu-id="e5954-1822">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="e5954-1822">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1823">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1823">Network</span></span>

* <span data-ttu-id="e5954-1824">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="e5954-1824">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-1825">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e5954-1825">Rdbms</span></span>

* <span data-ttu-id="e5954-1826">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="e5954-1826">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1827">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1827">Role</span></span>

* <span data-ttu-id="e5954-1828">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="e5954-1828">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="e5954-1829">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="e5954-1829">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5954-1830">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-1830">Service Fabric</span></span>

* <span data-ttu-id="e5954-1831">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="e5954-1831">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="e5954-1832">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1832">February 26, 2019</span></span>

<span data-ttu-id="e5954-1833">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="e5954-1833">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1834">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1834">Core</span></span>

* <span data-ttu-id="e5954-1835">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="e5954-1835">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1836">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1836">ACR</span></span>

* <span data-ttu-id="e5954-1837">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1837">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="e5954-1838">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-1838">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1839">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1839">ACS</span></span>

* <span data-ttu-id="e5954-1840">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="e5954-1840">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1841">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1841">AppService</span></span>

* <span data-ttu-id="e5954-1842">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="e5954-1842">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-1843">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-1843">Batch</span></span>
* <span data-ttu-id="e5954-1844">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="e5954-1844">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="e5954-1845">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="e5954-1845">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="e5954-1846">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1846">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="e5954-1847">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="e5954-1847">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="e5954-1848">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="e5954-1848">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="e5954-1849">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-1849">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-1850">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-1850">CosmosDB</span></span>

* <span data-ttu-id="e5954-1851">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-1851">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="e5954-1852">Kusto</span><span class="sxs-lookup"><span data-stu-id="e5954-1852">Kusto</span></span>

* <span data-ttu-id="e5954-1853">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="e5954-1853">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1854">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1854">Network</span></span>

* <span data-ttu-id="e5954-1855">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1855">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="e5954-1856">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="e5954-1856">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="e5954-1857">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-1857">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="e5954-1858">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1858">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="e5954-1859">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1859">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="e5954-1860">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1860">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="e5954-1861">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="e5954-1861">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1862">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1862">Resource</span></span>

* <span data-ttu-id="e5954-1863">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-1863">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="e5954-1864">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1864">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="e5954-1865">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1865">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="e5954-1866">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1866">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="e5954-1867">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-1867">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1868">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1868">Role</span></span>

* <span data-ttu-id="e5954-1869">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1869">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1870">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1870">VM</span></span>

* <span data-ttu-id="e5954-1871">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="e5954-1871">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="e5954-1872">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1872">February 12, 2019</span></span>

<span data-ttu-id="e5954-1873">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="e5954-1873">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1874">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1874">Core</span></span>

* <span data-ttu-id="e5954-1875">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="e5954-1875">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="e5954-1876">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="e5954-1876">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1877">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1877">ACR</span></span>
* <span data-ttu-id="e5954-1878">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-1878">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="e5954-1879">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="e5954-1879">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1880">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1880">ACS</span></span>
* <span data-ttu-id="e5954-1881">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-1881">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="e5954-1882">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="e5954-1882">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="e5954-1883">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-1883">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1884">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1884">AMS</span></span>
* <span data-ttu-id="e5954-1885">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-1885">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="e5954-1886">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-1886">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1887">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1887">Appservice</span></span>
* <span data-ttu-id="e5954-1888">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1888">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="e5954-1889">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="e5954-1889">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="e5954-1890">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1890">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="e5954-1891">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e5954-1891">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="e5954-1892">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="e5954-1892">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-1893">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="e5954-1893">Botservice</span></span>
* <span data-ttu-id="e5954-1894">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="e5954-1894">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="e5954-1895">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="e5954-1895">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="e5954-1896">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-1896">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="e5954-1897">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="e5954-1897">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="e5954-1898">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="e5954-1898">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="e5954-1899">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="e5954-1899">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="e5954-1900">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1900">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="e5954-1901">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="e5954-1901">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="e5954-1902">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="e5954-1902">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="e5954-1903">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="e5954-1903">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-1904">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-1904">Key Vault</span></span>
* <span data-ttu-id="e5954-1905">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="e5954-1905">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1906">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1906">Monitor</span></span>
* <span data-ttu-id="e5954-1907">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="e5954-1907">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1908">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1908">Network</span></span>
* <span data-ttu-id="e5954-1909">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="e5954-1909">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="e5954-1910">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-1910">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="e5954-1911">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-1911">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="e5954-1912">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1912">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e5954-1913">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="e5954-1913">Policy Insights</span></span>
* <span data-ttu-id="e5954-1914">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-1914">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-1915">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1915">RDBMS</span></span>
* <span data-ttu-id="e5954-1916">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="e5954-1916">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-1917">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-1917">Redis</span></span>
* <span data-ttu-id="e5954-1918">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="e5954-1918">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="e5954-1919">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="e5954-1919">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="e5954-1920">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="e5954-1920">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="e5954-1921">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-1921">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="e5954-1922">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="e5954-1922">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="e5954-1923">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="e5954-1923">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="e5954-1924">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="e5954-1924">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="e5954-1925">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-1925">Role</span></span>
* <span data-ttu-id="e5954-1926">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="e5954-1926">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="e5954-1927">SQL VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1927">SQL VM</span></span>
* <span data-ttu-id="e5954-1928">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="e5954-1928">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1929">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1929">VM</span></span>
* <span data-ttu-id="e5954-1930">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="e5954-1930">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="e5954-1931">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1931">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="e5954-1932">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="e5954-1932">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="e5954-1933">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="e5954-1933">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="e5954-1934">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1934">January 31, 2019</span></span>

<span data-ttu-id="e5954-1935">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="e5954-1935">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="e5954-1936">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-1936">Core</span></span>

* <span data-ttu-id="e5954-1937">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="e5954-1937">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="e5954-1938">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1938">January 28, 2019</span></span>

<span data-ttu-id="e5954-1939">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="e5954-1939">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1940">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1940">ACR</span></span>
* <span data-ttu-id="e5954-1941">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="e5954-1941">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-1942">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1942">ACS</span></span>
* <span data-ttu-id="e5954-1943">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="e5954-1943">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e5954-1944">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-1944">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="e5954-1945">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="e5954-1945">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-1946">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-1946">AMS</span></span>
* <span data-ttu-id="e5954-1947">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="e5954-1947">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="e5954-1948">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="e5954-1948">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1949">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1949">Appservice</span></span>
* <span data-ttu-id="e5954-1950">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1950">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="e5954-1951">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e5954-1951">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="e5954-1952">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="e5954-1952">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="e5954-1953">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-1953">Container</span></span>
* <span data-ttu-id="e5954-1954">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="e5954-1954">Added `container start` command</span></span>
* <span data-ttu-id="e5954-1955">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-1955">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5954-1956">EventGrid</span><span class="sxs-lookup"><span data-stu-id="e5954-1956">EventGrid</span></span>
* <span data-ttu-id="e5954-1957">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1957">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="e5954-1958">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="e5954-1958">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="e5954-1959">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-1959">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="e5954-1960">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="e5954-1960">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="e5954-1961">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-1961">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-1962">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-1962">HDInsight</span></span>
* <span data-ttu-id="e5954-1963">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="e5954-1963">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="e5954-1964">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="e5954-1964">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="e5954-1965">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1965">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="e5954-1966">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1966">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="e5954-1967">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="e5954-1967">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="e5954-1968">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="e5954-1968">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-1969">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-1969">IoT</span></span>
* <span data-ttu-id="e5954-1970">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="e5954-1970">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="e5954-1971">Kusto</span><span class="sxs-lookup"><span data-stu-id="e5954-1971">Kusto</span></span>
* <span data-ttu-id="e5954-1972">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-1972">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-1973">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-1973">Monitor</span></span>
* <span data-ttu-id="e5954-1974">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-1974">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-1975">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-1975">Profile</span></span>
* <span data-ttu-id="e5954-1976">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="e5954-1976">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-1977">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-1977">Network</span></span>
* <span data-ttu-id="e5954-1978">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="e5954-1978">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="e5954-1979">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="e5954-1979">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-1980">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-1980">Resource</span></span>
* <span data-ttu-id="e5954-1981">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e5954-1981">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="e5954-1982">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-1982">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="e5954-1983">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-1983">SQL Virtual Machine</span></span>
* <span data-ttu-id="e5954-1984">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-1984">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-1985">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-1985">Storage</span></span>
* <span data-ttu-id="e5954-1986">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="e5954-1986">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="e5954-1987">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="e5954-1987">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-1988">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-1988">VM</span></span>
* <span data-ttu-id="e5954-1989">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="e5954-1989">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="e5954-1990">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e5954-1990">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="e5954-1991">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="e5954-1991">January 15, 2019</span></span>

<span data-ttu-id="e5954-1992">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="e5954-1992">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-1993">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-1993">ACR</span></span>
* <span data-ttu-id="e5954-1994">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="e5954-1994">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="e5954-1995">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-1995">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="e5954-1996">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="e5954-1996">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="e5954-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-1997">ACS</span></span>
* <span data-ttu-id="e5954-1998">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="e5954-1998">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-1999">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-1999">Appservice</span></span>
* <span data-ttu-id="e5954-2000">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="e5954-2000">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="e5954-2001">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-2001">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="e5954-2002">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="e5954-2002">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="e5954-2003">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="e5954-2003">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-2004">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="e5954-2004">Botservice</span></span>
* <span data-ttu-id="e5954-2005">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2005">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="e5954-2006">Configurar</span><span class="sxs-lookup"><span data-stu-id="e5954-2006">Configure</span></span>
* <span data-ttu-id="e5954-2007">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="e5954-2007">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-2008">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-2008">CosmosDB</span></span>
* <span data-ttu-id="e5954-2009">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="e5954-2009">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-2010">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-2010">HDInsight</span></span>
* <span data-ttu-id="e5954-2011">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="e5954-2011">Added commands for managing applications</span></span>
* <span data-ttu-id="e5954-2012">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="e5954-2012">Added commands for managing script actions</span></span>
* <span data-ttu-id="e5954-2013">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="e5954-2013">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="e5954-2014">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="e5954-2014">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="e5954-2015">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="e5954-2015">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2016">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2016">Network</span></span>
* <span data-ttu-id="e5954-2017">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2017">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="e5954-2018">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="e5954-2018">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="e5954-2019">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2019">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="e5954-2020">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="e5954-2020">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2021">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2021">Role</span></span>
* <span data-ttu-id="e5954-2022">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2022">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="e5954-2023">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-2023">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="e5954-2024">Segurança</span><span class="sxs-lookup"><span data-stu-id="e5954-2024">Security</span></span>
* <span data-ttu-id="e5954-2025">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2025">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2026">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2026">Storage</span></span>
* <span data-ttu-id="e5954-2027">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="e5954-2027">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="e5954-2028">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="e5954-2028">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="e5954-2029">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2029">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="e5954-2030">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2030">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="e5954-2031">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="e5954-2031">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2032">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2032">VM</span></span>
* <span data-ttu-id="e5954-2033">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="e5954-2033">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="e5954-2034">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2034">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5954-2035">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="e5954-2035">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="e5954-2036">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="e5954-2036">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="e5954-2037">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2037">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="e5954-2038">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="e5954-2038">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="e5954-2039">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2039">December 20, 2018</span></span>

<span data-ttu-id="e5954-2040">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="e5954-2040">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="e5954-2041">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2041">Appservice</span></span>
* <span data-ttu-id="e5954-2042">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="e5954-2042">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="e5954-2043">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="e5954-2043">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="e5954-2044">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-2044">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e5954-2045">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-2045">IoTCentral</span></span>
* <span data-ttu-id="e5954-2046">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="e5954-2046">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2047">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2047">Role</span></span>
* <span data-ttu-id="e5954-2048">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2048">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2049">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2049">SQL</span></span>
* <span data-ttu-id="e5954-2050">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2050">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2051">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2051">VM</span></span>
* <span data-ttu-id="e5954-2052">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2052">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="e5954-2053">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2053">December 18, 2018</span></span>

<span data-ttu-id="e5954-2054">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="e5954-2054">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="e5954-2055">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2055">ACR</span></span>
* <span data-ttu-id="e5954-2056">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="e5954-2056">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="e5954-2057">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="e5954-2057">Condensed the table layout for task list</span></span>
* <span data-ttu-id="e5954-2058">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="e5954-2058">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2059">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2059">ACS</span></span>
* <span data-ttu-id="e5954-2060">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="e5954-2060">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e5954-2061">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2061">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="e5954-2062">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="e5954-2062">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="e5954-2063">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-2063">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="e5954-2064">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-2064">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="e5954-2065">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="e5954-2065">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2066">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2066">Appservice</span></span>
* <span data-ttu-id="e5954-2067">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="e5954-2067">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="e5954-2068">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="e5954-2068">Botservice</span></span>
* <span data-ttu-id="e5954-2069">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2069">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="e5954-2070">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="e5954-2070">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="e5954-2071">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="e5954-2071">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="e5954-2072">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="e5954-2072">Reduced Kudu network calls</span></span>
* <span data-ttu-id="e5954-2073">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="e5954-2073">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-2074">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-2074">Consumption</span></span>
* <span data-ttu-id="e5954-2075">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="e5954-2075">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-2076">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-2076">CosmosDB</span></span>
* <span data-ttu-id="e5954-2077">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="e5954-2077">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="e5954-2078">Mapas</span><span class="sxs-lookup"><span data-stu-id="e5954-2078">Maps</span></span>
* <span data-ttu-id="e5954-2079">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2079">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2080">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2080">Network</span></span>
* <span data-ttu-id="e5954-2081">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="e5954-2081">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="e5954-2082">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-2082">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2083">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2083">Resource</span></span>
* <span data-ttu-id="e5954-2084">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2084">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="e5954-2085">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-2085">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2086">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2086">Storage</span></span>
*  <span data-ttu-id="e5954-2087">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2087">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2088">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2088">VM</span></span>
* <span data-ttu-id="e5954-2089">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="e5954-2089">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="e5954-2090">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2090">December 4, 2018</span></span>

<span data-ttu-id="e5954-2091">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="e5954-2091">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="e5954-2092">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2092">Core</span></span>
* <span data-ttu-id="e5954-2093">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="e5954-2093">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="e5954-2094">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2094">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2095">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2095">Appservice</span></span>
* <span data-ttu-id="e5954-2096">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2096">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="e5954-2097">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="e5954-2097">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2098">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2098">Network</span></span>
* <span data-ttu-id="e5954-2099">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="e5954-2099">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2100">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2100">Role</span></span>
* <span data-ttu-id="e5954-2101">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="e5954-2101">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="e5954-2102">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2102">VM</span></span>
* <span data-ttu-id="e5954-2103">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-2103">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="e5954-2104">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="e5954-2104">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="e5954-2105">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="e5954-2105">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="e5954-2106">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-2106">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="e5954-2107">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2107">November 20, 2018</span></span>

<span data-ttu-id="e5954-2108">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="e5954-2108">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="e5954-2109">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2109">Core</span></span>
* <span data-ttu-id="e5954-2110">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="e5954-2110">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2111">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2111">ACR</span></span>
* <span data-ttu-id="e5954-2112">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="e5954-2112">Added context token to task step</span></span>
* <span data-ttu-id="e5954-2113">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="e5954-2113">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="e5954-2114">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e5954-2114">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2115">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2115">Appservice</span></span>
* <span data-ttu-id="e5954-2116">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="e5954-2116">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="e5954-2117">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="e5954-2117">Updated the default `node_version`.</span></span> <span data-ttu-id="e5954-2118">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="e5954-2118">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="e5954-2119">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2119">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="e5954-2120">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="e5954-2120">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e5954-2121">Iot Central</span><span class="sxs-lookup"><span data-stu-id="e5954-2121">IotCentral</span></span>
* <span data-ttu-id="e5954-2122">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-2122">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-2123">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-2123">KeyVault</span></span>
* <span data-ttu-id="e5954-2124">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="e5954-2124">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2125">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2125">Network</span></span>
* <span data-ttu-id="e5954-2126">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="e5954-2126">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="e5954-2127">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="e5954-2127">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="e5954-2128">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2128">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="e5954-2129">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-2129">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2130">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e5954-2130">Rdbms</span></span>
* <span data-ttu-id="e5954-2131">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-2131">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="e5954-2132">Rbac</span><span class="sxs-lookup"><span data-stu-id="e5954-2132">Rbac</span></span>
* <span data-ttu-id="e5954-2133">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2133">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="e5954-2134">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2134">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="e5954-2135">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2135">Storage</span></span>
* <span data-ttu-id="e5954-2136">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2136">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="e5954-2137">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="e5954-2137">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="e5954-2138">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="e5954-2138">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="e5954-2139">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2139">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2140">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2140">VM</span></span>
* <span data-ttu-id="e5954-2141">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2141">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="e5954-2142">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="e5954-2142">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="e5954-2143">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="e5954-2143">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="e5954-2144">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="e5954-2144">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="e5954-2145">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2145">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="e5954-2146">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-2146">Added `snapshot wait` command</span></span>
* <span data-ttu-id="e5954-2147">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-2147">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="e5954-2148">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2148">November 6, 2018</span></span>

<span data-ttu-id="e5954-2149">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="e5954-2149">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2150">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2150">Core</span></span>
* <span data-ttu-id="e5954-2151">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="e5954-2151">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2152">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2152">ACR</span></span>
* <span data-ttu-id="e5954-2153">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="e5954-2153">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="e5954-2154">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="e5954-2154">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2155">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2155">ACS</span></span>
* <span data-ttu-id="e5954-2156">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2156">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="e5954-2157">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e5954-2157">Advisor</span></span>
* <span data-ttu-id="e5954-2158">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="e5954-2158">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-2159">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2159">AMS</span></span>
* <span data-ttu-id="e5954-2160">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="e5954-2160">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="e5954-2161">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="e5954-2161">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="e5954-2162">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2162">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="e5954-2163">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="e5954-2163">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="e5954-2164">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="e5954-2164">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="e5954-2165">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="e5954-2165">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="e5954-2166">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="e5954-2166">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="e5954-2167">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="e5954-2167">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="e5954-2168">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="e5954-2168">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="e5954-2169">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="e5954-2169">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="e5954-2170">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-2170">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="e5954-2171">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2171">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="e5954-2172">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="e5954-2172">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="e5954-2173">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="e5954-2173">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="e5954-2174">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2174">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="e5954-2175">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="e5954-2175">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="e5954-2176">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="e5954-2176">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2177">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2177">AppService</span></span>
* <span data-ttu-id="e5954-2178">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="e5954-2178">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="e5954-2179">Configurar</span><span class="sxs-lookup"><span data-stu-id="e5954-2179">Configure</span></span>
* <span data-ttu-id="e5954-2180">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="e5954-2180">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2181">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2181">Container</span></span>
* <span data-ttu-id="e5954-2182">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="e5954-2182">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="e5954-2183">EventHub</span><span class="sxs-lookup"><span data-stu-id="e5954-2183">EventHub</span></span>
* <span data-ttu-id="e5954-2184">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2184">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2185">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2185">Interactive</span></span>
* <span data-ttu-id="e5954-2186">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="e5954-2186">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-2187">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-2187">Monitor</span></span>
* <span data-ttu-id="e5954-2188">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2188">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2189">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2189">Network</span></span>
* <span data-ttu-id="e5954-2190">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="e5954-2190">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="e5954-2191">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="e5954-2191">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="e5954-2192">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2192">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="e5954-2193">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-2193">Profile</span></span>
* <span data-ttu-id="e5954-2194">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="e5954-2194">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2195">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2195">RDBMS</span></span>
* <span data-ttu-id="e5954-2196">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="e5954-2196">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2197">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2197">Resource</span></span>
* <span data-ttu-id="e5954-2198">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="e5954-2198">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2199">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2199">Role</span></span>
* <span data-ttu-id="e5954-2200">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="e5954-2200">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="e5954-2201">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2201">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="e5954-2202">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="e5954-2202">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2203">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2203">Storage</span></span>
* <span data-ttu-id="e5954-2204">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="e5954-2204">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2205">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2205">VM</span></span>
* <span data-ttu-id="e5954-2206">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-2206">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="e5954-2207">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-2207">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="e5954-2208">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="e5954-2208">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="e5954-2209">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="e5954-2209">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="e5954-2210">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="e5954-2210">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="e5954-2211">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="e5954-2211">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="e5954-2212">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2212">October 23, 2018</span></span>

<span data-ttu-id="e5954-2213">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="e5954-2213">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2214">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2214">Core</span></span>
* <span data-ttu-id="e5954-2215">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5954-2215">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="e5954-2216">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5954-2216">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2217">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2217">ACR</span></span>
* <span data-ttu-id="e5954-2218">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="e5954-2218">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-2219">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-2219">CDN</span></span>
* <span data-ttu-id="e5954-2220">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="e5954-2220">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e5954-2221">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2221">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2222">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2222">Container</span></span>
* <span data-ttu-id="e5954-2223">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="e5954-2223">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="e5954-2224">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-2224">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="e5954-2225">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-2225">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="e5954-2226">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-2226">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="e5954-2227">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="e5954-2227">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="e5954-2228">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="e5954-2228">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="e5954-2229">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2229">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-2230">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-2230">CosmosDB</span></span>
* <span data-ttu-id="e5954-2231">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2231">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2232">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2232">Interactive</span></span>
* <span data-ttu-id="e5954-2233">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="e5954-2233">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5954-2234">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2234">IoT Central</span></span>
* <span data-ttu-id="e5954-2235">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-2235">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="e5954-2236">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="e5954-2236">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-2237">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-2237">Monitor</span></span>
* <span data-ttu-id="e5954-2238">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="e5954-2238">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="e5954-2239">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2239">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="e5954-2240">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="e5954-2240">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e5954-2241">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-2241">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="e5954-2242">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="e5954-2242">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="e5954-2243">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2243">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="e5954-2244">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="e5954-2244">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="e5954-2245">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="e5954-2245">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e5954-2246">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-2246">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="e5954-2247">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2247">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2248">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2248">Network</span></span>
* <span data-ttu-id="e5954-2249">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="e5954-2249">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="e5954-2250">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="e5954-2250">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="e5954-2251">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e5954-2251">ServiceBus</span></span>
* <span data-ttu-id="e5954-2252">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2252">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2253">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2253">SQL</span></span>
* <span data-ttu-id="e5954-2254">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="e5954-2254">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2255">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2255">Storage</span></span>
* <span data-ttu-id="e5954-2256">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="e5954-2256">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="e5954-2257">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="e5954-2257">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2258">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2258">VM</span></span>
* <span data-ttu-id="e5954-2259">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2259">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5954-2260">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2260">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="e5954-2261">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2261">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="e5954-2262">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2262">October 16, 2018</span></span>

<span data-ttu-id="e5954-2263">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="e5954-2263">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2264">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2264">VM</span></span>
* <span data-ttu-id="e5954-2265">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="e5954-2265">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="e5954-2266">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2266">October 9, 2018</span></span>

<span data-ttu-id="e5954-2267">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="e5954-2267">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2268">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2268">Core</span></span>
* <span data-ttu-id="e5954-2269">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="e5954-2269">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2270">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2270">ACR</span></span>
* <span data-ttu-id="e5954-2271">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="e5954-2271">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2272">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2272">ACS</span></span>
* <span data-ttu-id="e5954-2273">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="e5954-2273">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="e5954-2274">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="e5954-2274">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="e5954-2275">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="e5954-2275">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="e5954-2276">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2276">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2277">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2277">Container</span></span>
* <span data-ttu-id="e5954-2278">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="e5954-2278">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="e5954-2279">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-2279">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="e5954-2280">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="e5954-2280">Event Hub</span></span>
* <span data-ttu-id="e5954-2281">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2281">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="e5954-2282">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="e5954-2282">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="e5954-2283">Extensões</span><span class="sxs-lookup"><span data-stu-id="e5954-2283">Extensions</span></span>
* <span data-ttu-id="e5954-2284">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="e5954-2284">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e5954-2285">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e5954-2285">HDInsight</span></span>
* <span data-ttu-id="e5954-2286">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2286">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-2287">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2287">IoT</span></span>
* <span data-ttu-id="e5954-2288">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2288">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-2289">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-2289">KeyVault</span></span>
* <span data-ttu-id="e5954-2290">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="e5954-2290">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2291">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2291">Network</span></span>
* <span data-ttu-id="e5954-2292">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="e5954-2292">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="e5954-2293">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="e5954-2293">See #6052</span></span>
* <span data-ttu-id="e5954-2294">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2294">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="e5954-2295">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="e5954-2295">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="e5954-2296">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5954-2296">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="e5954-2297">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5954-2297">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="e5954-2298">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="e5954-2298">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="e5954-2299">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2299">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2300">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2300">Role</span></span>
* <span data-ttu-id="e5954-2301">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="e5954-2301">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="e5954-2302">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="e5954-2302">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="e5954-2303">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="e5954-2303">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="e5954-2304">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="e5954-2304">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5954-2305">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2305">Service Bus</span></span>
* <span data-ttu-id="e5954-2306">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="e5954-2306">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2307">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2307">VM</span></span>
* <span data-ttu-id="e5954-2308">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="e5954-2308">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="e5954-2309">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2309">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="e5954-2310">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="e5954-2310">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="e5954-2311">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="e5954-2311">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="e5954-2312">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="e5954-2312">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="e5954-2313">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="e5954-2313">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="e5954-2314">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2314">September 21, 2018</span></span>

<span data-ttu-id="e5954-2315">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="e5954-2315">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2316">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2316">ACR</span></span>
* <span data-ttu-id="e5954-2317">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2317">Added ACR Task commands</span></span>
* <span data-ttu-id="e5954-2318">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="e5954-2318">Added quick run command</span></span>
* <span data-ttu-id="e5954-2319">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-2319">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="e5954-2320">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2320">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="e5954-2321">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="e5954-2321">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="e5954-2322">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="e5954-2322">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2323">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2323">ACS</span></span>
* <span data-ttu-id="e5954-2324">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-2324">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="e5954-2325">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="e5954-2325">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2326">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2326">AppService</span></span>

* <span data-ttu-id="e5954-2327">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="e5954-2327">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="e5954-2328">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="e5954-2328">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="e5954-2329">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="e5954-2329">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="e5954-2330">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="e5954-2330">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-2331">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2331">Batch</span></span>
* <span data-ttu-id="e5954-2332">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="e5954-2332">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="e5954-2333">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="e5954-2333">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="e5954-2334">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2334">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="e5954-2335">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="e5954-2335">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5954-2336">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e5954-2336">Batch AI</span></span> 
* <span data-ttu-id="e5954-2337">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2337">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5954-2338">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-2338">Cognitive Services</span></span>
* <span data-ttu-id="e5954-2339">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="e5954-2339">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="e5954-2340">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="e5954-2340">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="e5954-2341">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="e5954-2341">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="e5954-2342">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2342">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="e5954-2343">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2343">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="e5954-2344">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="e5954-2344">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2345">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2345">Container</span></span>
* <span data-ttu-id="e5954-2346">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="e5954-2346">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="e5954-2347">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2347">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="e5954-2348">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="e5954-2348">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="e5954-2349">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-2349">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="e5954-2350">DataLake</span><span class="sxs-lookup"><span data-stu-id="e5954-2350">Datalake</span></span>
* <span data-ttu-id="e5954-2351">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="e5954-2351">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="e5954-2352">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2352">Interactive Shell</span></span>
* <span data-ttu-id="e5954-2353">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2353">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="e5954-2354">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-2354">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-2355">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2355">IoT</span></span>
* <span data-ttu-id="e5954-2356">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2356">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-2357">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e5954-2357">Key Vault</span></span>
* <span data-ttu-id="e5954-2358">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="e5954-2358">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2359">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2359">Network</span></span>
* <span data-ttu-id="e5954-2360">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="e5954-2360">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="e5954-2361">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2361">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="e5954-2362">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="e5954-2362">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="e5954-2363">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="e5954-2363">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="e5954-2364">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2364">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="e5954-2365">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2365">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="e5954-2366">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="e5954-2366">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="e5954-2367">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="e5954-2367">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="e5954-2368">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="e5954-2368">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="e5954-2369">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="e5954-2369">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="e5954-2370">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="e5954-2370">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="e5954-2371">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="e5954-2371">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="e5954-2372">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="e5954-2372">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="e5954-2373">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e5954-2373">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="e5954-2374">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="e5954-2374">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="e5954-2375">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="e5954-2375">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="e5954-2376">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2376">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="e5954-2377">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="e5954-2377">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2378">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2378">RDBMS</span></span>
* <span data-ttu-id="e5954-2379">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="e5954-2379">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="e5954-2380">Reserva</span><span class="sxs-lookup"><span data-stu-id="e5954-2380">Reservation</span></span>
* <span data-ttu-id="e5954-2381">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="e5954-2381">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="e5954-2382">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="e5954-2382">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="e5954-2383">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2383">Manage App</span></span>
* <span data-ttu-id="e5954-2384">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="e5954-2384">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="e5954-2385">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="e5954-2385">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2386">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2386">Role</span></span>
* <span data-ttu-id="e5954-2387">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="e5954-2387">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="e5954-2388">SignalR</span><span class="sxs-lookup"><span data-stu-id="e5954-2388">SignalR</span></span>
* <span data-ttu-id="e5954-2389">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="e5954-2389">First release</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2390">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2390">Storage</span></span>
* <span data-ttu-id="e5954-2391">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="e5954-2391">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="e5954-2392">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="e5954-2392">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2393">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2393">VM</span></span>
* <span data-ttu-id="e5954-2394">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="e5954-2394">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="e5954-2395">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="e5954-2395">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="e5954-2396">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2396">August 28, 2018</span></span>

<span data-ttu-id="e5954-2397">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="e5954-2397">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2398">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2398">Core</span></span>

* <span data-ttu-id="e5954-2399">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="e5954-2399">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="e5954-2400">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5954-2400">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2401">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2401">ACR</span></span>

* <span data-ttu-id="e5954-2402">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-2402">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="e5954-2403">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="e5954-2403">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2404">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2404">ACS</span></span>

* <span data-ttu-id="e5954-2405">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="e5954-2405">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="e5954-2406">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-2406">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2407">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2407">AppService</span></span>

* <span data-ttu-id="e5954-2408">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="e5954-2408">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="e5954-2409">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2409">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="e5954-2410">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2410">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-2411">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-2411">Backup</span></span>

* <span data-ttu-id="e5954-2412">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2412">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="e5954-2413">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="e5954-2413">Bot Service</span></span>

* <span data-ttu-id="e5954-2414">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2414">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5954-2415">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-2415">Cognitive Services</span></span>

* <span data-ttu-id="e5954-2416">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="e5954-2416">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-2417">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2417">IoT</span></span>

* <span data-ttu-id="e5954-2418">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="e5954-2418">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-2419">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-2419">Monitor</span></span>

* <span data-ttu-id="e5954-2420">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="e5954-2420">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="e5954-2421">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-2421">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2422">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2422">Network</span></span>

* <span data-ttu-id="e5954-2423">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2423">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2424">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2424">Resource</span></span>

* <span data-ttu-id="e5954-2425">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2425">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2426">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2426">Storage</span></span>

* <span data-ttu-id="e5954-2427">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2427">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2428">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2428">VM</span></span>

* <span data-ttu-id="e5954-2429">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2429">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="e5954-2430">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2430">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="e5954-2431">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2431">Auguest 14, 2018</span></span>

<span data-ttu-id="e5954-2432">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="e5954-2432">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2433">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2433">Core</span></span>

* <span data-ttu-id="e5954-2434">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="e5954-2434">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="e5954-2435">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="e5954-2435">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="e5954-2436">Telemetria</span><span class="sxs-lookup"><span data-stu-id="e5954-2436">Telemetry</span></span>

* <span data-ttu-id="e5954-2437">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="e5954-2437">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2438">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2438">ACR</span></span>

* <span data-ttu-id="e5954-2439">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-2439">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="e5954-2440">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2440">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2441">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2441">ACS</span></span>

* <span data-ttu-id="e5954-2442">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-2442">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="e5954-2443">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2443">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="e5954-2444">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="e5954-2444">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="e5954-2445">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="e5954-2445">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="e5954-2446">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="e5954-2446">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="e5954-2447">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2447">AppService</span></span>

* <span data-ttu-id="e5954-2448">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="e5954-2448">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="e5954-2449">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="e5954-2449">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-2450">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e5954-2450">BatchAI</span></span>

* <span data-ttu-id="e5954-2451">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="e5954-2451">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="e5954-2452">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2452">Container</span></span>

* <span data-ttu-id="e5954-2453">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2453">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="e5954-2454">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2454">IoT</span></span>

* <span data-ttu-id="e5954-2455">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="e5954-2455">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="e5954-2456">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="e5954-2456">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="e5954-2457">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-2457">Iot Central</span></span>

* <span data-ttu-id="e5954-2458">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="e5954-2458">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-2459">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-2459">KeyVault</span></span>


* <span data-ttu-id="e5954-2460">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="e5954-2460">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="e5954-2461">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2461">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="e5954-2462">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="e5954-2462">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="e5954-2463">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="e5954-2463">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="e5954-2464">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="e5954-2464">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="e5954-2465">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="e5954-2465">Relay</span></span>

* <span data-ttu-id="e5954-2466">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2466">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2467">Sql</span><span class="sxs-lookup"><span data-stu-id="e5954-2467">Sql</span></span>

* <span data-ttu-id="e5954-2468">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="e5954-2468">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2469">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2469">Storage</span></span>

* <span data-ttu-id="e5954-2470">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="e5954-2470">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="e5954-2471">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="e5954-2471">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="e5954-2472">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="e5954-2472">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="e5954-2473">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="e5954-2473">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="e5954-2474">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2474">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2475">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2475">VM</span></span>

* <span data-ttu-id="e5954-2476">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="e5954-2476">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e5954-2477">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2477">July 31, 2018</span></span>

<span data-ttu-id="e5954-2478">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e5954-2478">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2479">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2479">ACR</span></span>

* <span data-ttu-id="e5954-2480">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2480">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e5954-2481">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="e5954-2481">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2482">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2482">ACS</span></span>

* <span data-ttu-id="e5954-2483">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="e5954-2483">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-2484">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2484">Batch</span></span>

* <span data-ttu-id="e5954-2485">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="e5954-2485">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2486">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2486">Container</span></span>

* <span data-ttu-id="e5954-2487">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2487">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2488">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2488">Network</span></span>

* <span data-ttu-id="e5954-2489">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5954-2489">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e5954-2490">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2490">Resource</span></span>

* <span data-ttu-id="e5954-2491">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="e5954-2491">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e5954-2492">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="e5954-2492">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2493">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2493">Role</span></span>

* <span data-ttu-id="e5954-2494">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e5954-2494">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e5954-2495">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-2495">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e5954-2496">Search</span><span class="sxs-lookup"><span data-stu-id="e5954-2496">Search</span></span>

* <span data-ttu-id="e5954-2497">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="e5954-2497">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5954-2498">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-2498">Service Bus</span></span>

* <span data-ttu-id="e5954-2499">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="e5954-2499">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e5954-2500">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2500">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="e5954-2501">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="e5954-2501">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="e5954-2502">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="e5954-2502">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2503">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2503">Storage</span></span>

* <span data-ttu-id="e5954-2504">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="e5954-2504">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e5954-2505">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2505">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2506">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2506">VM</span></span>

* <span data-ttu-id="e5954-2507">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2507">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e5954-2508">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="e5954-2508">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="e5954-2509">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2509">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e5954-2510">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="e5954-2510">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e5954-2511">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2511">July 18, 2018</span></span>

<span data-ttu-id="e5954-2512">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e5954-2512">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2513">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2513">Core</span></span>

* <span data-ttu-id="e5954-2514">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="e5954-2514">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e5954-2515">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e5954-2515">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e5954-2516">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="e5954-2516">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2517">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2517">ACR</span></span>

* <span data-ttu-id="e5954-2518">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="e5954-2518">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e5954-2519">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="e5954-2519">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e5954-2520">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2520">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e5954-2521">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-2521">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2522">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2522">ACS</span></span>

* <span data-ttu-id="e5954-2523">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="e5954-2523">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2524">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2524">AppService</span></span>

* <span data-ttu-id="e5954-2525">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="e5954-2525">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-2526">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2526">Batch</span></span>

* <span data-ttu-id="e5954-2527">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5954-2527">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e5954-2528">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-2528">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5954-2529">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e5954-2529">Batch AI</span></span>

* <span data-ttu-id="e5954-2530">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="e5954-2530">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2531">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2531">Container</span></span>

* <span data-ttu-id="e5954-2532">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="e5954-2532">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e5954-2533">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="e5954-2533">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2534">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2534">Network</span></span>

* <span data-ttu-id="e5954-2535">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2535">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="e5954-2536">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-2536">Added `network nic wait`</span></span>
* <span data-ttu-id="e5954-2537">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2537">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="e5954-2538">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2538">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="e5954-2539">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2539">Resource</span></span>

* <span data-ttu-id="e5954-2540">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-2540">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="e5954-2541">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-2541">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="e5954-2542">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-2542">Added `deployment wait` command</span></span>
* <span data-ttu-id="e5954-2543">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="e5954-2543">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2544">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2544">SQL</span></span>

* <span data-ttu-id="e5954-2545">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2545">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e5954-2546">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="e5954-2546">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="e5954-2547">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="e5954-2547">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2548">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2548">Storage</span></span>

* <span data-ttu-id="e5954-2549">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="e5954-2549">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2550">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2550">VM</span></span>

* <span data-ttu-id="e5954-2551">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2551">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e5954-2552">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2552">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="e5954-2553">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="e5954-2553">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e5954-2554">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2554">July 3, 2018</span></span>

<span data-ttu-id="e5954-2555">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e5954-2555">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-2556">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-2556">AKS</span></span>

* <span data-ttu-id="e5954-2557">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2557">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e5954-2558">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2558">July 3, 2018</span></span>

<span data-ttu-id="e5954-2559">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e5954-2559">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2560">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2560">Core</span></span>

* <span data-ttu-id="e5954-2561">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2561">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2562">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2562">ACR</span></span>

* <span data-ttu-id="e5954-2563">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-2563">Added polling build status</span></span>
* <span data-ttu-id="e5954-2564">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-2564">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e5954-2565">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="e5954-2565">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2566">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2566">ACS</span></span>

* <span data-ttu-id="e5954-2567">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2567">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e5954-2568">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="e5954-2568">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e5954-2569">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2569">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e5954-2570">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-2570">Added `--listen-port` support</span></span>
* <span data-ttu-id="e5954-2571">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2571">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e5954-2572">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="e5954-2572">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e5954-2573">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="e5954-2573">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2574">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2574">AppService</span></span>

* <span data-ttu-id="e5954-2575">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="e5954-2575">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="e5954-2576">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="e5954-2576">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-2577">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-2577">Backup</span></span>

* <span data-ttu-id="e5954-2578">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="e5954-2578">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-2579">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e5954-2579">BatchAI</span></span>

* <span data-ttu-id="e5954-2580">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2580">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e5954-2581">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-2581">Cloud</span></span>

* <span data-ttu-id="e5954-2582">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-2582">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2583">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2583">Container</span></span>

* <span data-ttu-id="e5954-2584">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="e5954-2584">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e5954-2585">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-2585">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="e5954-2586">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="e5954-2586">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-2587">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2587">Extension</span></span>

* <span data-ttu-id="e5954-2588">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-2588">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2589">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2589">Network</span></span>

* <span data-ttu-id="e5954-2590">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="e5954-2590">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2591">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e5954-2591">Rdbms</span></span>

* <span data-ttu-id="e5954-2592">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-2592">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2593">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2593">Resource</span></span>

* <span data-ttu-id="e5954-2594">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-2594">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2595">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2595">VM</span></span>

* <span data-ttu-id="e5954-2596">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e5954-2596">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e5954-2597">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2597">June 25, 2018</span></span>

<span data-ttu-id="e5954-2598">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e5954-2598">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e5954-2599">CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-2599">CLI</span></span>

* <span data-ttu-id="e5954-2600">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2600">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e5954-2601">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2601">June 19, 2018</span></span>

<span data-ttu-id="e5954-2602">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e5954-2602">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2603">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2603">Core</span></span>

* <span data-ttu-id="e5954-2604">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2604">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2605">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2605">ACR</span></span>

* <span data-ttu-id="e5954-2606">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="e5954-2606">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e5954-2607">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="e5954-2607">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2608">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2608">ACS</span></span>

* <span data-ttu-id="e5954-2609">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="e5954-2609">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e5954-2610">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="e5954-2610">Added `--update` support</span></span>
* <span data-ttu-id="e5954-2611">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="e5954-2611">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="e5954-2612">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-2612">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e5954-2613">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-2613">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e5954-2614">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="e5954-2614">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="e5954-2615">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5954-2615">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="e5954-2616">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5954-2616">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2617">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2617">AppService</span></span>

* <span data-ttu-id="e5954-2618">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="e5954-2618">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e5954-2619">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="e5954-2619">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-2620">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2620">Batch</span></span>

* <span data-ttu-id="e5954-2621">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="e5954-2621">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5954-2622">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e5954-2622">Batch AI</span></span>

* <span data-ttu-id="e5954-2623">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="e5954-2623">Added support for workspaces.</span></span> <span data-ttu-id="e5954-2624">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="e5954-2624">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e5954-2625">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="e5954-2625">Added support for experiments.</span></span> <span data-ttu-id="e5954-2626">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="e5954-2626">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e5954-2627">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="e5954-2627">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e5954-2628">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2628">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e5954-2629">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="e5954-2629">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e5954-2630">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="e5954-2630">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e5954-2631">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="e5954-2631">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e5954-2632">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="e5954-2632">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e5954-2633">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2633">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e5954-2634">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="e5954-2634">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e5954-2635">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2635">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e5954-2636">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="e5954-2636">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e5954-2637">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="e5954-2637">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e5954-2638">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="e5954-2638">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e5954-2639">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2639">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e5954-2640">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="e5954-2640">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="e5954-2641">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="e5954-2641">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="e5954-2642">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e5954-2642">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e5954-2643">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="e5954-2643">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e5954-2644">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="e5954-2644">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e5954-2645">Mapas</span><span class="sxs-lookup"><span data-stu-id="e5954-2645">Maps</span></span>

* <span data-ttu-id="e5954-2646">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="e5954-2646">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2647">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2647">Network</span></span>

* <span data-ttu-id="e5954-2648">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="e5954-2648">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e5954-2649">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e5954-2649">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e5954-2650">#6502</span><span class="sxs-lookup"><span data-stu-id="e5954-2650">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e5954-2651">Reservas</span><span class="sxs-lookup"><span data-stu-id="e5954-2651">Reservations</span></span>

* <span data-ttu-id="e5954-2652">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2652">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="e5954-2653">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2653">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="e5954-2654">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="e5954-2654">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="e5954-2655">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e5954-2655">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="e5954-2656">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="e5954-2656">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="e5954-2657">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2657">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2658">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2658">Role</span></span>

* <span data-ttu-id="e5954-2659">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="e5954-2659">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2660">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2660">SQL</span></span>

* <span data-ttu-id="e5954-2661">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2661">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2662">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2662">Storage</span></span>

* <span data-ttu-id="e5954-2663">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="e5954-2663">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2664">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2664">VM</span></span>

* <span data-ttu-id="e5954-2665">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2665">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="e5954-2666">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="e5954-2666">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="e5954-2667">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="e5954-2667">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e5954-2668">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2668">June 13, 2018</span></span>

<span data-ttu-id="e5954-2669">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e5954-2669">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2670">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2670">Core</span></span>

* <span data-ttu-id="e5954-2671">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="e5954-2671">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e5954-2672">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2672">June 13, 2018</span></span>

<span data-ttu-id="e5954-2673">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e5954-2673">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-2674">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-2674">AKS</span></span>

* <span data-ttu-id="e5954-2675">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2675">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="e5954-2676">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="e5954-2676">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e5954-2677">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2677">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="e5954-2678">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2678">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="e5954-2679">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2679">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2680">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2680">AppService</span></span>

* <span data-ttu-id="e5954-2681">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="e5954-2681">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e5954-2682">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2682">June 5, 2018</span></span>

<span data-ttu-id="e5954-2683">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e5954-2683">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2684">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2684">Interactive</span></span>

* <span data-ttu-id="e5954-2685">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2685">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e5954-2686">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2686">June 5, 2018</span></span>

<span data-ttu-id="e5954-2687">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e5954-2687">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2688">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2688">Core</span></span>

* <span data-ttu-id="e5954-2689">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="e5954-2689">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e5954-2690">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="e5954-2690">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2691">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2691">ACR</span></span>

* <span data-ttu-id="e5954-2692">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="e5954-2692">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e5954-2693">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="e5954-2693">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e5954-2694">AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-2694">AKS</span></span>

* <span data-ttu-id="e5954-2695">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="e5954-2695">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-2696">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2696">Batch</span></span>

* <span data-ttu-id="e5954-2697">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e5954-2697">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-2698">IOT</span><span class="sxs-lookup"><span data-stu-id="e5954-2698">IOT</span></span>

* <span data-ttu-id="e5954-2699">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="e5954-2699">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2700">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2700">Network</span></span>

* <span data-ttu-id="e5954-2701">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="e5954-2701">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="e5954-2702">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="e5954-2702">Policy Insights</span></span>

* <span data-ttu-id="e5954-2703">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-2703">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e5954-2704">ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-2704">ARM</span></span>

* <span data-ttu-id="e5954-2705">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="e5954-2705">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2706">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2706">SQL</span></span>

* <span data-ttu-id="e5954-2707">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="e5954-2707">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e5954-2708">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="e5954-2708">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e5954-2709">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2709">Storage</span></span>

* <span data-ttu-id="e5954-2710">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="e5954-2710">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2711">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2711">VM</span></span>

* <span data-ttu-id="e5954-2712">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="e5954-2712">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e5954-2713">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2713">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="e5954-2714">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2714">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="e5954-2715">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2715">May 22, 2018</span></span>

<span data-ttu-id="e5954-2716">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e5954-2716">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2717">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2717">Core</span></span>

* <span data-ttu-id="e5954-2718">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="e5954-2718">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2719">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2719">ACS</span></span>

* <span data-ttu-id="e5954-2720">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-2720">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="e5954-2721">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-2721">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2722">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2722">AppService</span></span>

* <span data-ttu-id="e5954-2723">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="e5954-2723">Improved generic update commands</span></span>
* <span data-ttu-id="e5954-2724">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="e5954-2724">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2725">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2725">Container</span></span>

* <span data-ttu-id="e5954-2726">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="e5954-2726">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e5954-2727">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2727">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-2728">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2728">Extension</span></span>

* <span data-ttu-id="e5954-2729">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="e5954-2729">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2730">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2730">Interactive</span></span>

* <span data-ttu-id="e5954-2731">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="e5954-2731">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e5954-2732">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="e5954-2732">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-2733">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-2733">KeyVault</span></span>

* <span data-ttu-id="e5954-2734">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="e5954-2734">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2735">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2735">Network</span></span>

* <span data-ttu-id="e5954-2736">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e5954-2736">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e5954-2737">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e5954-2737">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2738">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2738">SQL</span></span>

* <span data-ttu-id="e5954-2739">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="e5954-2739">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e5954-2740">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="e5954-2740">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="e5954-2741">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="e5954-2741">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e5954-2742">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5954-2742">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e5954-2743">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e5954-2743">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="e5954-2744">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2744">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="e5954-2745">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="e5954-2745">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="e5954-2746">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2746">`edition`.</span></span> <span data-ttu-id="e5954-2747">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="e5954-2747">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="e5954-2748">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2748">`elasticPoolName`.</span></span> <span data-ttu-id="e5954-2749">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="e5954-2749">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e5954-2750">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="e5954-2750">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="e5954-2751">`edition`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2751">`edition`.</span></span> <span data-ttu-id="e5954-2752">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="e5954-2752">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="e5954-2753">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2753">`dtu`.</span></span> <span data-ttu-id="e5954-2754">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="e5954-2754">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="e5954-2755">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2755">`databaseDtuMin`.</span></span> <span data-ttu-id="e5954-2756">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="e5954-2756">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="e5954-2757">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2757">`databaseDtuMax`.</span></span> <span data-ttu-id="e5954-2758">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="e5954-2758">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e5954-2759">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2759">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e5954-2760">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2760">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2761">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2761">Storage</span></span>

* <span data-ttu-id="e5954-2762">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-2762">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e5954-2763">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-2763">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2764">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2764">VM</span></span>

* <span data-ttu-id="e5954-2765">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2765">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e5954-2766">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="e5954-2766">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="e5954-2767">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="e5954-2767">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="e5954-2768">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="e5954-2768">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e5954-2769">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2769">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="e5954-2770">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2770">May 7, 2018</span></span>

<span data-ttu-id="e5954-2771">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e5954-2771">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2772">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2772">Core</span></span>

* <span data-ttu-id="e5954-2773">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="e5954-2773">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e5954-2774">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e5954-2774">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e5954-2775">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2775">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e5954-2776">#5591</span><span class="sxs-lookup"><span data-stu-id="e5954-2776">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e5954-2777">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2777">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e5954-2778">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="e5954-2778">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e5954-2779">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2779">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e5954-2780">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="e5954-2780">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="e5954-2781">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="e5954-2781">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2782">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2782">ACR</span></span>

* <span data-ttu-id="e5954-2783">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2783">Added ACR Build commands</span></span>
* <span data-ttu-id="e5954-2784">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="e5954-2784">Improved resource not found error messages</span></span>
* <span data-ttu-id="e5954-2785">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="e5954-2785">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e5954-2786">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="e5954-2786">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e5954-2787">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="e5954-2787">Improved repository commands error messages</span></span>
* <span data-ttu-id="e5954-2788">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2788">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2789">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2789">ACS</span></span>

* <span data-ttu-id="e5954-2790">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-2790">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e5954-2791">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-2791">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e5954-2792">AMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2792">AMS</span></span>

* <span data-ttu-id="e5954-2793">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-2793">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2794">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2794">Appservice</span></span>

* <span data-ttu-id="e5954-2795">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-2795">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e5954-2796">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2796">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="e5954-2797">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="e5954-2797">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e5954-2798">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="e5954-2798">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e5954-2799">Lote AI</span><span class="sxs-lookup"><span data-stu-id="e5954-2799">Batch AI</span></span>

* <span data-ttu-id="e5954-2800">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-2800">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5954-2801">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-2801">Cognitive Services</span></span>

* <span data-ttu-id="e5954-2802">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="e5954-2802">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-2803">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-2803">Consumption</span></span>

* <span data-ttu-id="e5954-2804">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2804">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2805">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2805">Container</span></span>

* <span data-ttu-id="e5954-2806">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-2806">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e5954-2807">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-2807">Cosmos DB</span></span>

* <span data-ttu-id="e5954-2808">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e5954-2808">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e5954-2809">DMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2809">DMS</span></span>

* <span data-ttu-id="e5954-2810">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-2810">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-2811">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2811">Extension</span></span>

* <span data-ttu-id="e5954-2812">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="e5954-2812">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2813">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2813">Interactive</span></span>

* <span data-ttu-id="e5954-2814">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="e5954-2814">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e5954-2815">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="e5954-2815">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e5954-2816">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-2816">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e5954-2817">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="e5954-2817">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-2818">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-2818">Lab</span></span>

* <span data-ttu-id="e5954-2819">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="e5954-2819">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2820">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2820">Network</span></span>

* <span data-ttu-id="e5954-2821">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="e5954-2821">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e5954-2822">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-2822">Profile</span></span>

* <span data-ttu-id="e5954-2823">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="e5954-2823">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e5954-2824">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="e5954-2824">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e5954-2825">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="e5954-2825">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-2826">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-2826">Redis</span></span>

* <span data-ttu-id="e5954-2827">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2827">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="e5954-2828">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="e5954-2828">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e5954-2829">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2829">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="e5954-2830">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="e5954-2830">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="e5954-2831">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2831">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e5954-2832">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2832">Role</span></span>

* <span data-ttu-id="e5954-2833">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="e5954-2833">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2834">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2834">Storage</span></span>

* <span data-ttu-id="e5954-2835">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2835">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e5954-2836">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="e5954-2836">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e5954-2837">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="e5954-2837">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e5954-2838">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="e5954-2838">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e5954-2839">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="e5954-2839">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2840">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2840">VM</span></span>

* <span data-ttu-id="e5954-2841">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="e5954-2841">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e5954-2842">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-2842">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e5954-2843">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="e5954-2843">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e5954-2844">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="e5954-2844">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="e5954-2845">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="e5954-2845">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e5954-2846">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="e5954-2846">Added write accelerator support</span></span>
* <span data-ttu-id="e5954-2847">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e5954-2847">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="e5954-2848">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="e5954-2848">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e5954-2849">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="e5954-2849">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e5954-2850">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2850">April 10, 2018</span></span>

<span data-ttu-id="e5954-2851">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e5954-2851">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2852">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2852">ACR</span></span>

* <span data-ttu-id="e5954-2853">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="e5954-2853">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2854">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2854">ACS</span></span>

* <span data-ttu-id="e5954-2855">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="e5954-2855">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2856">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2856">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="e5954-2858">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="e5954-2858">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-2859">BatchAI</span><span class="sxs-lookup"><span data-stu-id="e5954-2859">BatchAI</span></span>

* <span data-ttu-id="e5954-2860">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="e5954-2860">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="e5954-2861">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-2861">Job level mounting</span></span>
  - <span data-ttu-id="e5954-2862">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="e5954-2862">Environment variables with secret values</span></span>
  - <span data-ttu-id="e5954-2863">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="e5954-2863">Performance counters settings</span></span>
  - <span data-ttu-id="e5954-2864">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-2864">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="e5954-2865">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="e5954-2865">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="e5954-2866">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="e5954-2866">Usage and limits reporting</span></span>
  - <span data-ttu-id="e5954-2867">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="e5954-2867">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="e5954-2868">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2868">Support for custom images</span></span>
  - <span data-ttu-id="e5954-2869">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="e5954-2869">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e5954-2870">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-2870">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e5954-2871">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="e5954-2871">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e5954-2872">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="e5954-2872">National clouds are supported</span></span>
* <span data-ttu-id="e5954-2873">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="e5954-2873">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e5954-2874">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="e5954-2874">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e5954-2875">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-2875">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e5954-2876">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="e5954-2876">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e5954-2877">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="e5954-2877">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e5954-2878">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="e5954-2878">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e5954-2879">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2879">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e5954-2880">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="e5954-2880">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e5954-2881">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="e5954-2881">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e5954-2882">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2882">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="e5954-2883">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="e5954-2883">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e5954-2884">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="e5954-2884">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e5954-2885">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2885">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e5954-2886">Cobrança</span><span class="sxs-lookup"><span data-stu-id="e5954-2886">Billing</span></span>

* <span data-ttu-id="e5954-2887">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="e5954-2887">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-2888">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-2888">Consumption</span></span>

* <span data-ttu-id="e5954-2889">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="e5954-2889">Added `marketplace` commands</span></span>
* <span data-ttu-id="e5954-2890">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e5954-2890">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="e5954-2891">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="e5954-2891">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="e5954-2892">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="e5954-2892">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e5954-2893">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="e5954-2893">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e5954-2894">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="e5954-2894">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2895">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2895">Container</span></span>

* <span data-ttu-id="e5954-2896">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="e5954-2896">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="e5954-2897">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="e5954-2897">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-2898">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2898">Extension</span></span>

* <span data-ttu-id="e5954-2899">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="e5954-2899">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2900">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2900">Interactive</span></span>

* <span data-ttu-id="e5954-2901">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="e5954-2901">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e5954-2902">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="e5954-2902">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e5954-2903">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="e5954-2903">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2904">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2904">Network</span></span>

* <span data-ttu-id="e5954-2905">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="e5954-2905">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e5954-2906">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2906">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e5954-2907">#4910</span><span class="sxs-lookup"><span data-stu-id="e5954-2907">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e5954-2908">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e5954-2908">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e5954-2909">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="e5954-2909">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e5954-2910">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2910">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="e5954-2911">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2911">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="e5954-2912">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="e5954-2912">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-2913">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-2913">Profile</span></span>

* <span data-ttu-id="e5954-2914">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2914">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="e5954-2915">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="e5954-2915">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2916">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2916">RDBMS</span></span>

* <span data-ttu-id="e5954-2917">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="e5954-2917">Added `georestore` command</span></span>
* <span data-ttu-id="e5954-2918">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2918">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2919">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2919">Resource</span></span>

* <span data-ttu-id="e5954-2920">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2920">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="e5954-2921">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2921">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-2922">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-2922">SQL</span></span>

* <span data-ttu-id="e5954-2923">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="e5954-2923">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2924">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2924">Storage</span></span>

* <span data-ttu-id="e5954-2925">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="e5954-2925">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2926">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2926">VM</span></span>

* <span data-ttu-id="e5954-2927">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2927">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="e5954-2928">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2928">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="e5954-2930">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2930">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="e5954-2931">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="e5954-2931">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e5954-2932">#5718</span><span class="sxs-lookup"><span data-stu-id="e5954-2932">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e5954-2933">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="e5954-2933">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e5954-2934">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2934">March 27, 2018</span></span>

<span data-ttu-id="e5954-2935">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e5954-2935">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e5954-2936">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-2936">Core</span></span>

* <span data-ttu-id="e5954-2937">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="e5954-2937">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2938">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2938">ACS</span></span>

* <span data-ttu-id="e5954-2939">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5954-2939">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-2940">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-2940">Appservice</span></span>

* <span data-ttu-id="e5954-2941">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e5954-2941">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e5954-2942">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2942">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-2943">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-2943">Backup</span></span>

* <span data-ttu-id="e5954-2944">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2944">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e5954-2945">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-2945">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e5954-2946">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e5954-2946">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e5954-2947">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e5954-2947">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5954-2948">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2948">Container</span></span>

* <span data-ttu-id="e5954-2949">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="e5954-2949">Added `container exec` command.</span></span> <span data-ttu-id="e5954-2950">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="e5954-2950">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e5954-2951">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-2951">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-2952">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-2952">Extension</span></span>

* <span data-ttu-id="e5954-2953">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-2953">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e5954-2954">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e5954-2954">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e5954-2955">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-2955">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-2956">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-2956">Interactive</span></span>

* <span data-ttu-id="e5954-2957">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2957">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e5954-2958">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="e5954-2958">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e5954-2959">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-2959">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e5954-2960">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="e5954-2960">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-2961">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-2961">Lab</span></span>

* <span data-ttu-id="e5954-2962">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="e5954-2962">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-2963">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-2963">Monitor</span></span>

* <span data-ttu-id="e5954-2964">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e5954-2964">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e5954-2965">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="e5954-2965">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e5954-2966">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e5954-2966">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e5954-2967">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-2967">Network</span></span>

* <span data-ttu-id="e5954-2968">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="e5954-2968">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-2969">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-2969">Profile</span></span>

* <span data-ttu-id="e5954-2970">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="e5954-2970">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-2971">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-2971">RDBMS</span></span>

* <span data-ttu-id="e5954-2972">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e5954-2972">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-2973">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-2973">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e5954-2975">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-2975">Role</span></span>

* <span data-ttu-id="e5954-2976">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e5954-2976">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e5954-2977">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="e5954-2977">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e5954-2978">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2978">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e5954-2979">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2979">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e5954-2980">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="e5954-2980">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-2981">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-2981">Storage</span></span>

* <span data-ttu-id="e5954-2982">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="e5954-2982">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e5954-2983">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="e5954-2983">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-2984">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-2984">VM</span></span>

* <span data-ttu-id="e5954-2985">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="e5954-2985">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e5954-2986">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e5954-2986">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e5954-2987">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="e5954-2987">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e5954-2988">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="e5954-2988">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e5954-2989">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-2989">March 13, 2018</span></span>

<span data-ttu-id="e5954-2990">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e5954-2990">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-2991">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-2991">ACR</span></span>

* <span data-ttu-id="e5954-2992">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-2992">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e5954-2993">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-2993">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e5954-2994">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="e5954-2994">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-2995">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-2995">ACS</span></span>

* <span data-ttu-id="e5954-2996">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="e5954-2996">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e5954-2997">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="e5954-2997">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e5954-2998">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e5954-2998">Advisor</span></span>

* <span data-ttu-id="e5954-2999">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e5954-2999">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e5954-3000">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3000">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e5954-3001">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="e5954-3001">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="e5954-3002">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e5954-3002">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e5954-3003">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3003">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3004">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3004">Appservice</span></span>

* <span data-ttu-id="e5954-3005">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="e5954-3005">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e5954-3006">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3006">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e5954-3007">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-3007">Eventhubs</span></span>

* <span data-ttu-id="e5954-3008">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3008">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-3009">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-3009">Extension</span></span>

* <span data-ttu-id="e5954-3010">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="e5954-3010">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-3011">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3011">Interactive</span></span>

* <span data-ttu-id="e5954-3012">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="e5954-3012">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e5954-3013">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="e5954-3013">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e5954-3014">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="e5954-3014">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e5954-3015">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="e5954-3015">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3016">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3016">Monitor</span></span>

* <span data-ttu-id="e5954-3017">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-3017">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e5954-3018">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e5954-3018">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e5954-3019">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e5954-3019">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e5954-3020">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-3020">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3021">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3021">Network</span></span>

* <span data-ttu-id="e5954-3022">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3022">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e5954-3023">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e5954-3023">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e5954-3024">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3024">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e5954-3025">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e5954-3025">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3026">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3026">Profile</span></span>

* <span data-ttu-id="e5954-3027">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="e5954-3027">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e5954-3028">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="e5954-3028">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-3029">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-3029">RDBMS</span></span>

* <span data-ttu-id="e5954-3030">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="e5954-3030">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e5954-3031">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-3031">Service Bus</span></span>

* <span data-ttu-id="e5954-3032">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3032">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3033">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3033">Storage</span></span>

* <span data-ttu-id="e5954-3034">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-3034">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e5954-3035">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="e5954-3035">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3036">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3036">VM</span></span>

* <span data-ttu-id="e5954-3037">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="e5954-3037">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e5954-3038">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-3038">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e5954-3039">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="e5954-3039">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e5954-3040">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="e5954-3040">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e5954-3041">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-3041">February 27, 2018</span></span>

<span data-ttu-id="e5954-3042">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e5954-3042">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3043">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3043">Core</span></span>

* <span data-ttu-id="e5954-3044">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="e5954-3044">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e5954-3045">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="e5954-3045">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e5954-3046">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="e5954-3046">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3047">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3047">ACS</span></span>

* <span data-ttu-id="e5954-3048">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3048">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e5954-3049">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="e5954-3049">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e5954-3050">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e5954-3050">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e5954-3051">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e5954-3051">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3052">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3052">Appservice</span></span>

* <span data-ttu-id="e5954-3053">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e5954-3053">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e5954-3054">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-3054">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e5954-3055">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-3055">Cognitive Services</span></span>

* <span data-ttu-id="e5954-3056">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-3056">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-3057">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-3057">Consumption</span></span>

* <span data-ttu-id="e5954-3058">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="e5954-3058">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e5954-3059">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="e5954-3059">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3060">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3060">Container</span></span>

* <span data-ttu-id="e5954-3061">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="e5954-3061">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3062">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3062">Network</span></span>

* <span data-ttu-id="e5954-3063">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e5954-3063">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3064">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3064">Resource</span></span>

* <span data-ttu-id="e5954-3065">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="e5954-3065">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3066">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3066">Role</span></span>

* <span data-ttu-id="e5954-3067">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-3067">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3068">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3068">SQL</span></span>

* <span data-ttu-id="e5954-3069">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="e5954-3069">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3070">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3070">Storage</span></span>

* <span data-ttu-id="e5954-3071">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3071">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3072">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3072">VM</span></span>

* <span data-ttu-id="e5954-3073">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-3073">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e5954-3074">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-3074">February 13, 2018</span></span>

<span data-ttu-id="e5954-3075">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e5954-3075">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3076">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3076">Core</span></span>

* <span data-ttu-id="e5954-3077">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="e5954-3077">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3078">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3078">ACS</span></span>

* <span data-ttu-id="e5954-3079">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="e5954-3079">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e5954-3080">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3080">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e5954-3081">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-3081">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e5954-3082">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-3082">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e5954-3083">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="e5954-3083">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e5954-3084">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e5954-3084">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e5954-3085">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-3085">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e5954-3086">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e5954-3086">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3087">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3087">Appservice</span></span>

* <span data-ttu-id="e5954-3088">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="e5954-3088">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e5954-3089">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e5954-3089">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-3090">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-3090">CDN</span></span>

* <span data-ttu-id="e5954-3091">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3091">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3092">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3092">Container</span></span>

* <span data-ttu-id="e5954-3093">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="e5954-3093">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e5954-3094">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3094">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-3095">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3095">CosmosDB</span></span>

* <span data-ttu-id="e5954-3096">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="e5954-3096">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-3097">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-3097">Extension</span></span>

* <span data-ttu-id="e5954-3098">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3098">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e5954-3099">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3099">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e5954-3100">Comentários</span><span class="sxs-lookup"><span data-stu-id="e5954-3100">Feedback</span></span>

* <span data-ttu-id="e5954-3101">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="e5954-3101">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-3102">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3102">Interactive</span></span>

* <span data-ttu-id="e5954-3103">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e5954-3103">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e5954-3104">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="e5954-3104">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-3105">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3105">IoT</span></span>

* <span data-ttu-id="e5954-3106">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e5954-3106">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e5954-3107">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e5954-3107">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e5954-3108">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3108">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e5954-3109">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="e5954-3109">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3110">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3110">Monitor</span></span>

* <span data-ttu-id="e5954-3111">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3111">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3112">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3112">Network</span></span>

* <span data-ttu-id="e5954-3113">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e5954-3113">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e5954-3114">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3114">Profile</span></span>

* <span data-ttu-id="e5954-3115">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3115">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3116">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3116">Resource</span></span>

* <span data-ttu-id="e5954-3117">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3117">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3118">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3118">Role</span></span>

* <span data-ttu-id="e5954-3119">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3119">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3120">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3120">SQL</span></span>

* <span data-ttu-id="e5954-3121">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e5954-3121">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e5954-3122">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e5954-3122">Added `sql db rename`</span></span>
* <span data-ttu-id="e5954-3123">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="e5954-3123">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3124">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3124">Storage</span></span>

* <span data-ttu-id="e5954-3125">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="e5954-3125">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3126">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3126">VM</span></span>

* <span data-ttu-id="e5954-3127">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="e5954-3127">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e5954-3128">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="e5954-3128">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e5954-3129">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="e5954-3129">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e5954-3130">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-3130">January 31, 2018</span></span>

<span data-ttu-id="e5954-3131">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e5954-3131">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3132">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3132">Core</span></span>

* <span data-ttu-id="e5954-3133">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="e5954-3133">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e5954-3134">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="e5954-3134">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e5954-3135">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="e5954-3135">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e5954-3136">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="e5954-3136">Use `--verbose` to see</span></span>
* <span data-ttu-id="e5954-3137">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="e5954-3137">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3138">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3138">ACS</span></span>

* <span data-ttu-id="e5954-3139">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="e5954-3139">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e5954-3140">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e5954-3140">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3141">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3141">Appservice</span></span>

* <span data-ttu-id="e5954-3142">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="e5954-3142">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e5954-3143">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="e5954-3143">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-3144">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-3144">CDN</span></span>

* <span data-ttu-id="e5954-3145">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3145">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-3146">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3146">CosmosDB</span></span>

* <span data-ttu-id="e5954-3147">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="e5954-3147">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-3148">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3148">Interactive</span></span>

* <span data-ttu-id="e5954-3149">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="e5954-3149">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3150">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3150">Network</span></span>

* <span data-ttu-id="e5954-3151">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3151">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e5954-3152">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="e5954-3152">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e5954-3153">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3153">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e5954-3154">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3154">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e5954-3155">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e5954-3155">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e5954-3156">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="e5954-3156">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e5954-3157">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3157">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e5954-3158">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="e5954-3158">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e5954-3159">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e5954-3159">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="e5954-3160">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e5954-3160">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3161">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3161">Profile</span></span>

* <span data-ttu-id="e5954-3162">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="e5954-3162">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3163">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3163">Resource</span></span>

* <span data-ttu-id="e5954-3164">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="e5954-3164">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3165">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3165">Storage</span></span>

* <span data-ttu-id="e5954-3166">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e5954-3166">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e5954-3167">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="e5954-3167">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e5954-3168">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-3168">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="e5954-3169">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3169">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e5954-3170">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="e5954-3170">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3171">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3171">VM</span></span>

* <span data-ttu-id="e5954-3172">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="e5954-3172">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e5954-3173">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="e5954-3173">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e5954-3174">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="e5954-3174">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e5954-3175">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3175">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e5954-3176">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e5954-3176">January 17, 2018</span></span>

<span data-ttu-id="e5954-3177">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e5954-3177">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-3178">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3178">ACR</span></span>

* <span data-ttu-id="e5954-3179">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-3179">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e5954-3180">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="e5954-3180">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3181">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3181">ACS</span></span>

* <span data-ttu-id="e5954-3182">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e5954-3182">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e5954-3183">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="e5954-3183">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3184">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3184">Appservice</span></span>

* <span data-ttu-id="e5954-3185">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="e5954-3185">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e5954-3186">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="e5954-3186">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e5954-3187">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="e5954-3187">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-3188">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-3188">Backup</span></span>

* <span data-ttu-id="e5954-3189">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="e5954-3189">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e5954-3190">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e5954-3190">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e5954-3191">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-3191">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e5954-3192">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="e5954-3192">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e5954-3193">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3193">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-3194">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3194">Batch</span></span>

* <span data-ttu-id="e5954-3195">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="e5954-3195">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e5954-3196">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-3196">Cloud</span></span>

* <span data-ttu-id="e5954-3197">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-3197">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-3198">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-3198">Consumption</span></span>

* <span data-ttu-id="e5954-3199">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e5954-3199">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5954-3200">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-3200">Event Grid</span></span>

* <span data-ttu-id="e5954-3201">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e5954-3201">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e5954-3202">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e5954-3202">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e5954-3203">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="e5954-3203">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e5954-3204">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e5954-3204">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e5954-3205">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3205">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e5954-3206">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3206">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e5954-3207">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e5954-3207">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e5954-3208">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="e5954-3208">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-3209">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3209">Interactive</span></span>

* <span data-ttu-id="e5954-3210">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e5954-3210">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e5954-3211">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="e5954-3211">Fixed errors on startup</span></span>
* <span data-ttu-id="e5954-3212">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3212">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-3213">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3213">IoT</span></span>

* <span data-ttu-id="e5954-3214">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e5954-3214">Added support for device provisioning service</span></span>
* <span data-ttu-id="e5954-3215">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="e5954-3215">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e5954-3216">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3216">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3217">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3217">Monitor</span></span>

* <span data-ttu-id="e5954-3218">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="e5954-3218">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e5954-3219">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3219">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e5954-3220">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e5954-3220">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3221">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3221">Network</span></span>

* <span data-ttu-id="e5954-3222">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3222">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e5954-3223">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3223">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3224">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3224">Profile</span></span>

* <span data-ttu-id="e5954-3225">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-3225">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3226">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3226">Role</span></span>

* <span data-ttu-id="e5954-3227">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="e5954-3227">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5954-3228">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-3228">Service Fabric</span></span>

* <span data-ttu-id="e5954-3229">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="e5954-3229">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e5954-3230">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="e5954-3230">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3231">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3231">VM</span></span>

* <span data-ttu-id="e5954-3232">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="e5954-3232">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e5954-3233">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="e5954-3233">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e5954-3234">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="e5954-3234">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e5954-3235">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e5954-3235">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e5954-3236">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="e5954-3236">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e5954-3237">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3237">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5954-3238">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3238">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5954-3239">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e5954-3239">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e5954-3240">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3240">December 19, 2017</span></span>

<span data-ttu-id="e5954-3241">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e5954-3241">Version 2.0.23</span></span>

* <span data-ttu-id="e5954-3242">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e5954-3242">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3243">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3243">Container</span></span>

* <span data-ttu-id="e5954-3244">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3244">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3245">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3245">Network</span></span>

* <span data-ttu-id="e5954-3246">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3246">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e5954-3247">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3247">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3248">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3248">Storage</span></span>

* <span data-ttu-id="e5954-3249">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e5954-3249">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3250">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3250">VM</span></span>

* <span data-ttu-id="e5954-3251">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="e5954-3251">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e5954-3252">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3252">December 5, 2017</span></span>

<span data-ttu-id="e5954-3253">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e5954-3253">Version 2.0.22</span></span>

* <span data-ttu-id="e5954-3254">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="e5954-3254">Removed `az component` commands.</span></span> <span data-ttu-id="e5954-3255">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="e5954-3255">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3256">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3256">Core</span></span>
* <span data-ttu-id="e5954-3257">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e5954-3257">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e5954-3258">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3258">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3259">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3259">ACS</span></span>

* <span data-ttu-id="e5954-3260">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3260">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e5954-3261">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3261">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e5954-3262">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="e5954-3262">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e5954-3263">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e5954-3263">Advisor</span></span>

* <span data-ttu-id="e5954-3264">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3264">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3265">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3265">Appservice</span></span>

* <span data-ttu-id="e5954-3266">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e5954-3266">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e5954-3267">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="e5954-3267">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e5954-3268">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e5954-3268">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e5954-3269">Consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-3269">Consumption</span></span>

* <span data-ttu-id="e5954-3270">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3270">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3271">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3271">Container</span></span>

* <span data-ttu-id="e5954-3272">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3272">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3273">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3273">Monitor</span></span>

* <span data-ttu-id="e5954-3274">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="e5954-3274">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3275">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3275">Resource</span></span>

* <span data-ttu-id="e5954-3276">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3276">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3277">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3277">Role</span></span>

* <span data-ttu-id="e5954-3278">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e5954-3278">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e5954-3279">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="e5954-3279">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e5954-3280">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e5954-3280">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3281">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3281">SQL</span></span>

* <span data-ttu-id="e5954-3282">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3282">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e5954-3283">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3283">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3284">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3284">VM</span></span>

* <span data-ttu-id="e5954-3285">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e5954-3285">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e5954-3286">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3286">November 14, 2017</span></span>

<span data-ttu-id="e5954-3287">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e5954-3287">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-3288">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3288">ACR</span></span>

* <span data-ttu-id="e5954-3289">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="e5954-3289">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e5954-3290">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3290">ACS</span></span>

* <span data-ttu-id="e5954-3291">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="e5954-3291">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e5954-3292">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3292">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e5954-3293">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e5954-3293">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e5954-3294">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-3294">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e5954-3295">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e5954-3295">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3296">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3296">Appservice</span></span>

* <span data-ttu-id="e5954-3297">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e5954-3297">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e5954-3298">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e5954-3298">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e5954-3299">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e5954-3299">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e5954-3300">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e5954-3300">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e5954-3301">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-3301">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e5954-3302">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="e5954-3302">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-3303">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3303">Batch</span></span>

* <span data-ttu-id="e5954-3304">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="e5954-3304">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-3305">Batchai</span><span class="sxs-lookup"><span data-stu-id="e5954-3305">Batchai</span></span>

* <span data-ttu-id="e5954-3306">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3306">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e5954-3307">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3307">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e5954-3308">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e5954-3308">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e5954-3309">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3309">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e5954-3310">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-3310">Cloud</span></span>

* <span data-ttu-id="e5954-3311">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="e5954-3311">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3312">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3312">Container</span></span>

* <span data-ttu-id="e5954-3313">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="e5954-3313">Added support to open multiple ports</span></span>
* <span data-ttu-id="e5954-3314">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="e5954-3314">Added container group restart policy</span></span>
* <span data-ttu-id="e5954-3315">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="e5954-3315">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e5954-3316">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="e5954-3316">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5954-3317">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-3317">Data Lake Analytics</span></span>

* <span data-ttu-id="e5954-3318">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e5954-3318">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5954-3319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3319">Data Lake Store</span></span>

* <span data-ttu-id="e5954-3320">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e5954-3320">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-3321">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-3321">Extension</span></span>

* <span data-ttu-id="e5954-3322">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e5954-3322">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e5954-3323">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="e5954-3323">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-3324">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3324">IoT</span></span>

* <span data-ttu-id="e5954-3325">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="e5954-3325">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3326">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3326">Monitor</span></span>

* <span data-ttu-id="e5954-3327">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e5954-3327">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3328">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3328">Network</span></span>

* <span data-ttu-id="e5954-3329">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="e5954-3329">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e5954-3330">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3330">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e5954-3331">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="e5954-3331">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e5954-3332">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e5954-3332">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e5954-3333">Reservas</span><span class="sxs-lookup"><span data-stu-id="e5954-3333">Reservations</span></span>

* <span data-ttu-id="e5954-3334">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3334">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3335">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3335">Resource</span></span>

* <span data-ttu-id="e5954-3336">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3336">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3337">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3337">SQL</span></span>

* <span data-ttu-id="e5954-3338">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3338">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3339">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3339">Storage</span></span>

* <span data-ttu-id="e5954-3340">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3340">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e5954-3341">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="e5954-3341">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e5954-3342">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e5954-3342">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e5954-3343">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e5954-3343">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e5954-3344">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3344">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e5954-3345">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e5954-3345">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e5954-3346">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3346">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3347">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3347">VM</span></span>

* <span data-ttu-id="e5954-3348">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="e5954-3348">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e5954-3349">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="e5954-3349">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e5954-3350">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3350">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e5954-3351">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e5954-3351">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e5954-3352">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e5954-3352">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e5954-3353">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3353">October 24, 2017</span></span>

<span data-ttu-id="e5954-3354">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e5954-3354">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3355">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3355">Core</span></span>

* <span data-ttu-id="e5954-3356">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e5954-3356">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-3357">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3357">ACR</span></span>

* <span data-ttu-id="e5954-3358">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e5954-3358">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e5954-3359">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="e5954-3359">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e5954-3360">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="e5954-3360">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3361">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3361">ACS</span></span>

* <span data-ttu-id="e5954-3362">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="e5954-3362">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e5954-3363">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="e5954-3363">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3364">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3364">Appservice</span></span>

* <span data-ttu-id="e5954-3365">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="e5954-3365">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e5954-3366">Componente</span><span class="sxs-lookup"><span data-stu-id="e5954-3366">Component</span></span>

* <span data-ttu-id="e5954-3367">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="e5954-3367">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3368">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3368">Monitor</span></span>

* <span data-ttu-id="e5954-3369">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="e5954-3369">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3370">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3370">Resource</span></span>

* <span data-ttu-id="e5954-3371">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="e5954-3371">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e5954-3372">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="e5954-3372">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3373">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3373">VM</span></span>

* <span data-ttu-id="e5954-3374">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3374">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e5954-3375">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3375">October 9, 2017</span></span>

<span data-ttu-id="e5954-3376">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e5954-3376">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3377">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3377">Core</span></span>

* <span data-ttu-id="e5954-3378">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5954-3378">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3379">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3379">Appservice</span></span>

* <span data-ttu-id="e5954-3380">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3380">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-3381">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3381">Batch</span></span>

* <span data-ttu-id="e5954-3382">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-3382">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e5954-3383">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="e5954-3383">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e5954-3384">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3384">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e5954-3385">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="e5954-3385">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e5954-3386">Batchai</span><span class="sxs-lookup"><span data-stu-id="e5954-3386">Batchai</span></span>

* <span data-ttu-id="e5954-3387">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3387">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-3388">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-3388">Keyvault</span></span>

* <span data-ttu-id="e5954-3389">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e5954-3389">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e5954-3390">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e5954-3390">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e5954-3391">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3391">Network</span></span>

* <span data-ttu-id="e5954-3392">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="e5954-3392">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e5954-3393">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="e5954-3393">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3394">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3394">Resource</span></span>

* <span data-ttu-id="e5954-3395">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="e5954-3395">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e5954-3396">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-3396">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e5954-3397">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="e5954-3397">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e5954-3398">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3398">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3399">Sql</span><span class="sxs-lookup"><span data-stu-id="e5954-3399">Sql</span></span>

* <span data-ttu-id="e5954-3400">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="e5954-3400">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e5954-3401">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="e5954-3401">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e5954-3402">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="e5954-3402">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3403">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3403">Storage</span></span>

* <span data-ttu-id="e5954-3404">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="e5954-3404">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3405">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3405">Vm</span></span>

* <span data-ttu-id="e5954-3406">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="e5954-3406">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e5954-3407">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3407">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e5954-3408">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e5954-3408">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e5954-3409">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3409">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e5954-3410">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3410">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e5954-3411">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3411">September 22, 2017</span></span>

<span data-ttu-id="e5954-3412">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="e5954-3412">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3413">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3413">Resource</span></span>

* <span data-ttu-id="e5954-3414">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="e5954-3414">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e5954-3415">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="e5954-3415">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e5954-3416">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3416">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e5954-3417">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e5954-3417">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3418">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3418">Network</span></span>

* <span data-ttu-id="e5954-3419">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e5954-3419">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e5954-3420">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="e5954-3420">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e5954-3421">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3421">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e5954-3422">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3422">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e5954-3423">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3423">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e5954-3424">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3424">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e5954-3425">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3425">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3426">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3426">Storage</span></span>

* <span data-ttu-id="e5954-3427">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="e5954-3427">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e5954-3428">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-3428">Eventgrid</span></span>

* <span data-ttu-id="e5954-3429">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="e5954-3429">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3430">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3430">SQL</span></span>

* <span data-ttu-id="e5954-3431">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="e5954-3431">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e5954-3432">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="e5954-3432">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e5954-3433">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3433">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-3434">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-3434">Keyvault</span></span>

* <span data-ttu-id="e5954-3435">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="e5954-3435">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3436">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3436">VM</span></span>

* <span data-ttu-id="e5954-3437">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3437">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e5954-3438">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="e5954-3438">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e5954-3439">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3439">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e5954-3440">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e5954-3440">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e5954-3441">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e5954-3441">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e5954-3442">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e5954-3442">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3443">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3443">ACS</span></span>

* <span data-ttu-id="e5954-3444">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3444">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3445">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3445">Appservice</span></span>

* <span data-ttu-id="e5954-3446">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3446">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e5954-3447">Backup</span><span class="sxs-lookup"><span data-stu-id="e5954-3447">Backup</span></span>

* <span data-ttu-id="e5954-3448">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-3448">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e5954-3449">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3449">September 11, 2017</span></span>

<span data-ttu-id="e5954-3450">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e5954-3450">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e5954-3451">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3451">Core</span></span>

* <span data-ttu-id="e5954-3452">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="e5954-3452">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e5954-3453">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e5954-3453">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3454">Acs</span><span class="sxs-lookup"><span data-stu-id="e5954-3454">Acs</span></span>

* <span data-ttu-id="e5954-3455">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e5954-3455">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e5954-3456">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="e5954-3456">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3457">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3457">Appservice</span></span>

* <span data-ttu-id="e5954-3458">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3458">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-3459">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-3459">CDN</span></span>

* <span data-ttu-id="e5954-3460">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3460">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e5954-3461">Extensão</span><span class="sxs-lookup"><span data-stu-id="e5954-3461">Extension</span></span>

* <span data-ttu-id="e5954-3462">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3462">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-3463">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-3463">Keyvault</span></span>

* <span data-ttu-id="e5954-3464">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-3464">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3465">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3465">Network</span></span>

* <span data-ttu-id="e5954-3466">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e5954-3466">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e5954-3467">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3467">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e5954-3468">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3468">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e5954-3469">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3469">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e5954-3470">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3470">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3471">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3471">Resource</span></span>

* <span data-ttu-id="e5954-3472">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3472">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e5954-3473">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3473">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e5954-3474">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="e5954-3474">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e5954-3475">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="e5954-3475">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3476">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3476">SQL</span></span>

* <span data-ttu-id="e5954-3477">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e5954-3477">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3478">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3478">VM</span></span>

* <span data-ttu-id="e5954-3479">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="e5954-3479">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e5954-3480">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="e5954-3480">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e5954-3481">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3481">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e5954-3482">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-3482">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e5954-3483">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="e5954-3483">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e5954-3484">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3484">August 31, 2017</span></span>

<span data-ttu-id="e5954-3485">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e5954-3485">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-3486">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e5954-3486">Keyvault</span></span>

* <span data-ttu-id="e5954-3487">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="e5954-3487">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e5954-3488">Sf</span><span class="sxs-lookup"><span data-stu-id="e5954-3488">Sf</span></span>

* <span data-ttu-id="e5954-3489">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e5954-3489">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3490">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3490">Storage</span></span>

* <span data-ttu-id="e5954-3491">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="e5954-3491">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e5954-3492">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="e5954-3492">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e5954-3493">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3493">August 28, 2017</span></span>

<span data-ttu-id="e5954-3494">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e5954-3494">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e5954-3495">CLI</span><span class="sxs-lookup"><span data-stu-id="e5954-3495">CLI</span></span>

* <span data-ttu-id="e5954-3496">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="e5954-3496">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3497">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3497">ACS</span></span>

* <span data-ttu-id="e5954-3498">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e5954-3498">Corrected preview regions</span></span>
* <span data-ttu-id="e5954-3499">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="e5954-3499">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e5954-3500">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="e5954-3500">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3501">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3501">Appservice</span></span>

* <span data-ttu-id="e5954-3502">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3502">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e5954-3503">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-3503">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e5954-3504">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3504">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e5954-3505">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3505">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e5954-3506">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3506">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-3507">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3507">IoT</span></span>

* <span data-ttu-id="e5954-3508">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="e5954-3508">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3509">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3509">Network</span></span>

* <span data-ttu-id="e5954-3510">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e5954-3510">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e5954-3511">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3511">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e5954-3512">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e5954-3512">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e5954-3513">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3513">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e5954-3514">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3514">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3515">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3515">Profile</span></span>

* <span data-ttu-id="e5954-3516">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="e5954-3516">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5954-3517">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-3517">Service Fabric</span></span>

* <span data-ttu-id="e5954-3518">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e5954-3518">Preview release</span></span>
* <span data-ttu-id="e5954-3519">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="e5954-3519">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e5954-3520">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e5954-3520">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e5954-3521">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="e5954-3521">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3522">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3522">Storage</span></span>

* <span data-ttu-id="e5954-3523">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="e5954-3523">Enabled setting blob tier</span></span>
* <span data-ttu-id="e5954-3524">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="e5954-3524">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e5954-3525">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="e5954-3525">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e5954-3526">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="e5954-3526">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e5954-3527">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3527">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e5954-3528">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="e5954-3528">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3529">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3529">VM</span></span>

* <span data-ttu-id="e5954-3530">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e5954-3530">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e5954-3531">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-3531">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e5954-3532">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3532">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e5954-3533">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e5954-3533">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e5954-3534">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="e5954-3534">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e5954-3535">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3535">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e5954-3536">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3536">August 15, 2017</span></span>

<span data-ttu-id="e5954-3537">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e5954-3537">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3538">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3538">ACS</span></span>

* <span data-ttu-id="e5954-3539">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="e5954-3539">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3540">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3540">Appservice</span></span>

* <span data-ttu-id="e5954-3541">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="e5954-3541">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5954-3542">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-3542">Event Grid</span></span>

* <span data-ttu-id="e5954-3543">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="e5954-3543">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e5954-3544">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3544">August 11, 2017</span></span>

<span data-ttu-id="e5954-3545">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e5954-3545">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3546">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3546">ACS</span></span>

* <span data-ttu-id="e5954-3547">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e5954-3547">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-3548">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3548">Batch</span></span>

* <span data-ttu-id="e5954-3549">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e5954-3549">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e5954-3550">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-3550">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e5954-3551">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3551">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e5954-3552">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="e5954-3552">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e5954-3553">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="e5954-3553">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e5954-3554">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="e5954-3554">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e5954-3555">Componente</span><span class="sxs-lookup"><span data-stu-id="e5954-3555">Component</span></span>

* <span data-ttu-id="e5954-3556">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="e5954-3556">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e5954-3557">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3557">Container</span></span>

* <span data-ttu-id="e5954-3558">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="e5954-3558">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e5954-3559">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3559">Data Lake Store</span></span>

* <span data-ttu-id="e5954-3560">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3560">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e5954-3561">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e5954-3561">Event Grid</span></span>

* <span data-ttu-id="e5954-3562">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e5954-3562">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3563">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3563">Network</span></span>

* <span data-ttu-id="e5954-3564">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="e5954-3564">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e5954-3565">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="e5954-3565">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e5954-3566">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="e5954-3566">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e5954-3567">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e5954-3567">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3568">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3568">Profile</span></span>

* <span data-ttu-id="e5954-3569">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="e5954-3569">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3570">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3570">Storage</span></span>

* <span data-ttu-id="e5954-3571">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e5954-3571">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3572">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3572">VM</span></span>

* <span data-ttu-id="e5954-3573">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="e5954-3573">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e5954-3574">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="e5954-3574">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e5954-3575">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="e5954-3575">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e5954-3576">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="e5954-3576">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e5954-3577">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-3577">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e5954-3578">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3578">July 28, 2017</span></span>

<span data-ttu-id="e5954-3579">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e5954-3579">Version 2.0.12</span></span>

* <span data-ttu-id="e5954-3580">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3580">Added container commands</span></span>
* <span data-ttu-id="e5954-3581">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="e5954-3581">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e5954-3582">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3582">Core</span></span>

* <span data-ttu-id="e5954-3583">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="e5954-3583">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e5954-3584">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="e5954-3584">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e5954-3585">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="e5954-3585">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e5954-3586">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e5954-3586">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e5954-3587">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="e5954-3587">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e5954-3588">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="e5954-3588">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e5954-3589">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e5954-3589">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e5954-3590">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e5954-3590">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e5954-3591">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="e5954-3591">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e5954-3592">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="e5954-3592">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e5954-3593">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="e5954-3593">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e5954-3594">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="e5954-3594">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e5954-3595">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-3595">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e5954-3596">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e5954-3596">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e5954-3597">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e5954-3597">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e5954-3598">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e5954-3598">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e5954-3599">ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3599">ACR</span></span>

* <span data-ttu-id="e5954-3600">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-3600">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e5954-3601">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e5954-3601">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e5954-3602">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="e5954-3602">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e5954-3603">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3603">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e5954-3604">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3604">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e5954-3605">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="e5954-3605">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3606">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3606">ACS</span></span>

* <span data-ttu-id="e5954-3607">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e5954-3607">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3608">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3608">Appservice</span></span>

* <span data-ttu-id="e5954-3609">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="e5954-3609">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e5954-3610">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="e5954-3610">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e5954-3611">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e5954-3611">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e5954-3612">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="e5954-3612">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e5954-3613">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="e5954-3613">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e5954-3614">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e5954-3614">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e5954-3615">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="e5954-3615">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e5954-3616">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="e5954-3616">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e5954-3617">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="e5954-3617">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e5954-3618">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e5954-3618">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e5954-3619">Lote</span><span class="sxs-lookup"><span data-stu-id="e5954-3619">Batch</span></span>

* <span data-ttu-id="e5954-3620">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="e5954-3620">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e5954-3621">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e5954-3621">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e5954-3622">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e5954-3622">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e5954-3623">CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-3623">CDN</span></span>

* <span data-ttu-id="e5954-3624">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="e5954-3624">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e5954-3625">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e5954-3625">Cloud</span></span>

* <span data-ttu-id="e5954-3626">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="e5954-3626">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e5954-3627">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="e5954-3627">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e5954-3628">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="e5954-3628">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e5954-3629">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="e5954-3629">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e5954-3630">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e5954-3630">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-3631">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3631">CosmosDB</span></span>

* <span data-ttu-id="e5954-3632">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="e5954-3632">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e5954-3633">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="e5954-3633">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5954-3634">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-3634">Data Lake Analytics</span></span>

* <span data-ttu-id="e5954-3635">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e5954-3635">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e5954-3636">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3636">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e5954-3637">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e5954-3637">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5954-3638">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3638">Data Lake Store</span></span>

* <span data-ttu-id="e5954-3639">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3639">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e5954-3640">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="e5954-3640">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e5954-3641">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e5954-3641">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e5954-3642">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3642">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e5954-3643">Interativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3643">Interactive</span></span>

* <span data-ttu-id="e5954-3644">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="e5954-3644">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e5954-3645">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="e5954-3645">Increased test coverage</span></span>
* <span data-ttu-id="e5954-3646">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="e5954-3646">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e5954-3647">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e5954-3647">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e5954-3648">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="e5954-3648">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e5954-3649">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="e5954-3649">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e5954-3650">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e5954-3650">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e5954-3651">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="e5954-3651">Added `--progress` flag</span></span>
* <span data-ttu-id="e5954-3652">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="e5954-3652">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e5954-3653">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="e5954-3653">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e5954-3654">IoT</span><span class="sxs-lookup"><span data-stu-id="e5954-3654">IoT</span></span>

* <span data-ttu-id="e5954-3655">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="e5954-3655">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e5954-3656">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e5954-3656">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e5954-3657">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="e5954-3657">Key vault</span></span>

* <span data-ttu-id="e5954-3658">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="e5954-3658">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e5954-3659">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="e5954-3659">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e5954-3660">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="e5954-3660">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e5954-3661">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="e5954-3661">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e5954-3662">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="e5954-3662">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e5954-3663">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="e5954-3663">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e5954-3664">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e5954-3664">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e5954-3665">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e5954-3665">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-3666">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3666">Lab</span></span>

* <span data-ttu-id="e5954-3667">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e5954-3667">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e5954-3668">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3668">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3669">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3669">Monitor</span></span>

* <span data-ttu-id="e5954-3670">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="e5954-3670">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e5954-3671">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e5954-3671">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e5954-3672">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e5954-3672">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e5954-3673">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e5954-3673">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e5954-3674">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e5954-3674">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e5954-3675">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e5954-3675">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e5954-3676">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="e5954-3676">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e5954-3677">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="e5954-3677">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e5954-3678">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e5954-3678">`location` no longer required</span></span>
  * <span data-ttu-id="e5954-3679">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="e5954-3679">Add name and ID support for target</span></span>
  * <span data-ttu-id="e5954-3680">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-3680">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e5954-3681">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e5954-3681">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e5954-3682">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="e5954-3682">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e5954-3683">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="e5954-3683">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e5954-3684">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e5954-3684">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e5954-3685">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3685">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3686">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3686">Network</span></span>

* <span data-ttu-id="e5954-3687">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e5954-3687">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e5954-3688">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3688">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e5954-3689">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="e5954-3689">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e5954-3690">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e5954-3690">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e5954-3691">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3691">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e5954-3692">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e5954-3692">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e5954-3693">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3693">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e5954-3694">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e5954-3694">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e5954-3695">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e5954-3695">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e5954-3696">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e5954-3696">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e5954-3697">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3697">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e5954-3698">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e5954-3698">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e5954-3699">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e5954-3699">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e5954-3700">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3700">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e5954-3701">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3701">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e5954-3702">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3702">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e5954-3703">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="e5954-3703">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e5954-3704">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e5954-3704">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e5954-3705">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3705">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e5954-3706">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3706">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e5954-3707">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3707">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e5954-3708">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e5954-3708">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e5954-3709">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e5954-3709">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e5954-3710">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e5954-3710">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e5954-3711">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e5954-3711">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e5954-3712">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e5954-3712">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e5954-3713">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e5954-3713">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3714">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3714">Profile</span></span>

* <span data-ttu-id="e5954-3715">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e5954-3715">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e5954-3716">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="e5954-3716">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e5954-3717">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="e5954-3717">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e5954-3718">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="e5954-3718">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e5954-3719">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="e5954-3719">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e5954-3720">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e5954-3720">RDBMS</span></span>

* <span data-ttu-id="e5954-3721">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="e5954-3721">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e5954-3722">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e5954-3722">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e5954-3723">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="e5954-3723">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e5954-3724">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e5954-3724">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3725">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3725">Resource</span></span>

* <span data-ttu-id="e5954-3726">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3726">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e5954-3727">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e5954-3727">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e5954-3728">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="e5954-3728">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e5954-3729">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e5954-3729">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e5954-3730">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="e5954-3730">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e5954-3731">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e5954-3731">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e5954-3732">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="e5954-3732">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e5954-3733">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e5954-3733">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3734">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3734">Role</span></span>

* <span data-ttu-id="e5954-3735">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e5954-3735">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e5954-3736">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="e5954-3736">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e5954-3737">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="e5954-3737">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e5954-3738">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e5954-3738">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e5954-3739">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e5954-3739">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e5954-3740">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-3740">Service Fabric</span></span>
* <span data-ttu-id="e5954-3741">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="e5954-3741">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e5954-3742">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e5954-3742">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e5954-3743">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e5954-3743">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3744">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3744">SQL</span></span>

* <span data-ttu-id="e5954-3745">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="e5954-3745">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e5954-3746">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e5954-3746">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e5954-3747">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e5954-3747">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3748">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3748">Storage</span></span>

* <span data-ttu-id="e5954-3749">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e5954-3749">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e5954-3750">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="e5954-3750">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e5954-3751">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="e5954-3751">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e5954-3752">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e5954-3752">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e5954-3753">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="e5954-3753">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e5954-3754">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e5954-3754">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3755">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3755">VM</span></span>

* <span data-ttu-id="e5954-3756">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="e5954-3756">Support configuring nsg</span></span>
* <span data-ttu-id="e5954-3757">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3757">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e5954-3758">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="e5954-3758">Support managed service identities</span></span>
* <span data-ttu-id="e5954-3759">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e5954-3759">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e5954-3760">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="e5954-3760">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e5954-3761">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3761">May 10, 2017</span></span>

<span data-ttu-id="e5954-3762">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e5954-3762">Version 2.0.6</span></span>

* <span data-ttu-id="e5954-3763">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3763">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e5954-3764">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="e5954-3764">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e5954-3765">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3765">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e5954-3766">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e5954-3766">Include Cognitive Services module</span></span>
* <span data-ttu-id="e5954-3767">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e5954-3767">Include Service Fabric module</span></span>
* <span data-ttu-id="e5954-3768">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="e5954-3768">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e5954-3769">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="e5954-3769">Add support for CDN commands</span></span>
* <span data-ttu-id="e5954-3770">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="e5954-3770">Remove Container module</span></span>
* <span data-ttu-id="e5954-3771">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e5954-3771">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e5954-3772">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e5954-3772">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e5954-3773">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3773">Core</span></span>

* <span data-ttu-id="e5954-3774">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="e5954-3774">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e5954-3775">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e5954-3775">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e5954-3776">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e5954-3776">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e5954-3777">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e5954-3777">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e5954-3778">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e5954-3778">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e5954-3779">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e5954-3779">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e5954-3780">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e5954-3780">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e5954-3781">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e5954-3781">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e5954-3782">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e5954-3782">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e5954-3783">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="e5954-3783">core: Improved performance</span></span>
* <span data-ttu-id="e5954-3784">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e5954-3784">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e5954-3785">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="e5954-3785">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3786">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3786">ACS</span></span>

* <span data-ttu-id="e5954-3787">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5954-3787">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e5954-3788">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="e5954-3788">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e5954-3789">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="e5954-3789">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e5954-3790">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e5954-3790">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3791">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3791">AppService</span></span>

* <span data-ttu-id="e5954-3792">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e5954-3792">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e5954-3793">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="e5954-3793">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e5954-3794">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="e5954-3794">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e5954-3795">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="e5954-3795">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e5954-3796">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="e5954-3796">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e5954-3797">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e5954-3797">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e5954-3798">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="e5954-3798">support slot swap with preview</span></span>
* <span data-ttu-id="e5954-3799">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e5954-3799">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e5954-3800">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e5954-3800">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e5954-3801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3801">CosmosDB</span></span>

* <span data-ttu-id="e5954-3802">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3802">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e5954-3803">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="e5954-3803">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e5954-3804">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="e5954-3804">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e5954-3805">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e5954-3805">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e5954-3806">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-3806">Data Lake Analytics</span></span>

* <span data-ttu-id="e5954-3807">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="e5954-3807">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e5954-3808">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="e5954-3808">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e5954-3809">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e5954-3809">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e5954-3810">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="e5954-3810">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e5954-3811">Tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-3811">Table</span></span>
  * <span data-ttu-id="e5954-3812">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-3812">Table valued function</span></span>
  * <span data-ttu-id="e5954-3813">Visualizar</span><span class="sxs-lookup"><span data-stu-id="e5954-3813">View</span></span>
  * <span data-ttu-id="e5954-3814">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="e5954-3814">Table Statistics.</span></span> <span data-ttu-id="e5954-3815">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="e5954-3815">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e5954-3816">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3816">Data Lake Store</span></span>

* <span data-ttu-id="e5954-3817">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="e5954-3817">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e5954-3818">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e5954-3818">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e5954-3819">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="e5954-3819">missed help for access show.</span></span> <span data-ttu-id="e5954-3820">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e5954-3820">adding it.</span></span> <span data-ttu-id="e5954-3821">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e5954-3821">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e5954-3822">Localizar</span><span class="sxs-lookup"><span data-stu-id="e5954-3822">Find</span></span>

* <span data-ttu-id="e5954-3823">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="e5954-3823">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e5954-3824">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e5954-3824">KeyVault</span></span>

* <span data-ttu-id="e5954-3825">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="e5954-3825">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e5954-3826">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="e5954-3826">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e5954-3827">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="e5954-3827">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e5954-3828">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="e5954-3828">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e5954-3829">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e5954-3829">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e5954-3830">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3830">Lab</span></span>

* <span data-ttu-id="e5954-3831">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3831">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e5954-3832">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3832">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e5954-3833">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3833">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e5954-3834">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3834">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e5954-3835">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="e5954-3835">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e5954-3836">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e5954-3836">Monitor</span></span>

* <span data-ttu-id="e5954-3837">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e5954-3837">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e5954-3838">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e5954-3838">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e5954-3839">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3839">Network</span></span>

* <span data-ttu-id="e5954-3840">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e5954-3840">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e5954-3841">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3841">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e5954-3842">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3842">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e5954-3843">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5954-3843">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e5954-3844">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e5954-3844">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e5954-3845">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="e5954-3845">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e5954-3846">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e5954-3846">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e5954-3847">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e5954-3847">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e5954-3848">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e5954-3848">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e5954-3849">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="e5954-3849">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e5954-3850">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e5954-3850">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e5954-3851">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3851">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e5954-3852">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3852">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e5954-3853">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="e5954-3853">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e5954-3854">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="e5954-3854">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e5954-3855">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="e5954-3855">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e5954-3856">Perfil</span><span class="sxs-lookup"><span data-stu-id="e5954-3856">Profile</span></span>

* <span data-ttu-id="e5954-3857">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e5954-3857">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e5954-3858">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e5954-3858">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e5954-3859">Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-3859">Redis</span></span>

* <span data-ttu-id="e5954-3860">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="e5954-3860">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e5954-3861">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="e5954-3861">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e5954-3862">Recurso</span><span class="sxs-lookup"><span data-stu-id="e5954-3862">Resource</span></span>

* <span data-ttu-id="e5954-3863">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e5954-3863">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e5954-3864">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e5954-3864">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e5954-3865">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e5954-3865">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e5954-3866">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="e5954-3866">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e5954-3867">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e5954-3867">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e5954-3868">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="e5954-3868">Add docs for az lock update.</span></span> <span data-ttu-id="e5954-3869">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e5954-3869">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e5954-3870">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="e5954-3870">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e5954-3871">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e5954-3871">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e5954-3872">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="e5954-3872">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e5954-3873">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e5954-3873">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e5954-3874">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e5954-3874">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e5954-3875">Função</span><span class="sxs-lookup"><span data-stu-id="e5954-3875">Role</span></span>

* <span data-ttu-id="e5954-3876">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e5954-3876">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e5954-3877">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e5954-3877">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e5954-3878">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e5954-3878">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e5954-3879">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="e5954-3879">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e5954-3880">SQL</span><span class="sxs-lookup"><span data-stu-id="e5954-3880">SQL</span></span>

* <span data-ttu-id="e5954-3881">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e5954-3881">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e5954-3882">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e5954-3882">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e5954-3883">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3883">Storage</span></span>

* <span data-ttu-id="e5954-3884">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e5954-3884">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e5954-3885">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="e5954-3885">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e5954-3886">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="e5954-3886">Add support for large block blob upload</span></span>
* <span data-ttu-id="e5954-3887">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="e5954-3887">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3888">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3888">VM</span></span>

* <span data-ttu-id="e5954-3889">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="e5954-3889">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e5954-3890">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="e5954-3890">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e5954-3891">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e5954-3891">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e5954-3892">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e5954-3892">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e5954-3893">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="e5954-3893">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e5954-3894">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="e5954-3894">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e5954-3895">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e5954-3895">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e5954-3896">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3896">April 3, 2017</span></span>

<span data-ttu-id="e5954-3897">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e5954-3897">Version 2.0.2</span></span>

<span data-ttu-id="e5954-3898">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="e5954-3898">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e5954-3899">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e5954-3899">Core</span></span>

* <span data-ttu-id="e5954-3900">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3900">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e5954-3901">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e5954-3901">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e5954-3902">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e5954-3902">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e5954-3903">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e5954-3903">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e5954-3904">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e5954-3904">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e5954-3905">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="e5954-3905">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e5954-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e5954-3906">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e5954-3907">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="e5954-3907">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e5954-3908">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="e5954-3908">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e5954-3909">ACS</span><span class="sxs-lookup"><span data-stu-id="e5954-3909">ACS</span></span>

* <span data-ttu-id="e5954-3910">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e5954-3910">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e5954-3911">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="e5954-3911">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e5954-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e5954-3912">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e5954-3913">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="e5954-3913">Add support for windows clusters.</span></span> <span data-ttu-id="e5954-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e5954-3914">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e5954-3915">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="e5954-3915">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e5954-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e5954-3916">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e5954-3917">AppService</span><span class="sxs-lookup"><span data-stu-id="e5954-3917">AppService</span></span>

* <span data-ttu-id="e5954-3918">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e5954-3918">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e5954-3919">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e5954-3919">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e5954-3920">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e5954-3920">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e5954-3921">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e5954-3921">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e5954-3922">DataLake</span><span class="sxs-lookup"><span data-stu-id="e5954-3922">DataLake</span></span>

* <span data-ttu-id="e5954-3923">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e5954-3923">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e5954-3924">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e5954-3924">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e5954-3925">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="e5954-3925">DocuemntDB</span></span>

* <span data-ttu-id="e5954-3926">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e5954-3926">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e5954-3927">VM</span><span class="sxs-lookup"><span data-stu-id="e5954-3927">VM</span></span>

* <span data-ttu-id="e5954-3928">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e5954-3928">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e5954-3929">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e5954-3929">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e5954-3930">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e5954-3930">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e5954-3931">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e5954-3931">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e5954-3932">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e5954-3932">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e5954-3933">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="e5954-3933">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="e5954-3934">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e5954-3934">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e5954-3935">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="e5954-3935">February 27, 2017</span></span>

<span data-ttu-id="e5954-3936">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e5954-3936">Version 2.0.0</span></span>

<span data-ttu-id="e5954-3937">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="e5954-3937">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e5954-3938">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="e5954-3938">Container Service (acs)</span></span>
- <span data-ttu-id="e5954-3939">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e5954-3939">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e5954-3940">Rede</span><span class="sxs-lookup"><span data-stu-id="e5954-3940">Networking</span></span>
- <span data-ttu-id="e5954-3941">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e5954-3941">Storage</span></span>

<span data-ttu-id="e5954-3942">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e5954-3942">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e5954-3943">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-3943">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e5954-3944">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="e5954-3944">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e5954-3945">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="e5954-3945">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e5954-3946">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="e5954-3946">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e5954-3947">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e5954-3947">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e5954-3948">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e5954-3948">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e5954-3949">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e5954-3949">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e5954-3950">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e5954-3950">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="e5954-3951">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="e5954-3951">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="e5954-3952">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="e5954-3952">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="e5954-3953">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="e5954-3953">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="e5954-3954">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e5954-3954">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="e5954-3955">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="e5954-3955">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="e5954-3956">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="e5954-3956">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="e5954-3957">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="e5954-3957">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="e5954-3958">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e5954-3958">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="e5954-3959">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para se autenticar.</span><span class="sxs-lookup"><span data-stu-id="e5954-3959">`--use-cert-sn-issuer` parameter is not supported when using service principal key to authenticate.</span></span>
-   <span data-ttu-id="e5954-3960">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="e5954-3960">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="e5954-3961">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="e5954-3961">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---
