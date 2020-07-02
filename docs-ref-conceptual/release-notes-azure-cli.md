---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 06/23/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 68ba21af45850bc11b7568860607dc5bcb379b9f
ms.sourcegitcommit: a13a02e99e8eefb91f11e4a40f5fa0d3b5e758e0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "85256313"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="d6d14-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-103">Azure CLI release notes</span></span>

# <a name="current-release-notes"></a>[<span data-ttu-id="d6d14-104">Notas sobre a versão atuais</span><span class="sxs-lookup"><span data-stu-id="d6d14-104">Current release notes</span></span>](#tab/azure-cli)

## <a name="june-23-2020"></a><span data-ttu-id="d6d14-105">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-105">June 23, 2020</span></span>

<span data-ttu-id="d6d14-106">Versão 2.8.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-106">Version 2.8.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-107">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-107">ACR</span></span>

* <span data-ttu-id="d6d14-108">Adicionar suporte para desabilitar roteamento/ponto de extremidade da região</span><span class="sxs-lookup"><span data-stu-id="d6d14-108">Add support for region endpoint disable / routing disable</span></span>
* <span data-ttu-id="d6d14-109">[ALTERAÇÃO DA FALHA] `az acr login --expose-token` não aceita nome de usuário e senha</span><span class="sxs-lookup"><span data-stu-id="d6d14-109">[BREAKING CHANGE] `az acr login --expose-token` does not accept username and password</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-110">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-110">ACS</span></span>

* <span data-ttu-id="d6d14-111">Remover o cluster privado e a API 2019-10-27-preview</span><span class="sxs-lookup"><span data-stu-id="d6d14-111">Remove private cluster and 2019-10-27-preview API</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-112">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-112">AKS</span></span>

* <span data-ttu-id="d6d14-113">Suporte a --yes para az aks upgrade</span><span class="sxs-lookup"><span data-stu-id="d6d14-113">Support --yes for az aks upgrade</span></span>
* <span data-ttu-id="d6d14-114">Reverter "alteração da sku de vm padrão para Standard_D2s_v3 (#13541)"</span><span class="sxs-lookup"><span data-stu-id="d6d14-114">Revert "change default vm sku to Standard_D2s_v3 (#13541)"</span></span>
* <span data-ttu-id="d6d14-115">Adicionar "az aks update --uptime-sla"</span><span class="sxs-lookup"><span data-stu-id="d6d14-115">Add "az aks update --uptime-sla"</span></span>
* <span data-ttu-id="d6d14-116">Corrigir erro de digitação no comando az aks update</span><span class="sxs-lookup"><span data-stu-id="d6d14-116">Fix typo in az aks update command</span></span>
* <span data-ttu-id="d6d14-117">Alteração para dar suporte ao pool de agentes do nó 0 e bloquear a escala manual do pool habilitado para CAS</span><span class="sxs-lookup"><span data-stu-id="d6d14-117">Change to support 0 node agent pool and block manual scale for CAS enabled pool</span></span>
* <span data-ttu-id="d6d14-118">Corrigir erro de digitação em VirtualMachineScaleSets e atualizar referências a versões do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-118">Fix typo on VirtualMachineScaleSets and update references to Kubernetes versions</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-119">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-119">AMS</span></span>

* <span data-ttu-id="d6d14-120">ALTERAR o texto da ajuda do parâmetro "--expiry".</span><span class="sxs-lookup"><span data-stu-id="d6d14-120">CHANGE help text for "--expiry" parameter.</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-121">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-121">AppService</span></span>

* <span data-ttu-id="d6d14-122">`az webapp log deployment show`: mostrar o log de implantação mais recente ou os logs de uma implantação específica se a ID da implantação for especificada</span><span class="sxs-lookup"><span data-stu-id="d6d14-122">`az webapp log deployment show`: Show the latest deployment log, or the deployment logs of a specific deployment if deployment-id is specified</span></span>
* <span data-ttu-id="d6d14-123">`az webapp log deployment list`: lista de logs de implantação disponíveis</span><span class="sxs-lookup"><span data-stu-id="d6d14-123">`az webapp log deployment list`: List of deployment logs available</span></span>
* <span data-ttu-id="d6d14-124">Correção: erro de superfície quando um nome de webapp inválido é fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-124">Fix: Surface error when invalid webapp name provided</span></span>
* <span data-ttu-id="d6d14-125">Correção #13261: az webapp list-runtimes usa a lista estática até que a nova API de Pilhas Disponíveis esteja disponível</span><span class="sxs-lookup"><span data-stu-id="d6d14-125">Fix #13261 az webapp list-runtimes use static list until new Available Stacks API is available</span></span>
* <span data-ttu-id="d6d14-126">`az appservice ase create`: correção na criação do problema #13361</span><span class="sxs-lookup"><span data-stu-id="d6d14-126">`az appservice ase create`: Fix create issue #13361</span></span>
* <span data-ttu-id="d6d14-127">`az appservice ase list-addresses`: correção na alteração do SDK #13140.</span><span class="sxs-lookup"><span data-stu-id="d6d14-127">`az appservice ase list-addresses`: Fix change of SDK #13140.</span></span>
* <span data-ttu-id="d6d14-128">Correção da criação de webapp/slot para Contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-128">Fix webapp/slot creation for Windows Containers</span></span>
* <span data-ttu-id="d6d14-129">`az webapp auth update`: adicionar parâmetro opcional para atualizar a versão do runtime</span><span class="sxs-lookup"><span data-stu-id="d6d14-129">`az webapp auth update`: Add optional parameter to update runtime-version</span></span>
* <span data-ttu-id="d6d14-130">Suporte para listar, excluir, aprovar e rejeitar conexão de ponto de extremidade privado para webapp na CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-130">Support list, delete, approve and reject private endpoint connection for webapp in CLI</span></span>
* <span data-ttu-id="d6d14-131">Correção #13888: adicionar suporte para WebApps Estáticos: comandos get, list, create</span><span class="sxs-lookup"><span data-stu-id="d6d14-131">Fix #13888 : Add support for Static WebApps: get, list, create commands</span></span>
* <span data-ttu-id="d6d14-132">Mensagens de erro aprimoradas para Conexão de Túnel SSH</span><span class="sxs-lookup"><span data-stu-id="d6d14-132">Improved error messages for SSH Tunnel Connection</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-133">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-133">ARM</span></span>

* <span data-ttu-id="d6d14-134">`az tag`: adicionar exemplos para -h</span><span class="sxs-lookup"><span data-stu-id="d6d14-134">`az tag`: Add examples for -h</span></span>
* <span data-ttu-id="d6d14-135">`az deployment group/sub what-if`: adicionar parâmetro --exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="d6d14-135">`az deployment group/sub what-if`: Add --exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="d6d14-136">`az deployment group/sub/mg/tenant create`: adicionar parâmetro --what-if-exclude-change-types/-x.</span><span class="sxs-lookup"><span data-stu-id="d6d14-136">`az deployment group/sub/mg/tenant create`: Add --what-if-exclude-change-types/-x parameter.</span></span>
* <span data-ttu-id="d6d14-137">`az deployment group/sub/mg/tenant validate`: mostrar mensagens de erro em um formato melhor.</span><span class="sxs-lookup"><span data-stu-id="d6d14-137">`az deployment group/sub/mg/tenant validate`: Show error messages in a better format.</span></span>
* <span data-ttu-id="d6d14-138">`az group export`: adicionar novos parâmetros `--skip-resource-name-params` e `--skip-all-params` para dar suporte para ignorar parametrização</span><span class="sxs-lookup"><span data-stu-id="d6d14-138">`az group export`: Add new parameters `--skip-resource-name-params` and `--skip-all-params` to support skip parameterization</span></span>
* <span data-ttu-id="d6d14-139">Adicionar az feature unregister api</span><span class="sxs-lookup"><span data-stu-id="d6d14-139">Add az feature unregister api</span></span>

### <a name="aro"></a><span data-ttu-id="d6d14-140">ARO</span><span class="sxs-lookup"><span data-stu-id="d6d14-140">ARO</span></span>

* <span data-ttu-id="d6d14-141">Adicionar Public e Private aos parâmetros para obter ajuda com a visibilidade de entrada/apiserver</span><span class="sxs-lookup"><span data-stu-id="d6d14-141">Add Public, Private to params for help with ingress/apiserver visibility</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-142">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-142">Batch</span></span>

* <span data-ttu-id="d6d14-143">`az batch account create`: adicionar novo parâmetro `--public-network-access`</span><span class="sxs-lookup"><span data-stu-id="d6d14-143">`az batch account create`: Add new parameter `--public-network-access`</span></span>
* <span data-ttu-id="d6d14-144">`az batch account create`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="d6d14-144">`az batch account create`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="d6d14-145">`az batch account set`: adicionar novo parâmetro `--identity-type`</span><span class="sxs-lookup"><span data-stu-id="d6d14-145">`az batch account set`: Add new parameter `--identity-type`</span></span>
* <span data-ttu-id="d6d14-146">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool usando uma imagem personalizada, a propriedade --image agora pode se referir apenas a uma imagem da Galeria de Imagens Compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-146">[BREAKING CHANGE] az batch pool create: When creating a pool using a custom image, the --image property of can now only refer to a Shared Image Gallery image.</span></span>
* <span data-ttu-id="d6d14-147">[ALTERAÇÃO SIGNIFICATIVA] az batch pool create: ao criar um pool com a opção --json-file e especificar uma networkConfiguration, a propriedade publicIPs foi movida para uma nova propriedade publicIPAddressConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6d14-147">[BREAKING CHANGE] az batch pool create: When creating a pool with --json-file option and specifying a networkConfiguration, the publicIPs property has moved in to a new property publicIPAddressConfiguration.</span></span> <span data-ttu-id="d6d14-148">Essa nova propriedade também dá suporte a uma nova propriedade ipAddressProvisioningType, que especifica como o pool deve alocar os IPs, e a uma propriedade publicIPs, que permite a configuração de uma lista de recursos de PublicIP a serem usados caso ipAddressProvisioningType seja definido como UserManaged</span><span class="sxs-lookup"><span data-stu-id="d6d14-148">This new property also supports a new ipAddressProvisioningType property which specifies how the pool should allocate IP's and a publicIPs property which allows for configuration of a list of PublicIP resources to use in the case ipAddressProvisioningType is set to UserManaged</span></span>
* <span data-ttu-id="d6d14-149">`az network private-link-resource`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="d6d14-149">`az network private-link-resource`: Add support for the Microsoft.Batch batchAccount resource</span></span>
* <span data-ttu-id="d6d14-150">`az network private-endpoint-connection`: adicionar suporte para o recurso Microsoft.Batch batchAccount</span><span class="sxs-lookup"><span data-stu-id="d6d14-150">`az network private-endpoint-connection`: Add support for the Microsoft.Batch batchAccount resource</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-151">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-151">CDN</span></span>

* <span data-ttu-id="d6d14-152">`az cdn custom-domain enable-https`: adicionar suporte para BYOC.</span><span class="sxs-lookup"><span data-stu-id="d6d14-152">`az cdn custom-domain enable-https`: Add BYOC support.</span></span>
* <span data-ttu-id="d6d14-153">`az cdn custom-domain enable-https`: corrigir a habilitação de HTTPS personalizado com certificados gerenciados da CDN para os SKUs Standard_Verizon e Standard_Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6d14-153">`az cdn custom-domain enable-https`: Fix enabling custom HTTPS with CDN managed certificates for Standard_Verizon and Standard_Microsoft SKUs.</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d6d14-154">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-154">Cognitive Services</span></span>

* <span data-ttu-id="d6d14-155">[ALTERAÇÃO DA FALHA] `az cognitiveservices account` agora, há uma estrutura unificada para todos os comandos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-155">[BREAKING CHANGE] `az cognitiveservices account` now have a unified structure for all commands.</span></span>
* <span data-ttu-id="d6d14-156">`az cognitiveservices account identity`: adicionar gerenciamento de identidades para os Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-156">`az cognitiveservices account identity`: Add identity management for Cognitive Services.</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-157">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-157">Compute</span></span>

* <span data-ttu-id="d6d14-158">`az image builder`: atualização da versão da API para 2020-02-14</span><span class="sxs-lookup"><span data-stu-id="d6d14-158">`az image builder`: Upgrade API version to 2020-02-14</span></span>
* <span data-ttu-id="d6d14-159">`az image builder create`: adicionar `--identity` para dar suporte à configuração de identidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-159">`az image builder create`: Add `--identity` to support identity configuration</span></span>
* <span data-ttu-id="d6d14-160">`az image builder customizer add`: suporte para o personalizador de atualização do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-160">`az image builder customizer add`: Support Windows update customizer</span></span>
* <span data-ttu-id="d6d14-161">Novo comando `az image builder cancel`</span><span class="sxs-lookup"><span data-stu-id="d6d14-161">New command `az image builder cancel`</span></span>
* <span data-ttu-id="d6d14-162">Mostrar um aviso quando um usuário implanta um VMSS fixado a uma versão de uma imagem específica em vez da mais recente</span><span class="sxs-lookup"><span data-stu-id="d6d14-162">Show a warning when a user deploys a VMSS pinned to a specific image version rather than latest</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-163">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-163">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-164">`az cosmosdb`: adicionar o comando exists ao banco de dados e aos grupos de contêineres</span><span class="sxs-lookup"><span data-stu-id="d6d14-164">`az cosmosdb`: Add exists command to database and container groups</span></span>
* <span data-ttu-id="d6d14-165">Permitir a criação de coleções fixas</span><span class="sxs-lookup"><span data-stu-id="d6d14-165">Allow creating fixed collections</span></span>

### <a name="eventhub"></a><span data-ttu-id="d6d14-166">EventHub</span><span class="sxs-lookup"><span data-stu-id="d6d14-166">EventHub</span></span>

* <span data-ttu-id="d6d14-167">`az eventhubs namespace create`: adicionar parâmetros de identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="d6d14-167">`az eventhubs namespace create` : Add managed identity parameters</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-168">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-168">Extension</span></span>

* <span data-ttu-id="d6d14-169">Adicionar --version para dar suporte à instalação de uma versão específica</span><span class="sxs-lookup"><span data-stu-id="d6d14-169">Add --version to support to install from a specific version</span></span>
* <span data-ttu-id="d6d14-170">Habilitar as extensões da CLI a incluírem pacotes no namespace 'azure'</span><span class="sxs-lookup"><span data-stu-id="d6d14-170">Enable CLI extensions to include packages in the 'azure' namespace</span></span>

### <a name="iot-hub"></a><span data-ttu-id="d6d14-171">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-171">Iot Hub</span></span>

* <span data-ttu-id="d6d14-172">[ALTERAÇÃO SIGNIFICATIVA] az iot hub job: remover comandos de trabalho preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-172">[BREAKING CHANGE] az iot hub job: Remove deprecated job commands</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-173">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-173">KeyVault</span></span>

* <span data-ttu-id="d6d14-174">`az keyvault key import`: dá suporte à importação de cadeias de caracteres por meio de dois novos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d6d14-174">`az keyvault key import`: Supports importing from strings via two new parameters.</span></span>
* <span data-ttu-id="d6d14-175">Suporte à criptografia e descriptografia de cadeias de caracteres/bytes com chaves armazenadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-175">Support string/bytes encryption and decryption with stored keys</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-176">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-176">Monitor</span></span>

* <span data-ttu-id="d6d14-177">Suporte para não aguardar a criação do cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-177">Support no wait for cluster creation</span></span>
* <span data-ttu-id="d6d14-178">`az monitor log-analytics workspace saved-search`: suporte para novos comandos para a pesquisa salva</span><span class="sxs-lookup"><span data-stu-id="d6d14-178">`az monitor log-analytics workspace saved-search`: Support new commands for saved search</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-179">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-179">Network</span></span>

* <span data-ttu-id="d6d14-180">`az network application-gateway address-pool update`: refinar a mensagem de ajuda e adicionar exemplos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-180">`az network application-gateway address-pool update`: Refine help message and add examples.</span></span>
* <span data-ttu-id="d6d14-181">`az network vnet create`: suporte para o argumento --nsg</span><span class="sxs-lookup"><span data-stu-id="d6d14-181">`az network vnet create`: Support --nsg argument</span></span>
* <span data-ttu-id="d6d14-182">`az network lb address-pool`: suporte para criar o pool de back-end de lb com endereço de back-end.</span><span class="sxs-lookup"><span data-stu-id="d6d14-182">`az network lb address-pool`: Support create lb backend pool with backend address.</span></span>
* <span data-ttu-id="d6d14-183">`az network application-gateway address-pool`: correção para o argumento --add</span><span class="sxs-lookup"><span data-stu-id="d6d14-183">`az network application-gateway address-pool`: Fix for --add argument</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-184">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-184">RBAC</span></span>

* <span data-ttu-id="d6d14-185">`az ad sp create-for-rabc`: suporte para nome com espaço, barra e barra invertida</span><span class="sxs-lookup"><span data-stu-id="d6d14-185">`az ad sp create-for-rabc`: Support name with space, slash and back slash</span></span>
* <span data-ttu-id="d6d14-186">`az ad sp create-for-rbac`: refinar mensagem de erro quando o usuário especifica um escopo inválido</span><span class="sxs-lookup"><span data-stu-id="d6d14-186">`az ad sp create-for-rbac`: Refine error message when user specify an invalid scope</span></span>

### <a name="security"></a><span data-ttu-id="d6d14-187">Segurança</span><span class="sxs-lookup"><span data-stu-id="d6d14-187">Security</span></span>

* <span data-ttu-id="d6d14-188">Adicionar comandos de avaliação de segurança</span><span class="sxs-lookup"><span data-stu-id="d6d14-188">Add security assessment commands</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-189">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-189">SQL</span></span>

* <span data-ttu-id="d6d14-190">`az sql db ltr-policy/ltr-backup`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="d6d14-190">`az sql db ltr-policy/ltr-backup`: update/show long term retention policy, show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-191">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-191">Storage</span></span>

* <span data-ttu-id="d6d14-192">Corrigir problema de autenticação para dar suporte a get token para --subscription</span><span class="sxs-lookup"><span data-stu-id="d6d14-192">Fix authentication issue to support get token for --subscription</span></span>
* <span data-ttu-id="d6d14-193">`az storage remove`: correção do problema #13459 para gerar exceção para a falha da operação</span><span class="sxs-lookup"><span data-stu-id="d6d14-193">`az storage remove`: Fix issue #13459 to raise exception for operation failure</span></span>
* <span data-ttu-id="d6d14-194">Correção dos problemas #13012, #13632 e #13657 para remover argumentos não utilizados para comandos relacionados à geração de SAS</span><span class="sxs-lookup"><span data-stu-id="d6d14-194">Fix issues #13012, #13632 and #13657 to remove unused arguments for generate-sas related commands</span></span>
* <span data-ttu-id="d6d14-195">`az storage logging update`: adicionar verificação da versão de log</span><span class="sxs-lookup"><span data-stu-id="d6d14-195">`az storage logging update`: Add check for logging version</span></span>
* <span data-ttu-id="d6d14-196">`az storage blob show`: adicionar mais propriedades para o blob com o SDK da faixa 2</span><span class="sxs-lookup"><span data-stu-id="d6d14-196">`az storage blob show`: Add more properties for blob with track 2 SDK</span></span>
* <span data-ttu-id="d6d14-197">Correção #13708: refinar a mensagem de aviso para a credencial</span><span class="sxs-lookup"><span data-stu-id="d6d14-197">Fix #13708: Refine warning message for credential</span></span>
* <span data-ttu-id="d6d14-198">`az storage share-rm create/update`: adicionar suporte para protocolo NFS e squash raiz</span><span class="sxs-lookup"><span data-stu-id="d6d14-198">`az storage share-rm create/update`: Add NFS protocol and root squash support</span></span>
* <span data-ttu-id="d6d14-199">`az storage account create`: adicionar suporte para criptografia dupla</span><span class="sxs-lookup"><span data-stu-id="d6d14-199">`az storage account create`: Add support for double encryption</span></span>
* <span data-ttu-id="d6d14-200">[ALTERAÇÃO DA FALHA] `az storage blob/container/file/share/table/queue generate-sas`: tornar --expiry e --permissions obrigatórios</span><span class="sxs-lookup"><span data-stu-id="d6d14-200">[BREAKING CHANGE] `az storage blob/container/file/share/table/queue generate-sas`: make --expiry and --permissions required</span></span>
* <span data-ttu-id="d6d14-201">`az storage blob set-tier`: migrar para a Faixa 2 para dar suporte à definição da prioridade de reidratação</span><span class="sxs-lookup"><span data-stu-id="d6d14-201">`az storage blob set-tier`: Migrate to Track 2 to support setting rehydrate priority</span></span>

## <a name="june-02-2020"></a><span data-ttu-id="d6d14-202">02 de Junho de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-202">June 02, 2020</span></span>

<span data-ttu-id="d6d14-203">Versão 2.7.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-203">Version 2.7.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-204">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-204">ACR</span></span>

* <span data-ttu-id="d6d14-205">Correção de um erro de digitação em uma mensagem de erro de criação de token</span><span class="sxs-lookup"><span data-stu-id="d6d14-205">Fix a typo in an error message of token creation</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-206">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-206">AKS</span></span>

* <span data-ttu-id="d6d14-207">Alteração da sku de vm padrão para Standard_D2s_v3</span><span class="sxs-lookup"><span data-stu-id="d6d14-207">Change default vm sku to Standard_D2s_v3</span></span>
* <span data-ttu-id="d6d14-208">Correção da criação de atribuição de função para sub-rede personalizada MSI cluster Plus</span><span class="sxs-lookup"><span data-stu-id="d6d14-208">Fix creating role assignment for MSI clsuter plus custom subnet</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-209">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-209">AppService</span></span>

* <span data-ttu-id="d6d14-210">A correção #12739 az appservice list-locations retorna alguns locais inválidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-210">Fix #12739 az appservice list-locations returns some invalid locations</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-211">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-211">ARM</span></span>

* <span data-ttu-id="d6d14-212">`az deployment`: Correção do problema #13159 de mensagem incorreta do JSON após a remoção de comentários e a compactação</span><span class="sxs-lookup"><span data-stu-id="d6d14-212">`az deployment`: Fix issue #13159 of incorrect message of JSON after removing comments and compressing</span></span>
* <span data-ttu-id="d6d14-213">`az resource tag`: Correção do problema #13255 de marcação de recursos com o tipo de recurso `Microsoft.ContainerRegistry/registries/webhooks`</span><span class="sxs-lookup"><span data-stu-id="d6d14-213">`az resource tag`: Fix issue #13255 of tagging resources with resource type `Microsoft.ContainerRegistry/registries/webhooks`</span></span>
* <span data-ttu-id="d6d14-214">Melhoria dos exemplos do módulo de recursos</span><span class="sxs-lookup"><span data-stu-id="d6d14-214">Improve the examples for the resource module</span></span>

### <a name="aro"></a><span data-ttu-id="d6d14-215">ARO</span><span class="sxs-lookup"><span data-stu-id="d6d14-215">ARO</span></span>

* <span data-ttu-id="d6d14-216">Alteração do CLIError para corrigir o sinalizador para --worker-vm-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="d6d14-216">Change CLIError to correct flag for --worker-vm-disk-size-gb</span></span>

### <a name="eventhub"></a><span data-ttu-id="d6d14-217">EventHub</span><span class="sxs-lookup"><span data-stu-id="d6d14-217">EventHub</span></span>

* <span data-ttu-id="d6d14-218">Correção do problema #12406 Argumento --capture-interval não atualiza o "intervalInSeconds"</span><span class="sxs-lookup"><span data-stu-id="d6d14-218">Fix for issue #12406 Argument --capture-interval does not update the "intervalInSeconds"</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-219">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-219">HDInsight</span></span>

* <span data-ttu-id="d6d14-220">Alteração de get_json_object para shell_safe_json_parse</span><span class="sxs-lookup"><span data-stu-id="d6d14-220">Change get_json_object to shell_safe_json_parse</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-221">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-221">Monitor</span></span>

* <span data-ttu-id="d6d14-222">`az monitor metrics alert`: ajuste de várias mensagens de ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-222">`az monitor metrics alert`: refine several help messages</span></span>
* <span data-ttu-id="d6d14-223">`az monitor diagnostic-settings create`: suporte ao argumento --export-to-resource-specific</span><span class="sxs-lookup"><span data-stu-id="d6d14-223">`az monitor diagnostic-settings create`: support --export-to-resource-specific argument</span></span>
* <span data-ttu-id="d6d14-224">Suporte para recuperar o workspace de LA</span><span class="sxs-lookup"><span data-stu-id="d6d14-224">Support LA workspace recover</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-225">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-225">Network</span></span>

* <span data-ttu-id="d6d14-226">`az network dns zone`: suporte – caractere</span><span class="sxs-lookup"><span data-stu-id="d6d14-226">`az network dns zone`: support - character</span></span>
* <span data-ttu-id="d6d14-227">`az network vpn-connection ipsec-policy`: alteração do --sa-lifetime e do --sa-max-size para valores maiores no exemplo</span><span class="sxs-lookup"><span data-stu-id="d6d14-227">`az network vpn-connection ipsec-policy`: change the --sa-lifetime and --sa-max-size to larger values in example</span></span>
* <span data-ttu-id="d6d14-228">Aumento da rede para 2020-04-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-228">Bump network to 2020-04-01</span></span>
* <span data-ttu-id="d6d14-229">`az network private-endpoint-connection`: suporte à grade de eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-229">`az network private-endpoint-connection`: support event grid</span></span>
* <span data-ttu-id="d6d14-230">`az network express-route list-route-tables`: correção do bug que faz não ser possível listar rotas como tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-230">`az network express-route list-route-tables`: fix bug that cannot list routes as table</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-231">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-231">Packaging</span></span>

* <span data-ttu-id="d6d14-232">Adição do Pacote Focal do Ubuntu</span><span class="sxs-lookup"><span data-stu-id="d6d14-232">Add Ubuntu Focal Package</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-233">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-233">RBAC</span></span>

* <span data-ttu-id="d6d14-234">`az ad sp credential reset`: modificar a geração de credenciais para evitar caracteres especiais problemáticos</span><span class="sxs-lookup"><span data-stu-id="d6d14-234">`az ad sp credential reset`: modify credential generation to avoid troublesome special characters</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-235">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-235">Redis</span></span>

* <span data-ttu-id="d6d14-236">Correção #13529: alteração da documentação do parâmetro enable_non_ssl_port</span><span class="sxs-lookup"><span data-stu-id="d6d14-236">Fix #13529: Change documentation of parameter enable_non_ssl_port</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-237">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-237">Storage</span></span>

* <span data-ttu-id="d6d14-238">`az storage copy`: adição do parâmetro `--follow-symlinks` para dar suporte ao symlinks</span><span class="sxs-lookup"><span data-stu-id="d6d14-238">`az storage copy`: Add parameter `--follow-symlinks` to support symlinks</span></span>
* <span data-ttu-id="d6d14-239">Habilitar contexto local para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-239">Enable local context for storage account</span></span>
* <span data-ttu-id="d6d14-240">`az storage logging`: Correção do problema #11969 para ajustar a mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-240">`az storage logging`: Fix issue #11969 to refine error message</span></span>

## <a name="may-19-2020"></a><span data-ttu-id="d6d14-241">19 de maio de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-241">May 19, 2020</span></span>

<span data-ttu-id="d6d14-242">Versão 2.6.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-242">Version 2.6.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-243">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-243">ACR</span></span>

* <span data-ttu-id="d6d14-244">Adiciona tempo limite padrão de 5 minutos para solicitações ao ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-244">Add default timeout of 5 minutes for any requests to ACR</span></span>
* <span data-ttu-id="d6d14-245">Suporte para desabilitar o acesso à redes públicas</span><span class="sxs-lookup"><span data-stu-id="d6d14-245">Support disable public network access</span></span>
* <span data-ttu-id="d6d14-246">`az acr token create`: expõe o argumento --days</span><span class="sxs-lookup"><span data-stu-id="d6d14-246">`az acr token create`: expose --days argument</span></span>
* <span data-ttu-id="d6d14-247">`az acr import`: aceita valores do argumento --source que contêm logon no nome do servidor por meio da correção final do cliente</span><span class="sxs-lookup"><span data-stu-id="d6d14-247">`az acr import`: accept --source argument values which contain login in server name through client end correction</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-248">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-248">ACS</span></span>

* <span data-ttu-id="d6d14-249">Correção de bug: remover limpeza de campos para campos que não existem mais</span><span class="sxs-lookup"><span data-stu-id="d6d14-249">Bug fix: remove fields cleanup for fields that no longer exist</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-250">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-250">AKS</span></span>

* <span data-ttu-id="d6d14-251">Atualiza o tempo de atividade do contexto de ajuda de comando do SLA</span><span class="sxs-lookup"><span data-stu-id="d6d14-251">Update uptime-sla command help context</span></span>
* <span data-ttu-id="d6d14-252">Remove a verificação do intervalo para a atualização da contagem de minutos do dimensionador automático</span><span class="sxs-lookup"><span data-stu-id="d6d14-252">Remove range check for updating min count for autoscaler</span></span>
* <span data-ttu-id="d6d14-253">Corrige o problema que fazia com que a CLI falhasse quando o usuário especificava apenas a senha do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-253">Fix that cli doe not fail when user only specifies Windows password</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-254">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-254">AMS</span></span>

* <span data-ttu-id="d6d14-255">`az ams transform create`: Adiciona a capacidade de criar uma transformação com um FaceDetector predefinido</span><span class="sxs-lookup"><span data-stu-id="d6d14-255">`az ams transform create`: Add ability to create a transform with a FaceDetector preset</span></span>
* <span data-ttu-id="d6d14-256">`az ams content-key-policy create`: Adiciona a capacidade de criar uma política de chave de conteúdo do FairPlay com uma configuração de aluguel offline</span><span class="sxs-lookup"><span data-stu-id="d6d14-256">`az ams content-key-policy create` : Add ability to create a FairPlay content key policy with an offline rental configuration</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-257">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-257">AppConfig</span></span>

* <span data-ttu-id="d6d14-258">Correção de bug para valores de chave da lista com campos</span><span class="sxs-lookup"><span data-stu-id="d6d14-258">Bug fix for list key values with fields</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-259">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-259">AppService</span></span>

* <span data-ttu-id="d6d14-260">`az functionapp create`: AzureWebJobsDashboard será definido somente se AppInsights estiver desabilitado</span><span class="sxs-lookup"><span data-stu-id="d6d14-260">`az functionapp create`: AzureWebJobsDashboard will only be set if AppInsights is disabled</span></span>
* <span data-ttu-id="d6d14-261">Correção #10664 – Integração VNet – Problema de Verificação de Localização e Correção #13257-AZ Web App falha quando o RG precisar ser criado</span><span class="sxs-lookup"><span data-stu-id="d6d14-261">Fix #10664- VNet Integration - Location Check Issue & fix #13257- az webapp up failing when RG needs to be created</span></span>
* <span data-ttu-id="d6d14-262">`az webapp|functionapp config ssl import`: Pesquisa o cofre de chaves em grupos de recursos na assinatura e aprimora a ajuda e os exemplos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-262">`az webapp|functionapp config ssl import`: Lookup key vault across resources groups in subscription and improve help and examples.</span></span>
* <span data-ttu-id="d6d14-263">Integra o contexto local para o serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-263">Onboard local context for app service</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-264">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-264">ARM</span></span>

* <span data-ttu-id="d6d14-265">`az deployment`: Corrige o problema que faz com que o templateLink não seja retornado ao implantar ou validar o template-uri</span><span class="sxs-lookup"><span data-stu-id="d6d14-265">`az deployment`: Fix the problem that the templateLink will not be returned when deploying or validating template-uri</span></span>
* <span data-ttu-id="d6d14-266">`az deployment`: Corrige o problema que faz com que implantação/validação não dê suporte ao caractere codificado especialmente</span><span class="sxs-lookup"><span data-stu-id="d6d14-266">`az deployment`: Fix the problem that deployment/validate does not support specially encoded character</span></span>
* <span data-ttu-id="d6d14-267">`az deployment sub/group what-if`: Corrige o alinhamento de matriz e o tratamento de erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-267">`az deployment sub/group what-if`: Fix array alignment and error handling</span></span>
* <span data-ttu-id="d6d14-268">`az deployment operation`: Modifica as informações preteridas</span><span class="sxs-lookup"><span data-stu-id="d6d14-268">`az deployment operation`: Modify the deprecate information</span></span>

### <a name="aro"></a><span data-ttu-id="d6d14-269">ARO</span><span class="sxs-lookup"><span data-stu-id="d6d14-269">ARO</span></span>

* <span data-ttu-id="d6d14-270">Adiciona exemplos para az aro create, list, list-credentials, show, delete</span><span class="sxs-lookup"><span data-stu-id="d6d14-270">Add examples to az aro create, list, list-credentials, show, delete</span></span>
* <span data-ttu-id="d6d14-271">Adiciona a função generate_random_id</span><span class="sxs-lookup"><span data-stu-id="d6d14-271">Add generate_random_id function</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-272">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-272">Backup</span></span>

* <span data-ttu-id="d6d14-273">Permite FriendlyName ao habilitar proteção para o comando AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="d6d14-273">Allow FriendlyName in enable protection for AzureFileShare command</span></span>
* <span data-ttu-id="d6d14-274">Correção do comando restore-disks da IaasVM</span><span class="sxs-lookup"><span data-stu-id="d6d14-274">Fix in IaasVM restore-disks Command</span></span>
* <span data-ttu-id="d6d14-275">Adiciona o BackupManagementType "MAB" ao comando item list</span><span class="sxs-lookup"><span data-stu-id="d6d14-275">Add "MAB" BackupManagementType to item list command</span></span>
* <span data-ttu-id="d6d14-276">Adiciona suporte para a repetição de tentativas de atualização da política para itens com falha.</span><span class="sxs-lookup"><span data-stu-id="d6d14-276">Add support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="d6d14-277">Adiciona a funcionalidade de Retomada de Proteção para as Máquinas Virtuais do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-277">Add Resume Protection functionality for Azure Virtual Machine</span></span>
* <span data-ttu-id="d6d14-278">Adiciona suporte para especificar o ResourceGroup para armazenar instantRP durante a Criação ou Modificação de Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-278">Add support to specify ResourceGroup for storing instantRP during Create or Modify Policy</span></span>

### <a name="ci"></a><span data-ttu-id="d6d14-279">CI</span><span class="sxs-lookup"><span data-stu-id="d6d14-279">CI</span></span>

* <span data-ttu-id="d6d14-280">Suporte para flake8 3.8.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-280">Support flake8 3.8.0</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-281">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-281">Compute</span></span>

* <span data-ttu-id="d6d14-282">Novo comando az vm auto-shutdown</span><span class="sxs-lookup"><span data-stu-id="d6d14-282">New command az vm auto-shutdown</span></span>
* <span data-ttu-id="d6d14-283">`az vm list-skus`: Atualização do comportamento --zone, retorna SKUs de todos os tipos agora</span><span class="sxs-lookup"><span data-stu-id="d6d14-283">`az vm list-skus`: Update --zone behavior, return all type skus now</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-284">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-284">Core</span></span>

* <span data-ttu-id="d6d14-285">Atualiza o status de ativado/desativado do contexto local para o nível de usuário global</span><span class="sxs-lookup"><span data-stu-id="d6d14-285">Update local context on/off status to global user level</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-286">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-286">Extension</span></span>

* <span data-ttu-id="d6d14-287">`az extension add`: Adiciona --system para habilitar a instalação de extensões em um caminho do sistema</span><span class="sxs-lookup"><span data-stu-id="d6d14-287">`az extension add`: Add --system to enable installing extensions in a system path</span></span>
* <span data-ttu-id="d6d14-288">Suporte para .egg-info para armazenar metadados de extensão de tipo de roda</span><span class="sxs-lookup"><span data-stu-id="d6d14-288">Support .egg-info to store wheel type extension metadata</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-289">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-289">IoT</span></span>

* <span data-ttu-id="d6d14-290">`az iot`: Atualiza a mensagem de reconhecimento de extensão da primeira execução do módulo de comando IoT para a ID precisa e moderna não preterida `azure-iot`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-290">`az iot`: Update the IoT command module first run extension awareness message to the accurate, non-deprecated modern Id `azure-iot`.</span></span>

### <a name="iot-hub"></a><span data-ttu-id="d6d14-291">Hub IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-291">IoT Hub</span></span>

* <span data-ttu-id="d6d14-292">Suporte para comandos de isolamento de rede e API 2020-03-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-292">Support for 2020-03-01 API and Network Isolation commands</span></span>

### <a name="netappfiles"></a><span data-ttu-id="d6d14-293">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="d6d14-293">NetAppFiles</span></span>

* <span data-ttu-id="d6d14-294">`az volume create`: Adiciona snapshot-id como um parâmetro para criar volume – isso permitirá que os usuários criem um volume por meio de um instantâneo existente.</span><span class="sxs-lookup"><span data-stu-id="d6d14-294">`az volume create`: Adds snapshot-id as a parameter to create volume this will allow users to create a volume from existing snapshot.</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-295">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-295">Network</span></span>

* <span data-ttu-id="d6d14-296">Corrige o valor TTL alterado não destinado ao DNS add-record</span><span class="sxs-lookup"><span data-stu-id="d6d14-296">Fix ttl value changed unintended for dns add-record</span></span>
* <span data-ttu-id="d6d14-297">`az network public-ip create`: Informa os clientes sobre futuras alterações da falha</span><span class="sxs-lookup"><span data-stu-id="d6d14-297">`az network public-ip create`: Inform customers of a coming breaking change</span></span>
* <span data-ttu-id="d6d14-298">Suporte para comandos genéricos para cenários de link privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-298">Support generic commands for private link scenario</span></span>
* <span data-ttu-id="d6d14-299">`az network private-endpoint-connection`: Suporte para tipos mysql, postgre e mariadb</span><span class="sxs-lookup"><span data-stu-id="d6d14-299">`az network private-endpoint-connection`: Support mysql, postgre and mariadb types</span></span>
* <span data-ttu-id="d6d14-300">`az network private-endpoint-connection`: Suporte para tipos cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d6d14-300">`az network private-endpoint-connection`: Support cosmosdb types</span></span>
* <span data-ttu-id="d6d14-301">`az network private-endpoint`: pretere --group-ids e redireciona para --group-id</span><span class="sxs-lookup"><span data-stu-id="d6d14-301">`az network private-endpoint`: deprecate --group-ids and redirect to --group-id</span></span>

### <a name="output"></a><span data-ttu-id="d6d14-302">Saída</span><span class="sxs-lookup"><span data-stu-id="d6d14-302">Output</span></span>

* <span data-ttu-id="d6d14-303">Mostra instruções de atualização em localizar, comentários e --help</span><span class="sxs-lookup"><span data-stu-id="d6d14-303">Show update instruction in find, feedback and --help</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-304">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-304">Packaging</span></span>

* <span data-ttu-id="d6d14-305">Cria pacotes MSI/Homebrew com dependências resolvidas de requirements.txt</span><span class="sxs-lookup"><span data-stu-id="d6d14-305">Build MSI/Homebrew packages with dependecies resolved from requirements.txt</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-306">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-306">RBAC</span></span>

* <span data-ttu-id="d6d14-307">`az ad sp credential reset`: corrige a geração de credenciais fracas</span><span class="sxs-lookup"><span data-stu-id="d6d14-307">`az ad sp credential reset`: fix weak credential generation</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-308">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-308">Storage</span></span>

* <span data-ttu-id="d6d14-309">`az storage account file-service-properties update/show`: Adiciona suporte a propriedades de arquivo para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-309">`az storage account file-service-properties update/show`: Add File Properties Support for Storage Account</span></span>
* <span data-ttu-id="d6d14-310">`az storage container create`: Correção #13373 ao adicionar o validador para acesso público</span><span class="sxs-lookup"><span data-stu-id="d6d14-310">`az storage container create`: Fix #13373 by adding validator for public access</span></span>
* <span data-ttu-id="d6d14-311">Adiciona suporte a ADLS Gen2 track2</span><span class="sxs-lookup"><span data-stu-id="d6d14-311">Add ADLS Gen2 track2 support</span></span>
* <span data-ttu-id="d6d14-312">`az storage blob sync`: Dar suporte à `--connection-string`</span><span class="sxs-lookup"><span data-stu-id="d6d14-312">`az storage blob sync`: Support `--connection-string`</span></span>
* <span data-ttu-id="d6d14-313">`az storage blob sync`: Corrige a mensagem de erro incorreta quando azcopy não consegue encontrar o local de instalação</span><span class="sxs-lookup"><span data-stu-id="d6d14-313">`az storage blob sync`: Fix the incorrect error message when azcopy cannot find the installation location</span></span>

## <a name="april-30-2020"></a><span data-ttu-id="d6d14-314">30 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-314">April 30, 2020</span></span>

<span data-ttu-id="d6d14-315">Versão 2.5.1</span><span class="sxs-lookup"><span data-stu-id="d6d14-315">Version 2.5.1</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-316">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-316">ACR</span></span>

* <span data-ttu-id="d6d14-317">`az acr check-health`: correção de "DOCKER_PULL_ERROR" no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-317">`az acr check-health`: Fix "DOCKER_PULL_ERROR" on Windows</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-318">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-318">Compute</span></span>

* <span data-ttu-id="d6d14-319">`az vm list-ip-addresses`: Tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="d6d14-319">`az vm list-ip-addresses`: Error handling</span></span>
* <span data-ttu-id="d6d14-320">Correção de um bug de criação de VM caso endpoint_vm_image_alias_doc não estivesse definido no perfil de nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-320">Fix a bug of vm create if endpoint_vm_image_alias_doc is not set in cloud profile</span></span>
* <span data-ttu-id="d6d14-321">`az vmss create`: adição de --os-disk-size-gb</span><span class="sxs-lookup"><span data-stu-id="d6d14-321">`az vmss create`: Add --os-disk-size-gb</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-322">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-322">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-323">`az cosmosdb create/update`: adição de suporte a --enable-public-network</span><span class="sxs-lookup"><span data-stu-id="d6d14-323">`az cosmosdb create/update`: add --enable-public-network support</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-324">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-324">Extension</span></span>

* <span data-ttu-id="d6d14-325">Correção do carregamento de metadados errados para a extensão de tipo roda</span><span class="sxs-lookup"><span data-stu-id="d6d14-325">Fix loading wrong metadata for wheel type extension</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-326">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-326">Packaging</span></span>

* <span data-ttu-id="d6d14-327">Adição de script az para Git Bash/Cygwin no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-327">Add az script for Git Bash/Cygwin on Windows</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-328">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-328">SQL</span></span>

* <span data-ttu-id="d6d14-329">`az sql instance-pool`: adição de grupo de comando de pools de instância</span><span class="sxs-lookup"><span data-stu-id="d6d14-329">`az sql instance-pool`: Add instance pools command group</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-330">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-330">Storage</span></span>

* <span data-ttu-id="d6d14-331">Atualização do pacote azure-multiapi-storage para 0.3.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-331">Upgrade package azure-multiapi-storage to 0.3.0</span></span>
* <span data-ttu-id="d6d14-332">Dá suporte ao GZRS para a criação e atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-332">Support GZRS for storage account creation and update</span></span>
* <span data-ttu-id="d6d14-333">`az storage account failover`: adição de suporte para failover da conta de armazenamento de GRS/GZRS</span><span class="sxs-lookup"><span data-stu-id="d6d14-333">`az storage account failover`: Add support for grs/gzrs storage account failover</span></span>
* <span data-ttu-id="d6d14-334">`az storage blob upload`: adição do parâmetro --encryption-scope para dar suporte à especificação da informação do escopo da criptografia</span><span class="sxs-lookup"><span data-stu-id="d6d14-334">`az storage blob upload`: Add --encryption-scope parameter to support specifying encryption scope information</span></span>

## <a name="april-28-2020"></a><span data-ttu-id="d6d14-335">28 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-335">April 28, 2020</span></span>

<span data-ttu-id="d6d14-336">Versão 2.5.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-336">Version 2.5.0</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-337">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-337">ACS</span></span>

* <span data-ttu-id="d6d14-338">[ALTERAÇÃO SIGNIFICATIVA] az openshift create: remove o parâmetro --vnet-peer.</span><span class="sxs-lookup"><span data-stu-id="d6d14-338">[BREAKING CHANGE] az openshift create: remove --vnet-peer parameter.</span></span>
* <span data-ttu-id="d6d14-339">`az openshift create`: adição de sinalizadores para dar suporte a clusters privados.</span><span class="sxs-lookup"><span data-stu-id="d6d14-339">`az openshift create`: add flags to support private cluster.</span></span>
* <span data-ttu-id="d6d14-340">`az openshift`: atualização para a versão `2019-10-27-preview` da API.</span><span class="sxs-lookup"><span data-stu-id="d6d14-340">`az openshift`: upgrade to `2019-10-27-preview` API version.</span></span>
* <span data-ttu-id="d6d14-341">`az openshift`: adição do comando `update`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-341">`az openshift`: add `update` command.</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-342">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-342">AKS</span></span>

* <span data-ttu-id="d6d14-343">`az aks create`: adição do suporte para Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-343">`az aks create`: Add support for Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-344">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-344">AppService</span></span>

* <span data-ttu-id="d6d14-345">`az webapp deployment source config-zip`: remoção da suspensão após request.get()</span><span class="sxs-lookup"><span data-stu-id="d6d14-345">`az webapp deployment source config-zip`: remove sleep after request.get()</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-346">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-346">ARM</span></span>

* <span data-ttu-id="d6d14-347">Adição de comandos What-If de implantação de modelo</span><span class="sxs-lookup"><span data-stu-id="d6d14-347">Add template deployment What-If commands</span></span>

### <a name="aro"></a><span data-ttu-id="d6d14-348">ARO</span><span class="sxs-lookup"><span data-stu-id="d6d14-348">ARO</span></span>

* <span data-ttu-id="d6d14-349">`az aro`: correção da saída da tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-349">`az aro`: Fix table output</span></span>

### <a name="ci"></a><span data-ttu-id="d6d14-350">CI</span><span class="sxs-lookup"><span data-stu-id="d6d14-350">CI</span></span>

* <span data-ttu-id="d6d14-351">Integração do pytest e preterição do nose para o teste de automação</span><span class="sxs-lookup"><span data-stu-id="d6d14-351">Onboard pytest and deprecate nose for Automation Test</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-352">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-352">Compute</span></span>

* <span data-ttu-id="d6d14-353">`az vmss disk detach`: correção do problema de NoneType do disco de dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-353">`az vmss disk detach`: fix data disk NoneType issue</span></span>
* <span data-ttu-id="d6d14-354">`az vm availability-set list`: suporte à exibição da lista de VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-354">`az vm availability-set list`: Support showing VM list</span></span>
* <span data-ttu-id="d6d14-355">`az vm list-skus`: correção do problema de exibição do formato de tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-355">`az vm list-skus`: Fix display problem of table format</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-356">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-356">KeyVault</span></span>

* <span data-ttu-id="d6d14-357">Adição de novo parâmetro `--enable-rbac-authorization` durante a criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-357">Add new parameter `--enable-rbac-authorization` during creating or updating</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-358">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-358">Monitor</span></span>

* <span data-ttu-id="d6d14-359">Suporte aos recursos de CMK do cluster de LA</span><span class="sxs-lookup"><span data-stu-id="d6d14-359">Support LA cluster CMK features</span></span>
* <span data-ttu-id="d6d14-360">`az monitor log-analytics workspace linked-storage`: dá suporte aos recursos BYOS</span><span class="sxs-lookup"><span data-stu-id="d6d14-360">`az monitor log-analytics workspace linked-storage`: supports BYOS features</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-361">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-361">Network</span></span>

* <span data-ttu-id="d6d14-362">`az network security-partner`: suporte para provedor de segurança de parceiros</span><span class="sxs-lookup"><span data-stu-id="d6d14-362">`az network security-partner`: support security partner provider</span></span>

### <a name="privatedns"></a><span data-ttu-id="d6d14-363">Privatedns</span><span class="sxs-lookup"><span data-stu-id="d6d14-363">Privatedns</span></span>

* <span data-ttu-id="d6d14-364">Adição do recurso na zona DNS privada para importar o arquivo da zona de exportação</span><span class="sxs-lookup"><span data-stu-id="d6d14-364">Add feature in private DNS zone to import export zone file</span></span>

## <a name="april-21-2020"></a><span data-ttu-id="d6d14-365">21 de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-365">April 21, 2020</span></span>

<span data-ttu-id="d6d14-366">Versão 2.4.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-366">Version 2.4.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-367">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-367">ACR</span></span>

* <span data-ttu-id="d6d14-368">`az acr run --cmd`: desabilitar a substituição do diretório de trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-368">`az acr run --cmd`: disable working directory override</span></span>
* <span data-ttu-id="d6d14-369">Suporte ao ponto de extremidade dos dados dedicados</span><span class="sxs-lookup"><span data-stu-id="d6d14-369">Support dedicated data endpoint</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-370">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-370">AKS</span></span>

* <span data-ttu-id="d6d14-371">`az aks list -o table` deve mostrar privateFqdn como fqdn para clusters privados</span><span class="sxs-lookup"><span data-stu-id="d6d14-371">`az aks list -o table` should show privateFqdn as fqdn for private clusters</span></span>
* <span data-ttu-id="d6d14-372">Adicionar --uptime-sla</span><span class="sxs-lookup"><span data-stu-id="d6d14-372">Add --uptime-sla</span></span>
* <span data-ttu-id="d6d14-373">Atualizar pacote containerservice</span><span class="sxs-lookup"><span data-stu-id="d6d14-373">Update containerservice package</span></span>
* <span data-ttu-id="d6d14-374">Adicionar suporte ao IP público do nó</span><span class="sxs-lookup"><span data-stu-id="d6d14-374">Add node public IP support</span></span>
* <span data-ttu-id="d6d14-375">Corrigir erros de digitação no comando de ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-375">Fix typo in the help command</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-376">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-376">AppConfig</span></span>

* <span data-ttu-id="d6d14-377">Resolver referência do cofre de chaves para os comandos kv list e export</span><span class="sxs-lookup"><span data-stu-id="d6d14-377">Resolve key vault reference for kv list and export commands</span></span>
* <span data-ttu-id="d6d14-378">Correção de bug para valores de chave da lista</span><span class="sxs-lookup"><span data-stu-id="d6d14-378">Bug fix for list key values</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-379">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-379">AppService</span></span>

* <span data-ttu-id="d6d14-380">`az functionapp create`: mudou a maneira como o linuxFxVersion estava sendo definido para os aplicativos de funções dotnet linux.</span><span class="sxs-lookup"><span data-stu-id="d6d14-380">`az functionapp create`: Changed the way linuxFxVersion was being set for dotnet linux function apps.</span></span> <span data-ttu-id="d6d14-381">Isso deve corrigir um bug que estava impedindo a criação de aplicativos de consumo em dotnet linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-381">This should fix a bug that was preventing dotnet linux consumption apps from being created</span></span>
* <span data-ttu-id="d6d14-382">[ALTERAÇÃO DA FALHA] `az webapp create`: correção para manter o AppSettings existente com o az webapp create</span><span class="sxs-lookup"><span data-stu-id="d6d14-382">[BREAKING CHANGE] `az webapp create`: fix to keep existing AppSettings with az webapp create</span></span>
* <span data-ttu-id="d6d14-383">[ALTERAÇÃO DA FALHA] `az webapp up`: correção para criar o RG para o comando az webapp up ao usar o sinalizador -g</span><span class="sxs-lookup"><span data-stu-id="d6d14-383">[BREAKING CHANGE] `az webapp up`: fix to create RG for az webapp up command when using -g flag</span></span>
* <span data-ttu-id="d6d14-384">[ALTERAÇÃO DA FALHA] `az webapp config`: correção para mostrar valores de saída não JSON com o az webapp config connection-string list</span><span class="sxs-lookup"><span data-stu-id="d6d14-384">[BREAKING CHANGE] `az webapp config`: fix to show values for non-JSON output with az webapp config connection-string list</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-385">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-385">ARM</span></span>

* <span data-ttu-id="d6d14-386">`az deployment create/validate`: adicionar o parâmetro `--no-prompt` para dar suporte à ação de ignorar o prompt de parâmetros ausentes para o modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="d6d14-386">`az deployment create/validate`: Add parameter `--no-prompt` to support skipping the prompt of missing parameters for ARM template</span></span>
* <span data-ttu-id="d6d14-387">`az deployment group/mg/sub/tenant validate`: dar suporte aos comentários no arquivo de parâmetro de implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-387">`az deployment group/mg/sub/tenant validate`: Support comments in deployment parameter file</span></span>
* <span data-ttu-id="d6d14-388">`az deployment`: remover `is_preview` para o parâmetro `--handle-extended-json-format`</span><span class="sxs-lookup"><span data-stu-id="d6d14-388">`az deployment`: Remove `is_preview` for parameter `--handle-extended-json-format`</span></span>
* <span data-ttu-id="d6d14-389">`az deployment group/mg/sub/tenant cancel`: dar suporte para cancelar a implantação do modelo do Resource Manager</span><span class="sxs-lookup"><span data-stu-id="d6d14-389">`az deployment group/mg/sub/tenant cancel`: Support cancel deployment for ARM template</span></span>
* <span data-ttu-id="d6d14-390">`az deployment group/mg/sub/tenant validate`: melhorar a mensagem de erro quando a verificação de implantação falhar</span><span class="sxs-lookup"><span data-stu-id="d6d14-390">`az deployment group/mg/sub/tenant validate`: Improve the error message when deployment verification fails</span></span>
* <span data-ttu-id="d6d14-391">`az deployment-scripts`: adicionar novos comandos para DeploymentScripts</span><span class="sxs-lookup"><span data-stu-id="d6d14-391">`az deployment-scripts`: Add new commands for DeploymentScripts</span></span>
* <span data-ttu-id="d6d14-392">`az resource tag`: adicionar o parâmetro `--is-incremental` para dar suporte à adição de marcas ao recurso de maneira incremental</span><span class="sxs-lookup"><span data-stu-id="d6d14-392">`az resource tag`: Add parameter `--is-incremental` to support adding tags to resource incrementally</span></span>

### <a name="aro"></a><span data-ttu-id="d6d14-393">ARO</span><span class="sxs-lookup"><span data-stu-id="d6d14-393">ARO</span></span>

* <span data-ttu-id="d6d14-394">`az aro`:  adicionar módulo de comando aro do Azure RedHat OpenShift V4</span><span class="sxs-lookup"><span data-stu-id="d6d14-394">`az aro`:  Add Azure RedHat OpenShift V4 aro command module</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-395">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-395">Batch</span></span>

* <span data-ttu-id="d6d14-396">Atualizar a API do Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-396">Update Batch API</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-397">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-397">Compute</span></span>

* <span data-ttu-id="d6d14-398">`az sig image-version create`: adicionar o tipo da conta de armazenamento Premium_LRS</span><span class="sxs-lookup"><span data-stu-id="d6d14-398">`az sig image-version create`: Add storage account type Premium_LRS</span></span>
* <span data-ttu-id="d6d14-399">`az vmss update`: corrigir problema de atualização de notificação de término</span><span class="sxs-lookup"><span data-stu-id="d6d14-399">`az vmss update`: Fix terminate notification update issue</span></span>
* <span data-ttu-id="d6d14-400">`az vm/vmss create`: adicionar suporte para a versão de imagem especializada</span><span class="sxs-lookup"><span data-stu-id="d6d14-400">`az vm/vmss create`: Add support for specialized image version</span></span>
* <span data-ttu-id="d6d14-401">Versão da API SIG 2019-12-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-401">SIG API Version 2019-12-01</span></span>
* <span data-ttu-id="d6d14-402">`az sig image-version create`: Adicionar --target-region-encryption</span><span class="sxs-lookup"><span data-stu-id="d6d14-402">`az sig image-version create`: Add --target-region-encryption</span></span>
* <span data-ttu-id="d6d14-403">Os testes de correção falham quando executados em série, pois o nome do keyvault está duplicado no cache global na memória</span><span class="sxs-lookup"><span data-stu-id="d6d14-403">Fix tests fail when running in serial due to keyvault name is duplicated in global in-momery cache</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-404">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-404">CosmosDB</span></span>

* <span data-ttu-id="d6d14-405">Dar suporte à `az cosmosdb private-link-resource/private-endpoint-connection`</span><span class="sxs-lookup"><span data-stu-id="d6d14-405">Support `az cosmosdb private-link-resource/private-endpoint-connection`</span></span>

### <a name="iot-central"></a><span data-ttu-id="d6d14-406">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-406">IoT Central</span></span>

* <span data-ttu-id="d6d14-407">Preterir `az iotcentral`</span><span class="sxs-lookup"><span data-stu-id="d6d14-407">Deprecate `az iotcentral`</span></span>
* <span data-ttu-id="d6d14-408">Adicionar o módulo de comando `az iot central`</span><span class="sxs-lookup"><span data-stu-id="d6d14-408">Add `az iot central` command module</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-409">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-409">Monitor</span></span>

* <span data-ttu-id="d6d14-410">Dar suporte ao cenário de link privado para monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-410">Support private link scenario for monitor</span></span>
* <span data-ttu-id="d6d14-411">Corrigir a maneira incorreta de simulação em test_monitor_general_operations.py</span><span class="sxs-lookup"><span data-stu-id="d6d14-411">Fix wrong mocking way in test_monitor_general_operations.py</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-412">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-412">Network</span></span>

* <span data-ttu-id="d6d14-413">Preterir o sku para o comando de atualização de ip público</span><span class="sxs-lookup"><span data-stu-id="d6d14-413">Deprecate sku for public ip update command</span></span>
* <span data-ttu-id="d6d14-414">`az network private-endpoint`: dar suporte ao grupo de zona dns privada</span><span class="sxs-lookup"><span data-stu-id="d6d14-414">`az network private-endpoint`: Support private dns zone group</span></span>
* <span data-ttu-id="d6d14-415">Habilitar o recurso de contexto local para o parâmetro vnet/sub-rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-415">Enable local context feature for vnet/subnet parameter</span></span>
* <span data-ttu-id="d6d14-416">Corrigir o exemplo de uso incorreto em test_nw_flow_log_delete</span><span class="sxs-lookup"><span data-stu-id="d6d14-416">Fix wrong usage example in test_nw_flow_log_delete</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-417">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-417">Packaging</span></span>

* <span data-ttu-id="d6d14-418">Descartar o suporte para o pacote Ubuntu/Disco</span><span class="sxs-lookup"><span data-stu-id="d6d14-418">Drop support for Ubuntu/Disco package</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-419">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-419">RBAC</span></span>

* <span data-ttu-id="d6d14-420">`az ad app create/update`: dar suporte a --optional-claims como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6d14-420">`az ad app create/update`: support --optional-claims as a parameter</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-421">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-421">RDBMS</span></span>

* <span data-ttu-id="d6d14-422">Adicionar comandos do administrador do Azure Active Directory para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-422">Add Azure active directory administrator commands for PostgreSQL and MySQL</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d6d14-423">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-423">Service Fabric</span></span>

* <span data-ttu-id="d6d14-424">Correção nº 12891: `az sf application update --application-parameters` remove parâmetros antigos que não estão na solicitação</span><span class="sxs-lookup"><span data-stu-id="d6d14-424">Fix #12891: `az sf application update --application-parameters` removes old parameters that are not in the request</span></span>
* <span data-ttu-id="d6d14-425">Correção nº 12470 az sf create cluster, corrigir bugs na atualização de durabilidade e confiabilidade e encontrar vmss corretamente por meio do código, dado um nome de tipo de nó</span><span class="sxs-lookup"><span data-stu-id="d6d14-425">Fix #12470 az sf create cluster, fix bugs in update durability and reliability and find vmss correctly through the code given a node type name</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-426">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-426">SQL</span></span>

* <span data-ttu-id="d6d14-427">Adicionar `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span><span class="sxs-lookup"><span data-stu-id="d6d14-427">Add `az sql mi op list`, `az sql mi op get`, `az sql mi op cancel`</span></span>
* <span data-ttu-id="d6d14-428">`az sql midb`: atualizar/mostrar política de retenção de longo prazo, mostrar/excluir backups de retenção de longo prazo, restaurar backup de retenção de longo prazo</span><span class="sxs-lookup"><span data-stu-id="d6d14-428">`az sql midb`: update/show long term retention policy,  show/delete long term retention backups, restore long term retention backup</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-429">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-429">Storage</span></span>

* <span data-ttu-id="d6d14-430">Atualizar azure-mgmt-storage para 9.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-430">Upgrade azure-mgmt-storage to 9.0.0</span></span>
* <span data-ttu-id="d6d14-431">`az storage logging off`: dar suporte à desativação do registro em log de uma conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-431">`az storage logging off`: Support turning off logging for a storage account</span></span>
* <span data-ttu-id="d6d14-432">`az storage account update`: habilitar rotação automática de chave para CMK</span><span class="sxs-lookup"><span data-stu-id="d6d14-432">`az storage account update`: Enable key auto-rotated for CMK</span></span>
* <span data-ttu-id="d6d14-433">`az storage account encryption-scope create/update/list/show`: adicionar suporte para personalizar o escopo de criptografia</span><span class="sxs-lookup"><span data-stu-id="d6d14-433">`az storage account encryption-scope create/update/list/show`: Add support to customize encryption scope</span></span>
* <span data-ttu-id="d6d14-434">`az storage container create`: adicionar --default-encryption-scope e --deny-encryption-scope-override a fim de definir o escopo de criptografia para o nível de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-434">`az storage container create`: Add --default-encryption-scope and --deny-encryption-scope-override to set encryption scope for container level</span></span>

### <a name="survey"></a><span data-ttu-id="d6d14-435">Pesquisa</span><span class="sxs-lookup"><span data-stu-id="d6d14-435">Survey</span></span>

* <span data-ttu-id="d6d14-436">Adicionar opção para desligar o link de pesquisa</span><span class="sxs-lookup"><span data-stu-id="d6d14-436">Add switch to turn off survey link</span></span>

## <a name="april-01-2020"></a><span data-ttu-id="d6d14-437">1º de abril de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-437">April 01, 2020</span></span>

<span data-ttu-id="d6d14-438">Versão 2.3.1</span><span class="sxs-lookup"><span data-stu-id="d6d14-438">Version 2.3.1</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-439">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-439">ACR</span></span>

* <span data-ttu-id="d6d14-440">Corrigir a versão errada do azure-mgmt-containerregistry para Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-440">Fix wrong version of azure-mgmt-containerregistry for Linux</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-441">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-441">Profile</span></span>

* <span data-ttu-id="d6d14-442">az login: Corrigir falha de logon com perfis de nuvem diferentes de `latest`</span><span class="sxs-lookup"><span data-stu-id="d6d14-442">az login: Fix login failure with cloud profiles other than `latest`</span></span>

## <a name="march-31-2020"></a><span data-ttu-id="d6d14-443">31 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-443">March 31, 2020</span></span>

<span data-ttu-id="d6d14-444">Versão 2.3.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-444">Version 2.3.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-445">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-445">ACR</span></span>

* <span data-ttu-id="d6d14-446">'az acr task update': exceção de ponteiro nulo</span><span class="sxs-lookup"><span data-stu-id="d6d14-446">'az acr task update': null pointer exception</span></span>
* <span data-ttu-id="d6d14-447">`az acr import`: Modificar a mensagem de ajuda e de erro para esclarecer o uso de --source e --registry</span><span class="sxs-lookup"><span data-stu-id="d6d14-447">`az acr import`: Modify help and error message to clarify the usage of --source and --registry</span></span>
* <span data-ttu-id="d6d14-448">Adicionar um validador para o argumento 'registry_name'</span><span class="sxs-lookup"><span data-stu-id="d6d14-448">Add a validator for argument 'registry_name'</span></span>
* <span data-ttu-id="d6d14-449">`az acr login`: remover o sinalizador de visualização em '--expose-token'</span><span class="sxs-lookup"><span data-stu-id="d6d14-449">`az acr login`:Remove the preview flag on '--expose-token'</span></span>
* <span data-ttu-id="d6d14-450">O parâmetro de branch 'az acr task create/update' de [ALTERAÇÃO SIGNIFICATIVA] foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-450">[BREAKING CHANGE] 'az acr task create/update' Branch parameter is removed</span></span>
* <span data-ttu-id="d6d14-451">O cliente 'az acr task update' agora pode atualizar o contexto, o token do git e/ou os gatilhos individualmente</span><span class="sxs-lookup"><span data-stu-id="d6d14-451">'az acr task update' Customer now can update context, git-token, and or triggers individually</span></span>
* <span data-ttu-id="d6d14-452">'az acr agentpool': novo recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-452">'az acr agentpool': new feature</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-453">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-453">AKS</span></span>

* <span data-ttu-id="d6d14-454">Corrigir apiServerAccessProfile ao atualizar --api-server-authorized-ip-ranges</span><span class="sxs-lookup"><span data-stu-id="d6d14-454">Fix apiServerAccessProfile when updating --api-server-authorized-ip-ranges</span></span>
* <span data-ttu-id="d6d14-455">aks update: Substituir IPs de saída por valores de entrada ao atualizar</span><span class="sxs-lookup"><span data-stu-id="d6d14-455">aks update: Override outbound IPs with input values when update</span></span>
* <span data-ttu-id="d6d14-456">Não criar SPN para clusters MSI e dar suporte à anexação de ACR a clusters MSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-456">Do not create SPN for MSI clusters and support attach acr to MSI clusters</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-457">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-457">AMS</span></span>

* <span data-ttu-id="d6d14-458">Correção nº. 12469: a adição da política de chave de conteúdo Fairplay falha devido a problemas com o parâmetro 'ask'</span><span class="sxs-lookup"><span data-stu-id="d6d14-458">Fix #12469: adding Fairplay content-key-policy fails due to problems with 'ask' parameter</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-459">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-459">AppConfig</span></span>

* <span data-ttu-id="d6d14-460">Adicionar --skip-keyvault a kv export</span><span class="sxs-lookup"><span data-stu-id="d6d14-460">Add --skip-keyvault for kv export</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-461">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-461">AppService</span></span>

* <span data-ttu-id="d6d14-462">Correção nº 12509: remover a marca para az webapp up por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-462">Fix #12509: Remove the tag to az webapp up by default</span></span>
* <span data-ttu-id="d6d14-463">az functionapp create: o menu de ajuda de --runtime-version foi atualizado e um aviso foi adicionado quando o usuário especifica --runtime-version para dotnet</span><span class="sxs-lookup"><span data-stu-id="d6d14-463">az functionapp create: Updated --runtime-version help menu and added warning when user specifies --runtime-version for dotnet</span></span>
* <span data-ttu-id="d6d14-464">az functionapp create: atualizado o modo como o javaVersion estava sendo definido para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-464">az functionapp create: Updated the way javaVersion was being set for Windows function apps</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-465">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-465">ARM</span></span>

* <span data-ttu-id="d6d14-466">az deployment create/validate: usar --handle-extended-json-format por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-466">az deployment create/validate: Use --handle-extended-json-format by default</span></span>
* <span data-ttu-id="d6d14-467">az lock create: adicionar exemplos de criação de subrecurso na documentação da ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-467">az lock create: Add examples of creating subresource in the help documentation</span></span>
* <span data-ttu-id="d6d14-468">az deployment {group/mg/sub/tenant} list: dar suporte à filtragem de provisioningState</span><span class="sxs-lookup"><span data-stu-id="d6d14-468">az deployment {group/mg/sub/tenant} list: Support provisioningState filtering</span></span>
* <span data-ttu-id="d6d14-469">az deployment: corrigir o bug de análise para o comentário no último argumento</span><span class="sxs-lookup"><span data-stu-id="d6d14-469">az deployment: Fix the parse bug for comment under the last argument</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-470">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-470">Backup</span></span>

* <span data-ttu-id="d6d14-471">Adicionadas várias funcionalidades de restauração de arquivo</span><span class="sxs-lookup"><span data-stu-id="d6d14-471">Added multiple files restore capabilities</span></span>
* <span data-ttu-id="d6d14-472">Adicionado suporte para backup somente de discos do SO</span><span class="sxs-lookup"><span data-stu-id="d6d14-472">Added support for Backing up OS Disks only</span></span>
* <span data-ttu-id="d6d14-473">Adicionado o parâmetro restore-as-unmanaged-disk para especificar a restauração não gerenciada</span><span class="sxs-lookup"><span data-stu-id="d6d14-473">Added restore-as-unmanaged-disk parameter to specify unmanaged restore</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-474">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-474">Compute</span></span>

* <span data-ttu-id="d6d14-475">az vm create: adicionar opção NONE de --nsg-rule</span><span class="sxs-lookup"><span data-stu-id="d6d14-475">az vm create: Add NONE option of --nsg-rule</span></span>
* <span data-ttu-id="d6d14-476">az vmss create/update: remover a marca de visualização de reparos automáticos do vmss</span><span class="sxs-lookup"><span data-stu-id="d6d14-476">az vmss create/update: remove vmss automatic repairs preview tag</span></span>
* <span data-ttu-id="d6d14-477">az vm update: dar suporte a --workspace</span><span class="sxs-lookup"><span data-stu-id="d6d14-477">az vm update: Support --workspace</span></span>
* <span data-ttu-id="d6d14-478">Corrigir um bug no código de inicialização de VirtualMachineScaleSetExtension</span><span class="sxs-lookup"><span data-stu-id="d6d14-478">Fix a bug in VirtualMachineScaleSetExtension initialization code</span></span>
* <span data-ttu-id="d6d14-479">Atualizar a versão do VMAccessAgent para 2.4</span><span class="sxs-lookup"><span data-stu-id="d6d14-479">Upgrade VMAccessAgent version to 2.4</span></span>
* <span data-ttu-id="d6d14-480">az vmss set-orchestration-service-state: dar suporte para o estado de definição do serviço de orquestração do vmss</span><span class="sxs-lookup"><span data-stu-id="d6d14-480">az vmss set-orchestration-service-state: support vmss set orchestration service state</span></span>
* <span data-ttu-id="d6d14-481">Atualizar a API do disco para a versão 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-481">Upgrade disk API version to 2019-11-01</span></span>
* <span data-ttu-id="d6d14-482">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span><span class="sxs-lookup"><span data-stu-id="d6d14-482">az disk create: add --disk-iops-read-only, --disk-mbps-read-only, --max-shares, --image-reference, --image-reference-lun, --gallery-image-reference, --gallery-image-reference-lun</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-483">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-483">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-484">Corrigir a ausência da opção --type para redirecionamentos de preterimento</span><span class="sxs-lookup"><span data-stu-id="d6d14-484">Fix missing --type option for deprecation redirections</span></span>

### <a name="docker"></a><span data-ttu-id="d6d14-485">Docker</span><span class="sxs-lookup"><span data-stu-id="d6d14-485">Docker</span></span>

* <span data-ttu-id="d6d14-486">Atualizar para Alpine 3.11 e Python 3.6.10</span><span class="sxs-lookup"><span data-stu-id="d6d14-486">Update to Alpine 3.11 and Python 3.6.10</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-487">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-487">Extension</span></span>

* <span data-ttu-id="d6d14-488">Permitir carregar extensões no caminho do sistema por meio de pacotes</span><span class="sxs-lookup"><span data-stu-id="d6d14-488">Allow to load extensions in the system path via packages</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-489">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-489">HDInsight</span></span>

* <span data-ttu-id="d6d14-490">(az hdinsight create:) dar suporte à especificação da versão de TLS mínima pelos clientes usando o parâmetro `--minimal-tls-version`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-490">(az hdinsight create:) Support customers specify minimal supported tls version by using parameter `--minimal-tls-version`.</span></span> <span data-ttu-id="d6d14-491">O valor permitido é 1.0,1.1,1.2</span><span class="sxs-lookup"><span data-stu-id="d6d14-491">The allowed value is 1.0,1.1,1.2</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-492">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-492">IoT</span></span>

* <span data-ttu-id="d6d14-493">Adicionar codeowner</span><span class="sxs-lookup"><span data-stu-id="d6d14-493">Add codeowner</span></span>
* <span data-ttu-id="d6d14-494">az iot hub create : alterar o SKU padrão de F1 para S1</span><span class="sxs-lookup"><span data-stu-id="d6d14-494">az iot hub create : Change default sku to S1 from F1</span></span>
* <span data-ttu-id="d6d14-495">iot hub: dar suporte a IotHub no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-495">iot hub: Support IotHub in the profile of 2019-03-01-hybrid</span></span>

### <a name="iotcentral"></a><span data-ttu-id="d6d14-496">IoT Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-496">IoTCentral</span></span>

* <span data-ttu-id="d6d14-497">Atualizar detalhes do erro, atualizar modelo de aplicativo padrão e a mensagem de aviso</span><span class="sxs-lookup"><span data-stu-id="d6d14-497">Update error details, update default application template and prompt message</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-498">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-498">KeyVault</span></span>

* <span data-ttu-id="d6d14-499">Suporte para backup/restauração de certificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-499">Support certificate backup/restore</span></span>
* <span data-ttu-id="d6d14-500">keyvault create/update: Suporte a --retention-days</span><span class="sxs-lookup"><span data-stu-id="d6d14-500">keyvault create/update: Support --retention-days</span></span>
* <span data-ttu-id="d6d14-501">Não exibir mais chaves/segredos gerenciados durante a listagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-501">No longer display managed keys/secrets while listing</span></span>
* <span data-ttu-id="d6d14-502">az keyvault create: suporte a `--network-acls`, `--network-acls-ips` e `--network-acls-vnets` para especificar regras de rede ao criar o cofre</span><span class="sxs-lookup"><span data-stu-id="d6d14-502">az keyvault create: support `--network-acls`, `--network-acls-ips` and `--network-acls-vnets` for specifying network rules while creating vault</span></span>

### <a name="lock"></a><span data-ttu-id="d6d14-503">Bloqueio</span><span class="sxs-lookup"><span data-stu-id="d6d14-503">Lock</span></span>

* <span data-ttu-id="d6d14-504">az lock delete fix bug: az lock delete não funciona no Microsoft.DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-504">az lock delete fix bug: az lock delete does not work on Microsoft.DocumentDB</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-505">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-505">Monitor</span></span>

* <span data-ttu-id="d6d14-506">az monitor clone: suporte a regras de métrica de clone de um recurso para outro</span><span class="sxs-lookup"><span data-stu-id="d6d14-506">az monitor clone: support clone metric rules from one resource to another</span></span>
* <span data-ttu-id="d6d14-507">Corrigir IcM179210086: não é possível criar um alerta de métrica personalizado para a métrica de Application Insights</span><span class="sxs-lookup"><span data-stu-id="d6d14-507">Fix IcM179210086: unable to create custom metric alert for their Application Insights metric</span></span>

### <a name="netappfiles"></a><span data-ttu-id="d6d14-508">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="d6d14-508">NetAppFiles</span></span>

* <span data-ttu-id="d6d14-509">az volume create: permitir volumes de proteção de dados adicionando operações de replicação: approve, suspend, resume, status, remove</span><span class="sxs-lookup"><span data-stu-id="d6d14-509">az volume create: Allow data protection volumes adding replication operations: approve, suspend, resume, status, remove</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-510">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-510">Network</span></span>

* <span data-ttu-id="d6d14-511">az network application-gateway waf-policy managed-rule rule-set add: dar suporte a Microsoft_BotManagerRuleSet</span><span class="sxs-lookup"><span data-stu-id="d6d14-511">az network application-gateway waf-policy managed-rule rule-set add: support Microsoft_BotManagerRuleSet</span></span>
* <span data-ttu-id="d6d14-512">network watcher flow-log show: corrigir informações erradas em preterimento</span><span class="sxs-lookup"><span data-stu-id="d6d14-512">network watcher flow-log show: fix wrong deprecating info</span></span>
* <span data-ttu-id="d6d14-513">dar suporte a nomes de host no ouvinte do gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-513">support host names in application gateway listener</span></span>
* <span data-ttu-id="d6d14-514">az network nat gateway: dar suporte para criar um recurso vazio sem IP público nem prefixo de IP público</span><span class="sxs-lookup"><span data-stu-id="d6d14-514">az network nat gateway: support create empty resource without public ip or public ip prefix</span></span>
* <span data-ttu-id="d6d14-515">Dar suporte à geração de gateway de VPN</span><span class="sxs-lookup"><span data-stu-id="d6d14-515">Support vpn gateway generation</span></span>
* <span data-ttu-id="d6d14-516">Dar suporte a `--if-none-match` em `az network dns record-set {} add-record`</span><span class="sxs-lookup"><span data-stu-id="d6d14-516">Support `--if-none-match` in `az network dns record-set {} add-record`</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-517">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-517">Packaging</span></span>

* <span data-ttu-id="d6d14-518">Remover o suporte ao Python 3.5</span><span class="sxs-lookup"><span data-stu-id="d6d14-518">Drop support for python 3.5</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-519">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-519">Profile</span></span>

* <span data-ttu-id="d6d14-520">az login: Mostrar aviso para erro de MFA</span><span class="sxs-lookup"><span data-stu-id="d6d14-520">az login: Show warning for MFA error</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-521">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-521">RDBMS</span></span>

* <span data-ttu-id="d6d14-522">Adicionar comandos de gerenciamento de chaves de criptografia de dados do servidor para PostgreSQL e MySQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-522">Add server data encryption key management commands for PostgreSQL and MySQL</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="d6d14-523">10 de março de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-523">March 10, 2020</span></span>

<span data-ttu-id="d6d14-524">Versão 2.2.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-524">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-525">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-525">ACR</span></span>

* <span data-ttu-id="d6d14-526">Correção: `az acr login` gerava erro incorretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-526">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="d6d14-527">Adicionou o novo comando `az acr helm install-cli`</span><span class="sxs-lookup"><span data-stu-id="d6d14-527">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="d6d14-528">Adicionou link privado e suporte do CMK</span><span class="sxs-lookup"><span data-stu-id="d6d14-528">Add private link and CMK support</span></span>
* <span data-ttu-id="d6d14-529">Adicionou o comando 'private-link-resource list'</span><span class="sxs-lookup"><span data-stu-id="d6d14-529">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-530">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-530">AKS</span></span>

* <span data-ttu-id="d6d14-531">correção da busca do AKS no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d6d14-531">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="d6d14-532">az aks: correção dos erros de complemento de monitoramento e de agentpool NoneType</span><span class="sxs-lookup"><span data-stu-id="d6d14-532">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="d6d14-533">Adicionou --nodepool-tags ao pool de nós ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-533">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="d6d14-534">Adicionou --tags ao adicionar ou atualizar um pool de nós para o cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-534">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="d6d14-535">AKS create: adicionou `--enable-private-cluster`</span><span class="sxs-lookup"><span data-stu-id="d6d14-535">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="d6d14-536">Adicionou --nodepool-labels ao criar o cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-536">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="d6d14-537">Adicionou --labels ao adicionar um novo pool de nós ao cluster do Kubernetes do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-537">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="d6d14-538">Adicionou / ausente na URL do painel</span><span class="sxs-lookup"><span data-stu-id="d6d14-538">add missing / in the dashboard url</span></span>
* <span data-ttu-id="d6d14-539">Suporte para criar clusters do AKS habilitando identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="d6d14-539">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="d6d14-540">az aks: validou o plug-in de rede como "Azure" ou "Kubenet"</span><span class="sxs-lookup"><span data-stu-id="d6d14-540">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="d6d14-541">az aks: adicionou suporte da chave da sessão do AAD</span><span class="sxs-lookup"><span data-stu-id="d6d14-541">az aks: Add aad session key support</span></span>
* <span data-ttu-id="d6d14-542">[ALTERAÇÃO SIGNIFICATIVA] AZ AKS: suporte para alterações de MSI para GF e BF para omsagent (Monitoramento de contêiner) (#1)</span><span class="sxs-lookup"><span data-stu-id="d6d14-542">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="d6d14-543">az aks use-dev-spaces: adicionou a opção de tipo de ponto de extremidade ao comando use-dev-spaces para personalizar o ponto de extremidade criado em um controlador Azure Dev Spaces</span><span class="sxs-lookup"><span data-stu-id="d6d14-543">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-544">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-544">AppConfig</span></span>

* <span data-ttu-id="d6d14-545">Desbloqueou usando "KV set" para adicionar o recurso e a referência do keyvault...</span><span class="sxs-lookup"><span data-stu-id="d6d14-545">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-546">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-546">AppService</span></span>

* <span data-ttu-id="d6d14-547">az webapp create: correção do problema ao executar o comando com --runtime</span><span class="sxs-lookup"><span data-stu-id="d6d14-547">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="d6d14-548">az functionapp deployment source config-zip: adicionou uma mensagem de erro se o grupo de recursos ou o nome da função forem inválidos/não existirem</span><span class="sxs-lookup"><span data-stu-id="d6d14-548">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="d6d14-549">functionapp create: correção da mensagem de aviso que aparece com `functionapp create` hoje, que cita um sinalizador de `--functions_version`, mas usa erroneamente `_` em vez de `-` no nome do sinalizador</span><span class="sxs-lookup"><span data-stu-id="d6d14-549">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="d6d14-550">az functionapp create: atualizou o modo como linuxFxVersion e o nome da imagem de contêiner eram definidos para aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-550">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="d6d14-551">az functionapp deployment source config-zip: correção de um problema causado pelas configurações do aplicativo que alterava a condição de corrida durante a implantação do zip, provocando erros 5xx durante a implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-551">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="d6d14-552">Correção #5720946: AZ WebApp backup falha ao definir o nome</span><span class="sxs-lookup"><span data-stu-id="d6d14-552">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-553">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-553">ARM</span></span>

* <span data-ttu-id="d6d14-554">az resource: aprimorou os exemplos do módulo de recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-554">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="d6d14-555">az policy assignment list: suporte à listagem de atribuições de política no escopo do Grupo de Gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-555">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="d6d14-556">Adicionou `az deployment group` e `az deployment operation group` para a implantação de modelos nos grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-556">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="d6d14-557">Esta é uma duplicata de `az group deployment` e `az group deployment operation`</span><span class="sxs-lookup"><span data-stu-id="d6d14-557">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="d6d14-558">Adicionou `az deployment sub` e `az deployment operation sub` para a implantação de modelos no escopo da assinatura.</span><span class="sxs-lookup"><span data-stu-id="d6d14-558">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="d6d14-559">Esta é uma duplicata de `az deployment` e `az deployment operation`</span><span class="sxs-lookup"><span data-stu-id="d6d14-559">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="d6d14-560">Adicionou `az deployment mg` e `az deployment operation mg` para implantação de modelos nos grupos de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-560">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="d6d14-561">Adicionou `az deployment tenant` e `az deployment operation tenant` para implantação de modelos no escopo do locatário.</span><span class="sxs-lookup"><span data-stu-id="d6d14-561">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="d6d14-562">az policy assignment create: adicionou descrição ao parâmetro `--location`</span><span class="sxs-lookup"><span data-stu-id="d6d14-562">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="d6d14-563">az group deployment create: adicionou o parâmetro `--aux-tenants` para dar suporte a locatários cruzados</span><span class="sxs-lookup"><span data-stu-id="d6d14-563">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-564">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-564">CDN</span></span>

* <span data-ttu-id="d6d14-565">Adicionou comandos do WAF da CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-565">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-566">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-566">Compute</span></span>

* <span data-ttu-id="d6d14-567">az sig image-version: adicionar --data-snapshot-luns</span><span class="sxs-lookup"><span data-stu-id="d6d14-567">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="d6d14-568">AZ PPG show: adicionou --outlocation-status para habilitar a busca do status de colocalização de todos os recursos no grupo de posicionamento por proximidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-568">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="d6d14-569">az vmss create/update: suporte a reparos automáticos</span><span class="sxs-lookup"><span data-stu-id="d6d14-569">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="d6d14-570">[ALTERAÇÃO SIGNIFICATIVA] modelo de imagem AZ: renomear modelo para builder</span><span class="sxs-lookup"><span data-stu-id="d6d14-570">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="d6d14-571">AZ Image Builder Create: adicionou --Image-template</span><span class="sxs-lookup"><span data-stu-id="d6d14-571">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-572">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-572">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-573">Adicionou procedimento armazenado do SQL, UDF e disparar cmdlets</span><span class="sxs-lookup"><span data-stu-id="d6d14-573">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="d6d14-574">az cosmosdb create: adicionou --key-uri para dar suporte à adição de informações de criptografia do cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="d6d14-574">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-575">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-575">KeyVault</span></span>

* <span data-ttu-id="d6d14-576">keyvault create: habilitou a exclusão reversível por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-576">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-577">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-577">Monitor</span></span>

* <span data-ttu-id="d6d14-578">az monitor metrics alert create: suporte a `~` em `--condition`</span><span class="sxs-lookup"><span data-stu-id="d6d14-578">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-579">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-579">Network</span></span>

* <span data-ttu-id="d6d14-580">az network application-gateway rewrite-rule create: suporte à configuração de URL</span><span class="sxs-lookup"><span data-stu-id="d6d14-580">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="d6d14-581">az network dns zone import: --zone-name não diferenciará maiúsculas de minúsculas no futuro</span><span class="sxs-lookup"><span data-stu-id="d6d14-581">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="d6d14-582">az network private-endpoint/private-link-service: removeu rótulo de visualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-582">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="d6d14-583">az network bastion: suporte a bastions</span><span class="sxs-lookup"><span data-stu-id="d6d14-583">az network bastion: support bastion</span></span>
* <span data-ttu-id="d6d14-584">az network vnet list-available-ips: dar suporte à lista de IPs disponíveis em uma vnet</span><span class="sxs-lookup"><span data-stu-id="d6d14-584">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="d6d14-585">az network watcher flow-log create/list/delete/update: adicionou novos comandos para gerenciar o log de fluxo do Inspetor e expor o --local para identificá-lo explicitamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-585">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="d6d14-586">az network watcher flow-log configure: preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-586">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="d6d14-587">az network watcher flow-log show: dá suporte a --location e --name para obter o resultado formatado por ARM, saída formatada antiga preterida</span><span class="sxs-lookup"><span data-stu-id="d6d14-587">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="d6d14-588">Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-588">Policy</span></span>

* <span data-ttu-id="d6d14-589">az policy assignment create: correção do bug que gerou automaticamente o nome da atribuição de política, que excede o limite</span><span class="sxs-lookup"><span data-stu-id="d6d14-589">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-590">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-590">RBAC</span></span>

* <span data-ttu-id="d6d14-591">az ad group show: correção do valor --group, que é tratado como um problema de regex</span><span class="sxs-lookup"><span data-stu-id="d6d14-591">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-592">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-592">RDBMS</span></span>

* <span data-ttu-id="d6d14-593">Trocou a versão do zure-mgmt-rdbms SDK para 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-593">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="d6d14-594">az postgres private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="d6d14-594">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="d6d14-595">az postgres private-link-resource: gerenciou recursos de link privado do Postgres</span><span class="sxs-lookup"><span data-stu-id="d6d14-595">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="d6d14-596">az mysql private-endpoint-connection: gerenciar conexões de ponto de extremidade privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-596">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="d6d14-597">az mysql private-link-resource: gerenciou recursos de link privado do MySQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-597">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="d6d14-598">az mariadb private-endpoint-connection: gerenciou conexões de ponto de extremidade privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-598">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="d6d14-599">az mariadb private-link-resource: gerenciou recursos de link privado do MariaDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-599">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="d6d14-600">Atualizando testes de ponto de extremidade privado do RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-600">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-601">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-601">SQL</span></span>

* <span data-ttu-id="d6d14-602">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span><span class="sxs-lookup"><span data-stu-id="d6d14-602">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="d6d14-603">(sql server create:) adicionou o sinalizador ' habilitar '/' desabilitar ' opcional public-network-access ao SQL Server create</span><span class="sxs-lookup"><span data-stu-id="d6d14-603">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="d6d14-604">(sql server update:) fez algumas alterações voltadas para o cliente</span><span class="sxs-lookup"><span data-stu-id="d6d14-604">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="d6d14-605">adicionou a propriedade minimal_tls_version para o banco de BD de MI e SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-605">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-606">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-606">Storage</span></span>

* <span data-ttu-id="d6d14-607">az storage blob delete-batch: sinalizador `--dryrun` de comportamento inadequado</span><span class="sxs-lookup"><span data-stu-id="d6d14-607">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="d6d14-608">az storage account network-rule add (correção de bug): a operação de adição deve ser idempotente</span><span class="sxs-lookup"><span data-stu-id="d6d14-608">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="d6d14-609">az storage account create/update: Adicionou suporte de preferência de roteamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-609">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="d6d14-610">Atualizou a versão do azure-mgmt-storage para 8.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-610">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="d6d14-611">az storage container immutability create: adicionou o parâmetro --allow-protected-append-write</span><span class="sxs-lookup"><span data-stu-id="d6d14-611">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="d6d14-612">az storage account private-link-resource list: Adicionou suporte para lista de recursos de link privado para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-612">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="d6d14-613">az storage account private-endpoint-connection approve/reject/show/delete: Suporte para gerenciar conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-613">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="d6d14-614">az storage account blob-service-properties update: adicionou --enable-restore-policy e --restore-days</span><span class="sxs-lookup"><span data-stu-id="d6d14-614">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="d6d14-615">az storage blob restore: adicionou suporte para restaurar intervalos de blob</span><span class="sxs-lookup"><span data-stu-id="d6d14-615">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="d6d14-616">18 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-616">February 18, 2020</span></span>

<span data-ttu-id="d6d14-617">Versão 2.1.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-617">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-618">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-618">ACR</span></span>

* <span data-ttu-id="d6d14-619">Adicionar um novo argumento `--expose-token` a `az acr login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-619">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="d6d14-620">Corrigir a saída incorreta de `az acr task identity show -n Name -r Registry -o table`</span><span class="sxs-lookup"><span data-stu-id="d6d14-620">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="d6d14-621">az acr login: Gerar CLIError se erros forem retornados pelo comando docker</span><span class="sxs-lookup"><span data-stu-id="d6d14-621">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-622">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-622">ACS</span></span>

* <span data-ttu-id="d6d14-623">aks create/update: adicionar a validação `--vnet-subnet-id`</span><span class="sxs-lookup"><span data-stu-id="d6d14-623">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="d6d14-624">Aladdin</span><span class="sxs-lookup"><span data-stu-id="d6d14-624">Aladdin</span></span>

* <span data-ttu-id="d6d14-625">Analisar os exemplos gerados no _help.py do comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-625">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-626">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-626">AMS</span></span>

* <span data-ttu-id="d6d14-627">az ams já está em GA</span><span class="sxs-lookup"><span data-stu-id="d6d14-627">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-628">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-628">AppConfig</span></span>

* <span data-ttu-id="d6d14-629">Revisar a mensagem de ajuda para excluir o filtro de chave/rótulo não compatível</span><span class="sxs-lookup"><span data-stu-id="d6d14-629">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="d6d14-630">Remover a marca de versão prévia da maioria dos comandos que excluem a identidade gerenciada e têm sinalizadores</span><span class="sxs-lookup"><span data-stu-id="d6d14-630">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="d6d14-631">Adicionar a chave gerenciada do cliente ao atualizar os repositórios</span><span class="sxs-lookup"><span data-stu-id="d6d14-631">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-632">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-632">AppService</span></span>

* <span data-ttu-id="d6d14-633">az webapp list-runtimes: Corrigir o bug de list-runtimes</span><span class="sxs-lookup"><span data-stu-id="d6d14-633">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="d6d14-634">Adicionar az webapp|functionapp config ssl create</span><span class="sxs-lookup"><span data-stu-id="d6d14-634">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="d6d14-635">Adicionar compatibilidade com aplicativos de funções v3 e nó 12</span><span class="sxs-lookup"><span data-stu-id="d6d14-635">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-636">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-636">ARM</span></span>

* <span data-ttu-id="d6d14-637">az policy assignment create: Corrigir a mensagem de erro quando o parâmetro `--policy` for inválido</span><span class="sxs-lookup"><span data-stu-id="d6d14-637">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="d6d14-638">az group deployment create: Corrigir o erro "stat: o caminho é muito longo para o Windows" ao usar o arquivo grande parameters.json</span><span class="sxs-lookup"><span data-stu-id="d6d14-638">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-639">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-639">Backup</span></span>

* <span data-ttu-id="d6d14-640">Corrigir o fluxo de recuperação de nível de item no OLR</span><span class="sxs-lookup"><span data-stu-id="d6d14-640">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="d6d14-641">Adicionar compatibilidade com restauração como arquivo aos bancos de dados SQL e SAP</span><span class="sxs-lookup"><span data-stu-id="d6d14-641">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-642">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-642">Compute</span></span>

* <span data-ttu-id="d6d14-643">vm/vmss/availability-set update: adicionar --ppg para permitir a atualização de ProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="d6d14-643">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="d6d14-644">vmss create: adicionar --data-disk-iops e --data-disk-mbps</span><span class="sxs-lookup"><span data-stu-id="d6d14-644">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="d6d14-645">az vm host: remover a marca de versão prévia de `vm host` e `vm host group`</span><span class="sxs-lookup"><span data-stu-id="d6d14-645">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="d6d14-646">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 10.728: `az vm create`: criar uma sub-rede automaticamente quando a vnet for especificada e não houver uma sub-rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-646">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="d6d14-647">Aumentar a robustez da lista de imagens de VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-647">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="d6d14-648">Eventhub</span><span class="sxs-lookup"><span data-stu-id="d6d14-648">Eventhub</span></span>

* <span data-ttu-id="d6d14-649">Compatibilidade com o Azure Stack para o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-649">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-650">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-650">KeyVault</span></span>

* <span data-ttu-id="d6d14-651">az keyvault key create: adicionar um novo valor `import` ao parâmetro `--ops`</span><span class="sxs-lookup"><span data-stu-id="d6d14-651">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="d6d14-652">az keyvault key list-versions: compatibilidade com o parâmetro `--id` para especificar chaves</span><span class="sxs-lookup"><span data-stu-id="d6d14-652">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="d6d14-653">Compatibilidade com conexões de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-653">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-654">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-654">Network</span></span>

* <span data-ttu-id="d6d14-655">Avançar para azure-mgmt-network 9.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-655">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="d6d14-656">az network private-link-service update/create: dá suporte a --enable-proxy-protocol</span><span class="sxs-lookup"><span data-stu-id="d6d14-656">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="d6d14-657">Adicionar o recurso de Monitor de conexão V2</span><span class="sxs-lookup"><span data-stu-id="d6d14-657">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-658">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-658">Packaging</span></span>

* <span data-ttu-id="d6d14-659">[ALTERAÇÃO SIGNIFICATIVA] Fim da compatibilidade com o Python 2.7</span><span class="sxs-lookup"><span data-stu-id="d6d14-659">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-660">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-660">Profile</span></span>

* <span data-ttu-id="d6d14-661">Visualização: Adicionar novos atributos `homeTenantId` e `managedByTenants` às contas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="d6d14-661">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="d6d14-662">Executar `az login` novamente para as alterações entrarem em vigor</span><span class="sxs-lookup"><span data-stu-id="d6d14-662">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="d6d14-663">az login: Mostrar um aviso quando uma assinatura estiver listada de mais de um locatário e definir a primeira como padrão.</span><span class="sxs-lookup"><span data-stu-id="d6d14-663">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="d6d14-664">Para selecionar um locatário específico ao acessar essa assinatura, inclua `--tenant` em `az login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-664">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-665">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-665">Role</span></span>

* <span data-ttu-id="d6d14-666">az role assignment create: Corrigir o erro em que atribuir uma função a uma entidade de serviço pelo nome de exibição gera um HTTP 400</span><span class="sxs-lookup"><span data-stu-id="d6d14-666">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-667">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-667">SQL</span></span>

* <span data-ttu-id="d6d14-668">Atualizar o cmdlet da Instância Gerenciada do SQL `az sql mi update` com dois novos parâmetros: nível e família</span><span class="sxs-lookup"><span data-stu-id="d6d14-668">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-669">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-669">Storage</span></span>

* <span data-ttu-id="d6d14-670">[ALTERAÇÃO DA FALHA] `az storage account create`: Alterar o tipo de conta de armazenamento padrão para StorageV2</span><span class="sxs-lookup"><span data-stu-id="d6d14-670">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="d6d14-671">4 de fevereiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-671">February 04, 2020</span></span>

<span data-ttu-id="d6d14-672">Versão 2.0.81</span><span class="sxs-lookup"><span data-stu-id="d6d14-672">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-673">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-673">ACS</span></span>

* <span data-ttu-id="d6d14-674">Adicionar suporte para definir portas alocadas de saída e tempos limite ociosos no balanceador de carga standard</span><span class="sxs-lookup"><span data-stu-id="d6d14-674">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="d6d14-675">Atualizar para a versão da API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-675">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-676">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-676">ACR</span></span>

* <span data-ttu-id="d6d14-677">A [ALTERAÇÃO DA FALHA] `az acr delete` será exibida</span><span class="sxs-lookup"><span data-stu-id="d6d14-677">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="d6d14-678">A [ALTERAÇÃO SIGNIFICATIVA] 'az acr task delete’ será exibida</span><span class="sxs-lookup"><span data-stu-id="d6d14-678">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="d6d14-679">Adicionar um novo grupo de comandos ‘az acr taskrun show/list/delete’ para o gerenciamento de taskrun</span><span class="sxs-lookup"><span data-stu-id="d6d14-679">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-680">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-680">AKS</span></span>

* <span data-ttu-id="d6d14-681">Cada cluster obtém uma entidade de serviço separada para aprimorar o isolamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-681">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-682">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-682">AppConfig</span></span>

* <span data-ttu-id="d6d14-683">Dar suporte à importação/exportação de referências keyvault de/a appservice</span><span class="sxs-lookup"><span data-stu-id="d6d14-683">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="d6d14-684">Dar suporte à importação/exportação de todos os rótulos de appconfig para appconfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-684">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="d6d14-685">Validar nomes de chave e recursos antes de configurar e importar</span><span class="sxs-lookup"><span data-stu-id="d6d14-685">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="d6d14-686">Exponha a modificação do sku para o repositório de configurações.</span><span class="sxs-lookup"><span data-stu-id="d6d14-686">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="d6d14-687">Adicione o grupo de comandos à identidade gerenciada.</span><span class="sxs-lookup"><span data-stu-id="d6d14-687">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-688">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-688">AppService</span></span>

* <span data-ttu-id="d6d14-689">Azure Stack: comandos de superfície no perfil de 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-689">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="d6d14-690">functionapp: adicionar a capacidade de criar aplicativos de funções Java no Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-690">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-691">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-691">ARM</span></span>

* <span data-ttu-id="d6d14-692">Correção de problema nº 10246: `az resource tag` falha quando o parâmetro `--ids` passado é a ID do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="d6d14-692">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="d6d14-693">Correção de problema nº 11658: o comando `az group export` não é compatível com os parâmetros `--query` e `--output`</span><span class="sxs-lookup"><span data-stu-id="d6d14-693">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="d6d14-694">Correção de problema nº 10279: O código de saída `az group deployment validate` é 0 quando a verificação falha</span><span class="sxs-lookup"><span data-stu-id="d6d14-694">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="d6d14-695">Correção de problema nº 9916: aprimorar a mensagem de erro do conflito entre a marca e outras condições de filtro para o comando `az resource list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-695">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="d6d14-696">Adicionar novo parâmetro `--managed-by` para dar suporte à adição de informações managedBy para o comando `az group create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-696">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="d6d14-697">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-697">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="d6d14-698">Adicionar o subgrupo `monitor` para gerenciar o monitoramento do Log Analytics no cluster do Red Hat OpensShift no Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-698">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-699">BotService</span><span class="sxs-lookup"><span data-stu-id="d6d14-699">BotService</span></span>

* <span data-ttu-id="d6d14-700">Correção de problema nº 11697: `az bot create` não é idempotente</span><span class="sxs-lookup"><span data-stu-id="d6d14-700">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="d6d14-701">Alterar testes de correção de nomes para serem executados somente em modo Ao vivo</span><span class="sxs-lookup"><span data-stu-id="d6d14-701">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-702">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-702">CDN</span></span>

* <span data-ttu-id="d6d14-703">Adicionar suporte ao recurso rulesEngine</span><span class="sxs-lookup"><span data-stu-id="d6d14-703">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="d6d14-704">Adicionar o novo grupo de comandos ‘cdn endpoint rule’ para gerenciar regras</span><span class="sxs-lookup"><span data-stu-id="d6d14-704">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="d6d14-705">Atualizar a versão azure-mgmt-cdn para a 4.0.0 para usar a versão da API 2019-04-15</span><span class="sxs-lookup"><span data-stu-id="d6d14-705">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="d6d14-706">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-706">Deployment Manager</span></span>

* <span data-ttu-id="d6d14-707">Adicione a operação de lista para todos os recursos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-707">Add list operation for all resources.</span></span>
* <span data-ttu-id="d6d14-708">Aprimore o recurso de etapa do novo tipo de etapa.</span><span class="sxs-lookup"><span data-stu-id="d6d14-708">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="d6d14-709">Atualize o pacote azure-mgmt-deploymentmanager para usar a versão 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="d6d14-709">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-710">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-710">IoT</span></span>

* <span data-ttu-id="d6d14-711">Substitua os comandos ‘IoT hub Job’.</span><span class="sxs-lookup"><span data-stu-id="d6d14-711">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="d6d14-712">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-712">IoT Central</span></span>

* <span data-ttu-id="d6d14-713">Dê suporte à atualização/criação de aplicativos com o novo nome do SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="d6d14-713">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-714">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-714">Key Vault</span></span>

* <span data-ttu-id="d6d14-715">Adicione um novo comando `az keyvault key download` para baixar chaves.</span><span class="sxs-lookup"><span data-stu-id="d6d14-715">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="d6d14-716">Diversos</span><span class="sxs-lookup"><span data-stu-id="d6d14-716">Misc</span></span>

* <span data-ttu-id="d6d14-717">Correção nº 6371: dar suporte à conclusão da variável de nome de arquivo e de ambiente em Bash</span><span class="sxs-lookup"><span data-stu-id="d6d14-717">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-718">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-718">Network</span></span>

* <span data-ttu-id="d6d14-719">Correção nº 2092: az network dns record-set add/remove: adicione um aviso quando record-set não é encontrado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-719">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="d6d14-720">No futuro, haverá suporte para um argumento extra para confirmar essa criação automática.</span><span class="sxs-lookup"><span data-stu-id="d6d14-720">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="d6d14-721">Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-721">Policy</span></span>

* <span data-ttu-id="d6d14-722">Adicionar o novo comando `az policy metadata` para recuperar recursos avançados de metadados de política</span><span class="sxs-lookup"><span data-stu-id="d6d14-722">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="d6d14-723">`az policy remediation create`: Especifique se a conformidade deve ser reavaliada antes da correção com o parâmetro `--resource-discovery-mode`</span><span class="sxs-lookup"><span data-stu-id="d6d14-723">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-724">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-724">Profile</span></span>

* <span data-ttu-id="d6d14-725">`az account get-access-token`: Adicionar parâmetro `--tenant` para adquirir o token do locatário diretamente, sem a necessidade de especificar uma assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-725">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-726">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-726">RBAC</span></span>

* <span data-ttu-id="d6d14-727">[ALTERAÇÃO SIGNIFICATIVA] Correção nº 11883: `az role assignment create`: o escopo vazio exibirá erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-727">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="d6d14-728">Segurança</span><span class="sxs-lookup"><span data-stu-id="d6d14-728">Security</span></span>

* <span data-ttu-id="d6d14-729">Adicione novos comandos `az atp show` e `az atp update` para exibir e gerenciar configurações avançadas de proteção contra ameaças para contas de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-729">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-730">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-730">SQL</span></span>

* <span data-ttu-id="d6d14-731">`sql dw create`: substitua os parâmetros `--zone-redundant` e `--read-replica-count`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-731">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="d6d14-732">Esses parâmetros não se aplicam ao DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="d6d14-732">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="d6d14-733">[ALTERAÇÃO DA FALHA] `az sql db create`: Remova "WideWorldImportersStd" e "WideWorldImportersFull" como valores permitidos documentados para "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="d6d14-733">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="d6d14-734">Esses bancos de dados de exemplo sempre farão a criação falhar.</span><span class="sxs-lookup"><span data-stu-id="d6d14-734">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="d6d14-735">Adicione os novos comandos `sql db classification show/list/update/delete` e `sql db classification recommendation list/enable/disable` para gerenciar classificações de confidencialidade para bancos de dados SQL.</span><span class="sxs-lookup"><span data-stu-id="d6d14-735">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="d6d14-736">`az sql db audit-policy`: Correção para ações e grupos de auditoria vazios</span><span class="sxs-lookup"><span data-stu-id="d6d14-736">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-737">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-737">Storage</span></span>

* <span data-ttu-id="d6d14-738">Adicione um novo grupo de comandos `az storage share-rm` para usar o provedor de recursos Microsoft.Storage para operações de gerenciamento de compartilhamento de arquivo do Azure.</span><span class="sxs-lookup"><span data-stu-id="d6d14-738">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="d6d14-739">Correção de problema nº 11415: erro de permissão para `az storage blob update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-739">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="d6d14-740">Integre Azcopy 10.3.3 e dê suporte a Win32.</span><span class="sxs-lookup"><span data-stu-id="d6d14-740">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="d6d14-741">`az storage copy`: Adicione os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="d6d14-741">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="d6d14-742">`az storage remove`: Altere os parâmetros `--inlcude` e `--exclude` para os parâmetros `--include-path`, `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="d6d14-742">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="d6d14-743">`az storage sync`: Adicione os parâmetros `--include-pattern`, `--exclude-path` e `--exclude-pattern`</span><span class="sxs-lookup"><span data-stu-id="d6d14-743">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="d6d14-744">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-744">ServiceFabric</span></span>

* <span data-ttu-id="d6d14-745">Adicione novos comandos para gerenciar o aplicativo e os serviços.</span><span class="sxs-lookup"><span data-stu-id="d6d14-745">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="d6d14-746">13 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-746">January 13, 2020</span></span>

<span data-ttu-id="d6d14-747">Versão 2.0.80</span><span class="sxs-lookup"><span data-stu-id="d6d14-747">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-748">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-748">Compute</span></span>

* <span data-ttu-id="d6d14-749">atualização do disco: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="d6d14-749">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="d6d14-750">criação/atualização do instantâneo: Adicionar --disk-encryption-set e --encryption-type</span><span class="sxs-lookup"><span data-stu-id="d6d14-750">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-751">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-751">Storage</span></span>

* <span data-ttu-id="d6d14-752">Atualizar a versão do azure-mgmt-storage para 7.1.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-752">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="d6d14-753">`az storage account create`: Adicionar `--encryption-key-type-for-table` e `--encryption-key-type-for-queue` para dar suporte ao Serviço de Criptografia de Tabela e de Fila</span><span class="sxs-lookup"><span data-stu-id="d6d14-753">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="d6d14-754">07 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-754">January 07, 2020</span></span>

<span data-ttu-id="d6d14-755">Versão 2.0.79</span><span class="sxs-lookup"><span data-stu-id="d6d14-755">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-756">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-756">ACR</span></span>

* <span data-ttu-id="d6d14-757">[ALTERAÇÃO SIGNIFICATIVA] Remover o parâmetro '--os' para 'acr build', 'acr task create/update', 'acr run' e 'acr pack'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-757">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="d6d14-758">Em vez disso, use '--platform'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-758">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-759">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-759">AppConfig</span></span>

* <span data-ttu-id="d6d14-760">Adicionar suporte para importar/exportar sinalizadores de recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-760">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="d6d14-761">Adicione o novo comando 'az appconfig kv set-keyvault' para criar a referência do keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-761">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="d6d14-762">Suporte a várias convenções de nomenclatura ao exportar os sinalizadores de recurso para o arquivo</span><span class="sxs-lookup"><span data-stu-id="d6d14-762">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-763">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-763">AppService</span></span>

* <span data-ttu-id="d6d14-764">Corrigir o problema #7154: Atualizar a documentação para o comando <> para usar acentos grave em vez de aspas simples</span><span class="sxs-lookup"><span data-stu-id="d6d14-764">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="d6d14-765">Corrigir o problema #11287: webapp up: Por padrão, faça o aplicativo criado usando 'should be 'SSL enabled'</span><span class="sxs-lookup"><span data-stu-id="d6d14-765">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="d6d14-766">Corrigir o problema #11592: Adicionar o sinalizador az webapp up para sites HTML estáticos</span><span class="sxs-lookup"><span data-stu-id="d6d14-766">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-767">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-767">ARM</span></span>

* <span data-ttu-id="d6d14-768">Corrigir `az resource tag`: As marcas do Cofre dos Serviços de Recuperação não podem ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-768">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-769">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-769">Backup</span></span>

* <span data-ttu-id="d6d14-770">Novo comando 'backup protection undelete' adicionado para habilitar o recurso de exclusão reversível para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="d6d14-770">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="d6d14-771">Novo parâmetro '--soft-delete-feature-state' adicionado para definir o comando propriedades do backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-771">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="d6d14-772">Suporte de exclusão de disco adicionado para carga de trabalho IaasVM</span><span class="sxs-lookup"><span data-stu-id="d6d14-772">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-773">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-773">Compute</span></span>

* <span data-ttu-id="d6d14-774">Corrigir a falha `vm create` no perfil do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d6d14-774">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="d6d14-775">parte final/listar definições de métricas de monitor de vm: suporte a métricas de consulta e definições de lista para uma vm.</span><span class="sxs-lookup"><span data-stu-id="d6d14-775">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="d6d14-776">Adicionar nova ação de comando de reaplicação para az vm</span><span class="sxs-lookup"><span data-stu-id="d6d14-776">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-777">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-777">HDInsight</span></span>

* <span data-ttu-id="d6d14-778">Suporte para criar um cluster Kafka com o Proxy REST do Kafka</span><span class="sxs-lookup"><span data-stu-id="d6d14-778">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="d6d14-779">Atualizar azure-mgmt-hdinsight para 1.3.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-779">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="d6d14-780">Diversos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-780">Misc.</span></span>

* <span data-ttu-id="d6d14-781">Adicionar comando de visualização `az version show` para mostrar as versões dos módulos e das extensões da CLI do Azure no formato JSON por padrão ou no formato configurado por --output</span><span class="sxs-lookup"><span data-stu-id="d6d14-781">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="d6d14-782">Hubs de Eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-782">Event Hubs</span></span>

* <span data-ttu-id="d6d14-783">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az eventhubs eventhub update' e 'az eventhubs eventhub create'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-783">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="d6d14-784">Essa opção não é válida para entidades do Hub de Eventos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-784">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="d6d14-785">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-785">Service Bus</span></span>

* <span data-ttu-id="d6d14-786">[ALTERAÇÃO SIGNIFICATIVA] Remover a opção de status 'ReceiveDisabled' do comando 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create' e 'az servicebus queue update'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-786">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="d6d14-787">Essa opção não é válida para tópicos e filas do Barramento de Serviço.</span><span class="sxs-lookup"><span data-stu-id="d6d14-787">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-788">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-788">RBAC</span></span>

* <span data-ttu-id="d6d14-789">Correção #11712: `az ad app/sp show` não devolve o código de saída 3 quando o aplicativo ou a entidade de serviço não existir</span><span class="sxs-lookup"><span data-stu-id="d6d14-789">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-790">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-790">Storage</span></span>

* <span data-ttu-id="d6d14-791">`az storage account create`: Remover o sinalizador de visualização do parâmetro --enable-hierarchical-namespace</span><span class="sxs-lookup"><span data-stu-id="d6d14-791">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="d6d14-792">Atualizar a versão azure-mgmt-storage para 7.0.0 para usar a versão de API 2019-06-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-792">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="d6d14-793">Adicionar novos parâmetros `--enable-delete-retention` e `--delete-retention-days` para dar suporte ao gerenciamento da política de retenção de exclusão para a conta de armazenamento blob-service-properties.</span><span class="sxs-lookup"><span data-stu-id="d6d14-793">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="d6d14-794">17 de dezembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-794">December 17, 2019</span></span>

<span data-ttu-id="d6d14-795">2.0.78</span><span class="sxs-lookup"><span data-stu-id="d6d14-795">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-796">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-796">ACR</span></span>

* <span data-ttu-id="d6d14-797">Contexto local de suporte adicionado na execução da tarefa acr</span><span class="sxs-lookup"><span data-stu-id="d6d14-797">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-798">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-798">ACS</span></span>

* <span data-ttu-id="d6d14-799">[ALTERAÇÃO SIGNIFICATIVA]criar az openshift: renomear `--workspace-resource-id` para `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-799">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-800">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-800">AMS</span></span>

* <span data-ttu-id="d6d14-801">Comandos de exibição atualizados para devolver 3 quando o recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="d6d14-801">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-802">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-802">AppConfig</span></span>

* <span data-ttu-id="d6d14-803">Bug corrigido ao acrescentar a versão de API à URL de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6d14-803">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="d6d14-804">A solução existente não funciona com a paginação.</span><span class="sxs-lookup"><span data-stu-id="d6d14-804">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="d6d14-805">Suporte adicionado para a exibição de idiomas além do inglês, pois nosso serviço de back-end é compatível com unicode para globalização.</span><span class="sxs-lookup"><span data-stu-id="d6d14-805">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-806">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-806">AppService</span></span>

* <span data-ttu-id="d6d14-807">Problema corrigido nº 11217: webapp: o upload ssl de configuração do az webapp deve ser compatível com o parâmetro do slot</span><span class="sxs-lookup"><span data-stu-id="d6d14-807">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="d6d14-808">Problema corrigido nº 10965: Erro: O nome não pode estar vazio.</span><span class="sxs-lookup"><span data-stu-id="d6d14-808">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="d6d14-809">Permitir remoção por ip_address e sub-rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-809">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="d6d14-810">Suporte adicionado para importar certificados do Key Vault `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-810">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-811">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-811">ARM</span></span>

* <span data-ttu-id="d6d14-812">Pacote azure-mgmt-resource atualizado para usar 6.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-812">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="d6d14-813">Suporte entre locatários para o comando `az group deployment create` adicionando o novo parâmetro `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="d6d14-813">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="d6d14-814">Novo parâmetro `--metadata` adicionado para dar suporte à adição de informações de metadados para definições de conjunto de políticas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-814">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-815">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-815">Backup</span></span>

* <span data-ttu-id="d6d14-816">Suporte de backup adicionado para carga de trabalho SQL e SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="d6d14-816">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-817">BotService</span><span class="sxs-lookup"><span data-stu-id="d6d14-817">BotService</span></span>

* <span data-ttu-id="d6d14-818">[ALTERAÇÃO SIGNIFICATIVA] Remover o sinalizador '--version ' do comando de visualização 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-818">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="d6d14-819">Somente os bots do SDK v4 são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="d6d14-819">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="d6d14-820">Verificação de disponibilidade de nome adicionada para 'az bot create'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-820">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="d6d14-821">Suporte adicionado para atualizar a URL do ícone para um bot por meio de 'az bot update'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-821">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="d6d14-822">Suporte adicionado para atualizar um canal Direct Line por meio de 'az bot directline update'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-822">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="d6d14-823">Suporte ao sinalizador '--enable-enhanced-auth' adicionado para 'az bot directline create'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-823">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="d6d14-824">Os seguintes grupos de comandos estão em GA e não estão em versão prévia: 'az bot authsetting'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-824">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="d6d14-825">Os seguintes comandos em 'az bot' estão em GA e não na versão prévia: 'criar', 'preparar-implantar', 'mostrar', 'excluir', 'atualizar'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-825">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="d6d14-826">Correção do valor 'az bot prepare-deploy' alterando '--proj-file-path ' para letras minúsculas (por exemplo, "Test. csproj" para "Test. csproj").</span><span class="sxs-lookup"><span data-stu-id="d6d14-826">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-827">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-827">Compute</span></span>

* <span data-ttu-id="d6d14-828">Criar/atualizar vmss: --scale-in-policy adicionado, que decide quais máquinas virtuais são escolhidas para remoção quando um VMSS é dimensionado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-828">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="d6d14-829">atualização de vm/vmss: --priority adicionado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-829">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="d6d14-830">atualização de vm/vmss: --max-price adicionado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-830">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="d6d14-831">Grupo de comandos do conjunto de criptografia de disco adicionado (criar, mostrar, atualizar, excluir e listar).</span><span class="sxs-lookup"><span data-stu-id="d6d14-831">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="d6d14-832">criação de disco: --encryption-type e --disk-encryption-set adicionados.</span><span class="sxs-lookup"><span data-stu-id="d6d14-832">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="d6d14-833">vm/vmss create: --os-disk-encryption-set e --data-disk-encryption-sets adicionados.</span><span class="sxs-lookup"><span data-stu-id="d6d14-833">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-834">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-834">Core</span></span>

* <span data-ttu-id="d6d14-835">Suporte para Python 3.4 removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-835">Removed support for Python 3.4</span></span>
* <span data-ttu-id="d6d14-836">Pesquisa de funções de plug-in em vários comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-836">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="d6d14-837">DLS</span><span class="sxs-lookup"><span data-stu-id="d6d14-837">DLS</span></span>

* <span data-ttu-id="d6d14-838">Versão atualizada do SDK do ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="d6d14-838">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="d6d14-839">Instalar</span><span class="sxs-lookup"><span data-stu-id="d6d14-839">Install</span></span>

* <span data-ttu-id="d6d14-840">Instalar suporte de script Python 3.8</span><span class="sxs-lookup"><span data-stu-id="d6d14-840">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-841">IOT</span><span class="sxs-lookup"><span data-stu-id="d6d14-841">IOT</span></span>

* <span data-ttu-id="d6d14-842">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro--failover-region removido de failover manual.</span><span class="sxs-lookup"><span data-stu-id="d6d14-842">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="d6d14-843">Agora ele fará failover para a região secundária emparelhada atribuída geograficamente.</span><span class="sxs-lookup"><span data-stu-id="d6d14-843">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-844">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-844">Key Vault</span></span>

* <span data-ttu-id="d6d14-845">Nº 8095 corrigido: `az keyvault storage remove`: melhorar a mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-845">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="d6d14-846">Nº 8921 corrigido: `az keyvault key/secret/certificate list/list-deleted/list-versions`: corrigir o bug de validação no parâmetro `--maxresults`</span><span class="sxs-lookup"><span data-stu-id="d6d14-846">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="d6d14-847">Nº 10512 corrigido: `az keyvault set-policy`: melhorar a mensagem de erro quando nenhuma das `--object-id`, `--spn` ou `--upn` for especificada</span><span class="sxs-lookup"><span data-stu-id="d6d14-847">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="d6d14-848">Nº 10846 corrigido: `az keyvault secret show-deleted`: quando `--id` for especificado, `--name/-n` não será necessário</span><span class="sxs-lookup"><span data-stu-id="d6d14-848">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="d6d14-849">Nº 11084 corrigido: `az keyvault secret download`: melhorar a mensagem de ajuda do parâmetro `--encoding`</span><span class="sxs-lookup"><span data-stu-id="d6d14-849">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-850">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-850">Network</span></span>

* <span data-ttu-id="d6d14-851">Investigação de gateway de aplicativo de rede az: Suporte --port option adicionado para especificar uma porta para sondar servidores de back-end ao criar e atualizar</span><span class="sxs-lookup"><span data-stu-id="d6d14-851">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="d6d14-852">az network application-gateway url-path-map create/update: correção de bug para `--waf-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-852">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="d6d14-853">az network application-gateway: Suporte `--rewrite-rule-set` adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-853">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="d6d14-854">az network list-service-aliases: Foram adicionados aliases de serviço da lista de suporte que podem ser usados para políticas de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-854">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="d6d14-855">importar zona dns da rede az: Suporte adicionado. @ no nome do registro</span><span class="sxs-lookup"><span data-stu-id="d6d14-855">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-856">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-856">Packaging</span></span>

* <span data-ttu-id="d6d14-857">Compilações de back edge adicionadas para instalação de pip</span><span class="sxs-lookup"><span data-stu-id="d6d14-857">Added back edge builds for pip install</span></span>
* <span data-ttu-id="d6d14-858">Pacote eoan do Ubuntu adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-858">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="d6d14-859">Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-859">Policy</span></span>

* <span data-ttu-id="d6d14-860">Inclusão de compatibilidade com a API de Política, versão de 01/09/2019.</span><span class="sxs-lookup"><span data-stu-id="d6d14-860">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="d6d14-861">az policy set-definition: Agrupamento de suporte adicionado nas definições do conjunto de políticas com `--definition-groups` parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6d14-861">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-862">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-862">Redis</span></span>

* <span data-ttu-id="d6d14-863">Adicionado o parâmetro de visualização `--replicas-per-master` ao comando `az redis create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-863">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="d6d14-864">Azure-MGMT-Redis adicionado do 6.0.0 para o 7.0.0rc1</span><span class="sxs-lookup"><span data-stu-id="d6d14-864">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="d6d14-865">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-865">ServiceFabric</span></span>

* <span data-ttu-id="d6d14-866">Corrigido em nó-tipo adicionar lógica, incluindo #10963: A adição do novo tipo de nó com nível de durabilidade Gold sempre gerará erro da CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-866">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="d6d14-867">Versão do ServiceFabricNodeVmExt atualizada para 1.1 no modelo de criação</span><span class="sxs-lookup"><span data-stu-id="d6d14-867">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-868">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-868">SQL</span></span>

* <span data-ttu-id="d6d14-869">Adicionados os parâmetros "--read-scale" e "--read-replicas" aos comandos criar e atualizar do BD SQL para dar suporte ao gerenciamento de escala de leitura.</span><span class="sxs-lookup"><span data-stu-id="d6d14-869">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-870">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-870">Storage</span></span>

* <span data-ttu-id="d6d14-871">Propriedade de compartilhamentos de arquivos grandes da versão GA para o comando criar e atualizar da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-871">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="d6d14-872">Suporte ao token SAS de delegação de usuário da versão GA</span><span class="sxs-lookup"><span data-stu-id="d6d14-872">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="d6d14-873">Novos comandos adicionados `az storage account blob-service-properties show` e `az storage account blob-service-properties update --enable-change-feed` para gerenciar Propriedades do serviço blob para a conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-873">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="d6d14-874">[PRÓXIMA ALTERAÇÃO DA FALHA] `az storage copy`: `*` não há mais suporte para o caractere de como um curinga na URL, mas novos parâmetros--include-pattern e --exclude-pattern serão adicionados com suporte a curinga `*`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-874">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="d6d14-875">Problema corrigido nº 11043: Suporte adicionado para remover contêiner/compartilhamento inteiro no comando `az storage remove`</span><span class="sxs-lookup"><span data-stu-id="d6d14-875">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="d6d14-876">26 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-876">November 26, 2019</span></span>

<span data-ttu-id="d6d14-877">Versão 2.0.77</span><span class="sxs-lookup"><span data-stu-id="d6d14-877">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-878">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-878">ACR</span></span>

* <span data-ttu-id="d6d14-879">Parâmetro `--branch` preterido da criação/atualização da tarefa ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-879">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="d6d14-880">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-880">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="d6d14-881">Sinalizador `--workspace-resource-id` adicionado para permitir a criação do cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-881">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="d6d14-882">`monitor_profile` adicionado para criar o cluster do Red Hat OpenShift no Azure com monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-882">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-883">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-883">AKS</span></span>

* <span data-ttu-id="d6d14-884">Operação de rotação de certificado de cluster de suporte adicionada usando "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="d6d14-884">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-885">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-885">AppConfig</span></span>

* <span data-ttu-id="d6d14-886">Suporte adicionado para usar ":" para o separador `as az appconfig kv import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-886">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="d6d14-887">Problema corrigido para listar valores de chave com vários rótulos incluindo o rótulo nulo.</span><span class="sxs-lookup"><span data-stu-id="d6d14-887">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="d6d14-888">SDK do plano de gerenciamento atualizado, azure-mgmt-appconfiguration, para a versão 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="d6d14-888">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="d6d14-889">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-889">AppService</span></span>

* <span data-ttu-id="d6d14-890">Problema corrigido nº 11100: AttributeError para az webapp up ao criar o plano de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-890">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="d6d14-891">az webapp up: Forçar a criação ou a implantação em um site para linguagens com suporte, nenhum padrão usado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-891">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="d6d14-892">Suporte adicionado para o Ambiente do Serviço de Aplicativo: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="d6d14-892">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-893">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-893">Backup</span></span>

* <span data-ttu-id="d6d14-894">Problema corrigido em list-associated-items da política de backup az.</span><span class="sxs-lookup"><span data-stu-id="d6d14-894">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="d6d14-895">Parâmetro BackupManagementType opcional adicionado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-895">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-896">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-896">Compute</span></span>

* <span data-ttu-id="d6d14-897">Versão de API de computação, discos e instantâneos atualizados para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-897">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="d6d14-898">vmss create: melhoria para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="d6d14-898">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="d6d14-899">sig image-definition create: --os-state adicionado para permitir a especificação se as máquinas virtuais criadas nessa imagem são 'Generalizadas' ou 'Especializadas'</span><span class="sxs-lookup"><span data-stu-id="d6d14-899">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="d6d14-900">sig image-definition create: --hyper-v-generation adicionado para permitir a especificação da geração do hipervisor</span><span class="sxs-lookup"><span data-stu-id="d6d14-900">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="d6d14-901">sig image-version create: --os-snapshot e --data-snapshots de suporte adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-901">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="d6d14-902">image create: --data-disk-caching adicionado para permitir a especificação da configuração de cache de discos de dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-902">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="d6d14-903">SDK de computação do Python atualizado para 10.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-903">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="d6d14-904">vm/vmss create: 'Spot' adicionado à propriedade de enumeração 'Priority'</span><span class="sxs-lookup"><span data-stu-id="d6d14-904">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="d6d14-905">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro '--max-billing' renomeado para '--max-price', para a VM e o VMSS, a fim de que seja consistente com os cmdlets do Swagger e do PowerShell</span><span class="sxs-lookup"><span data-stu-id="d6d14-905">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="d6d14-906">vm monitor log show: suporte adicionado para consultar o log pelo workspace do Log Analytics vinculado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-906">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-907">IOT</span><span class="sxs-lookup"><span data-stu-id="d6d14-907">IOT</span></span>

* <span data-ttu-id="d6d14-908">Correção nº 2531: argumentos de conveniência adicionados para a atualização do hub.</span><span class="sxs-lookup"><span data-stu-id="d6d14-908">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="d6d14-909">Correção nº 8323: parâmetros ausentes adicionados para criar o ponto de extremidade personalizado de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-909">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="d6d14-910">Corrigir bug de regressão: as alterações que substituem o ponto de extremidade de armazenamento padrão foram revertidas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-910">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-911">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-911">Key Vault</span></span>

* <span data-ttu-id="d6d14-912">Correção nº 11121: ao usar `az keyvault certificate list`, passar `--include-pending` agora não exige um valor de `true` ou `false`</span><span class="sxs-lookup"><span data-stu-id="d6d14-912">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="d6d14-913">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="d6d14-913">NetAppFiles</span></span>

* <span data-ttu-id="d6d14-914">azure-mgmt-netapp atualizado para 0.7.0 que inclui algumas propriedades de volume adicionais associadas a operações de replicação futuras</span><span class="sxs-lookup"><span data-stu-id="d6d14-914">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-915">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-915">Network</span></span>

* <span data-ttu-id="d6d14-916">application-gateway waf-config: preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-916">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="d6d14-917">application-gateway waf-policy: subgrupo managed-rules adicionado para gerenciar os conjuntos de regras e regras de exclusão gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-917">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="d6d14-918">application-gateway waf-policy: subgrupo policy-setting adicionado para gerenciar a configuração global de um waf-policy</span><span class="sxs-lookup"><span data-stu-id="d6d14-918">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="d6d14-919">[ALTERAÇÃO SIGNIFICATIVA] application-gateway waf-policy: subgrupo rule renomeado para custom-rule</span><span class="sxs-lookup"><span data-stu-id="d6d14-919">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="d6d14-920">application-gateway http-listener: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="d6d14-920">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="d6d14-921">application-gateway url-path-map rule: --firewall-policy adicionado durante a criação</span><span class="sxs-lookup"><span data-stu-id="d6d14-921">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="d6d14-922">Empacotamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-922">Packaging</span></span>

* <span data-ttu-id="d6d14-923">Wrapper az reescrito no Python</span><span class="sxs-lookup"><span data-stu-id="d6d14-923">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="d6d14-924">Suporte adicionado para Python 3.8</span><span class="sxs-lookup"><span data-stu-id="d6d14-924">Added support for Python 3.8</span></span>
* <span data-ttu-id="d6d14-925">Alterado para Python 3 para o pacote RPM</span><span class="sxs-lookup"><span data-stu-id="d6d14-925">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-926">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-926">Profile</span></span>

* <span data-ttu-id="d6d14-927">Erro aperfeiçoado ao executar `az login -u {} -p {}` com a conta Microsoft</span><span class="sxs-lookup"><span data-stu-id="d6d14-927">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="d6d14-928">`SSLError` aperfeiçoado ao executar `az login` atrás de um proxy com o certificado raiz autoassinado</span><span class="sxs-lookup"><span data-stu-id="d6d14-928">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="d6d14-929">Correção nº 10578: `az login` trava quando mais de uma instância é iniciada ao mesmo tempo no Windows ou WSL</span><span class="sxs-lookup"><span data-stu-id="d6d14-929">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="d6d14-930">Correção nº 11059: `az login --allow-no-subscriptions` falhará se houver assinaturas no locatário</span><span class="sxs-lookup"><span data-stu-id="d6d14-930">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="d6d14-931">Correção nº 11238: após renomear uma assinatura, fazer logon com a MSI fará a mesma assinatura aparecer duas vezes</span><span class="sxs-lookup"><span data-stu-id="d6d14-931">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-932">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-932">RBAC</span></span>

* <span data-ttu-id="d6d14-933">Correção nº 10996: erro aperfeiçoado para `--force-change-password-next-login` em `az ad user update` quando `--password` não for especificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-933">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-934">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-934">Redis</span></span>

* <span data-ttu-id="d6d14-935">Correção nº 2902: evite definir configurações de memória ao atualizar o cache do SKU básico</span><span class="sxs-lookup"><span data-stu-id="d6d14-935">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="d6d14-936">Reservas</span><span class="sxs-lookup"><span data-stu-id="d6d14-936">Reservations</span></span>

* <span data-ttu-id="d6d14-937">Versão do SDK atualizada para 0.6.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-937">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="d6d14-938">Informações de detalhes do plano de cobrança atualizadas após chamar Get-Gatalogs</span><span class="sxs-lookup"><span data-stu-id="d6d14-938">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="d6d14-939">Novo comando `az reservations reservation-order calculate` adicionado para calcular o preço de uma reserva</span><span class="sxs-lookup"><span data-stu-id="d6d14-939">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="d6d14-940">Novo comando `az reservations reservation-order purchase` adicionado para comprar uma nova reserva</span><span class="sxs-lookup"><span data-stu-id="d6d14-940">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="d6d14-941">Rest</span><span class="sxs-lookup"><span data-stu-id="d6d14-941">Rest</span></span>
* <span data-ttu-id="d6d14-942">`az rest` alterado para GA</span><span class="sxs-lookup"><span data-stu-id="d6d14-942">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-943">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-943">SQL</span></span>

* <span data-ttu-id="d6d14-944">azure-mgmt-sql atualizado para 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="d6d14-944">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-945">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-945">Storage</span></span>

* <span data-ttu-id="d6d14-946">storage account create: --enable-hierarchical-namespace adicionado para dar suporte à semântica do sistema de arquivos no serviço Blob.</span><span class="sxs-lookup"><span data-stu-id="d6d14-946">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="d6d14-947">Exceção não relacionada removida da mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-947">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="d6d14-948">Problemas corrigidos com a mensagem de erro incorreta "Você não tem as permissões necessárias para executar essa operação."</span><span class="sxs-lookup"><span data-stu-id="d6d14-948">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="d6d14-949">quando bloqueado pelas regras de rede ou AuthenticationFailed.</span><span class="sxs-lookup"><span data-stu-id="d6d14-949">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="d6d14-950">4 de novembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-950">November 4, 2019</span></span>

<span data-ttu-id="d6d14-951">Versão 2.0.76</span><span class="sxs-lookup"><span data-stu-id="d6d14-951">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-952">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-952">ACR</span></span>

* <span data-ttu-id="d6d14-953">O parâmetro de versão prévia `--pack-image-tag` foi adicionado ao comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-953">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="d6d14-954">Suporte adicionado para habilitar a auditoria na criação de um registro</span><span class="sxs-lookup"><span data-stu-id="d6d14-954">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="d6d14-955">Suporte adicionado para o RBAC com escopo de repositório</span><span class="sxs-lookup"><span data-stu-id="d6d14-955">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-956">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-956">AKS</span></span>

* <span data-ttu-id="d6d14-957">`--enable-cluster-autoscaler`, `--min-count` e `--max-count` foram adicionados ao comando `az aks create`, que habilita o dimensionamento automático do cluster para o pool de nós.</span><span class="sxs-lookup"><span data-stu-id="d6d14-957">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="d6d14-958">Foram adicionados os sinalizadores acima, bem como `--update-cluster-autoscaler` e `--disable-cluster-autoscaler` ao comando `az aks update`, permitindo atualizações do cluster de dimensionamento automático.</span><span class="sxs-lookup"><span data-stu-id="d6d14-958">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="d6d14-959">AppConfig</span><span class="sxs-lookup"><span data-stu-id="d6d14-959">AppConfig</span></span>

* <span data-ttu-id="d6d14-960">O grupo de comandos do recurso AppConfig foi adicionado para gerenciar os sinalizadores de recurso armazenados em uma Configuração de Aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-960">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="d6d14-961">Foi corrigido um bug secundário do comando de exportação para arquivo appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="d6d14-961">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="d6d14-962">Foi interrompida a leitura de conteúdo do arquivo de destino durante a exportação.</span><span class="sxs-lookup"><span data-stu-id="d6d14-962">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-963">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-963">AppService</span></span>

* <span data-ttu-id="d6d14-964">`az appservice plan create`: Foi adicionado o suporte para definir 'persitecalling' no comando appservice plan create.</span><span class="sxs-lookup"><span data-stu-id="d6d14-964">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="d6d14-965">Foi corrigido um problema em que a operação webapp config ssl bind estava removendo as marcas existentes do recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-965">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="d6d14-966">Foi adicionado o sinalizador `--build-remote` para `az functionapp deployment source config-zip` para dar suporte à ação de build remoto durante a implantação do aplicativo de funções.</span><span class="sxs-lookup"><span data-stu-id="d6d14-966">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="d6d14-967">Foi alterada a versão do nó padrão em aplicativos de funções para ~10 para Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-967">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="d6d14-968">A propriedade `--runtime-version` foi adicionada a `az functionapp create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-968">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-969">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-969">ARM</span></span>

* <span data-ttu-id="d6d14-970">`az deployment/group deployment validate`: Foi adicionado o parâmetro `--handle-extended-json-format` para dar suporte a várias linhas e comentários no modelo JSON durante a implantação.</span><span class="sxs-lookup"><span data-stu-id="d6d14-970">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="d6d14-971">O azure-mgmt-resource passou a usar a 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-971">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-972">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-972">Backup</span></span>

* <span data-ttu-id="d6d14-973">Foi adicionado o suporte de backup aos Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-973">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-974">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-974">Compute</span></span>

* <span data-ttu-id="d6d14-975">`az vm create`: foi adicionado um aviso ao especificar a rede acelerada e um adaptador de rede existente juntos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-975">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="d6d14-976">`az vm create`: foi adicionado `--vmss` para especificar um conjunto de dimensionamento de máquinas virtuais existente ao qual a máquina virtual deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="d6d14-976">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="d6d14-977">`az vm/vmss create`: foi adicionada uma cópia local do arquivo de alias de imagem para que ele possa ser acessado em um ambiente de rede restrita.</span><span class="sxs-lookup"><span data-stu-id="d6d14-977">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="d6d14-978">`az vmss create`: foi adicionado `--orchestration-mode` para especificar como as máquinas virtuais são gerenciadas pelo conjunto de dimensionamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-978">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="d6d14-979">`az vm/vmss update`: foi adicionado `--ultra-ssd-enabled` para permitir a atualização da configuração de SSD Ultra.</span><span class="sxs-lookup"><span data-stu-id="d6d14-979">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="d6d14-980">[ALTERAÇÃO DA FALHA] `az vm extension set`: foi corrigido o bug em que os usuários não podiam definir uma extensão em uma VM com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-980">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="d6d14-981">Foram adicionados os novos comandos `az vm image terms accept/cancel/show` para gerenciar os termos de imagem do Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="d6d14-981">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="d6d14-982">O VMAccessForLinux foi atualizado para a versão 1.5</span><span class="sxs-lookup"><span data-stu-id="d6d14-982">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-983">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-983">CosmosDB</span></span>

* <span data-ttu-id="d6d14-984">[ALTERAÇÃO DA FALHA] `az sql container create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="d6d14-984">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="d6d14-985">[ALTERAÇÃO DA FALHA] `az gremlin graph create`: `--partition-key-path` foi alterado para parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="d6d14-985">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="d6d14-986">`az sql container create`: Adição de `--unique-key-policy` e `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-986">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="d6d14-987">`az sql container create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="d6d14-987">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="d6d14-988">`gremlin graph create`: Adicionado `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-988">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="d6d14-989">`gremlin graph create/update`: o esquema padrão `--idx` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="d6d14-989">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="d6d14-990">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-990">Fixed typo in help message</span></span>
* <span data-ttu-id="d6d14-991">banco de dados: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-991">database: Added deprecation information</span></span>
* <span data-ttu-id="d6d14-992">coleção: Foram adicionadas informações sobre preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-992">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-993">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-993">IoT</span></span>

* <span data-ttu-id="d6d14-994">Um novo tipo de fonte de roteamento foi adicionado: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="d6d14-994">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="d6d14-995">Foi corrigido o erro de recursos ausentes no `az iot hub create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-995">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-996">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-996">Key Vault</span></span>

* <span data-ttu-id="d6d14-997">Foi corrigido um erro inesperado quando o arquivo de certificado não existe</span><span class="sxs-lookup"><span data-stu-id="d6d14-997">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="d6d14-998">Foi corrigido o problema em que o `az keyvault recover/purge` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-998">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="d6d14-999">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="d6d14-999">NetAppFiles</span></span>

* <span data-ttu-id="d6d14-1000">O azure-mgmt-netapp foi atualizado para 0.6.0 para usar a versão da API 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1000">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="d6d14-1001">Essa nova versão da API inclui:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1001">This new API version includes:</span></span>

    - <span data-ttu-id="d6d14-1002">A criação de volume `--protocol-types` agora aceita "NFSv4.1" não "NFSv4"</span><span class="sxs-lookup"><span data-stu-id="d6d14-1002">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="d6d14-1003">A propriedade da política de exportação de volume agora é chamada 'nfsv41' não 'nfsv4'</span><span class="sxs-lookup"><span data-stu-id="d6d14-1003">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="d6d14-1004">O volume `--creation-token` foi renomeado para `--file-path`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1004">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="d6d14-1005">A data de criação do instantâneo agora é chamada apenas de 'criação'</span><span class="sxs-lookup"><span data-stu-id="d6d14-1005">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1006">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1006">Network</span></span>

* <span data-ttu-id="d6d14-1007">`az network private-dns link vnet create/update`: suporte à vinculação de rede virtual entre locatários.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1007">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="d6d14-1008">[ALTERAÇÃO DA FALHA] `az network vnet subnet list`: `--resource-group` e `--vnet-name` foram alterados para serem obrigatórios agora.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1008">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="d6d14-1009">`az network public-ip prefix create`: Suporte adicionado para especificar a versão do endereço IP (IPv4, IPv6) durante a criação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1009">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="d6d14-1010">O azure-mgmt-network foi atualizado para 7.0.0 e a api-version para 2019-09-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-1010">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="d6d14-1011">`az network vrouter`: Suporte adicionado para o novo roteador virtual de serviço e o emparelhamento do roteador virtual</span><span class="sxs-lookup"><span data-stu-id="d6d14-1011">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="d6d14-1012">`az network express-route gateway connection`: Adicionado o suporte para `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1012">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-1013">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-1013">Profile</span></span>

* <span data-ttu-id="d6d14-1014">Foi corrigido o problema em que o `az account get-access-token --resource-type ms-graph` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-1014">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="d6d14-1015">O aviso foi removido de `az login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1015">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1016">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-1016">RBAC</span></span>

* <span data-ttu-id="d6d14-1017">Foi corrigido o problema em que o `az ad app update --id {} --display-name {}` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-1017">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="d6d14-1018">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-1018">ServiceFabric</span></span>

* <span data-ttu-id="d6d14-1019">`az sf cluster create`: foi corrigido um problema que ocorria ao modificar o VMSS de computação do template.json do Linux e do Windows, do Service Fabric, de discos Standard para discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1019">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1020">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1020">SQL</span></span>

* <span data-ttu-id="d6d14-1021">Os parâmetros `--compute-model`, `--auto-pause-delay` e `--min-capacity` foram adicionados para dar suporte a operações CRUD para a nova oferta de Banco de Dados SQL: Modelo de computação sem servidor.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1021">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1022">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1022">Storage</span></span>

* <span data-ttu-id="d6d14-1023">`az storage account create/update`: Foram adicionados o parâmetro --enable-files-adds e o grupo Argumentos de Propriedades do Azure Active Directory para dar suporte à Autenticação do Serviço de Domínio do Active Directory do Arquivos do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-1023">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="d6d14-1024">O `az storage account keys list/renew` foi expandido para dar suporte à listagem ou à regeneração de chaves Kerberos da conta de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1024">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="d6d14-1025">15 de outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1025">October 15, 2019</span></span>

<span data-ttu-id="d6d14-1026">Versão 2.0.75</span><span class="sxs-lookup"><span data-stu-id="d6d14-1026">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-1027">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1027">AKS</span></span>

* <span data-ttu-id="d6d14-1028">Alteração do valor padrão `--load-balancer-sku` para `standard` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1028">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="d6d14-1029">Alteração do valor padrão `--vm-set-type` para `virtualmachinescalesets` se for compatível com a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1029">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1030">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1030">AMS</span></span>

* <span data-ttu-id="d6d14-1031">[ALTERAÇÃO SIGNIFICATIVA] Alteração do nome de `job start` para `job create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1031">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="d6d14-1032">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--ask` de `content-key-policy create` para usar uma cadeia de 32 caracteres hexadecimais em vez do UTF8</span><span class="sxs-lookup"><span data-stu-id="d6d14-1032">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1033">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1033">AppService</span></span>

* <span data-ttu-id="d6d14-1034">Adição dos comandos `webapp config access-restriction show|set|add|remove`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1034">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="d6d14-1035">Adição de um melhor tratamento de erro a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1035">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="d6d14-1036">Adição de suporte do SKU `Isolated` para `appservice plan update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1036">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-1037">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1037">ARM</span></span>

* <span data-ttu-id="d6d14-1038">Adição do parâmetro `--handle-extended-json-format``deployment create` para dar suporte a várias linhas e a comentários no modelo json</span><span class="sxs-lookup"><span data-stu-id="d6d14-1038">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-1039">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1039">Compute</span></span>

* <span data-ttu-id="d6d14-1040">Parâmetro `--enable-agent` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1040">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="d6d14-1041">Alteração de `vm create` para usar um SKU de IP público padrão automaticamente ao usar zonas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1041">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="d6d14-1042">Alteração de `vm create` para criar automaticamente um nome de computador válido para uma VM, caso nenhum tenha sido fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1042">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="d6d14-1043">Adição do parâmetro `--computer-name-prefix` a `vmss create` para dar suporte ao prefixo de nome de computador personalizado de máquinas virtuais no VMSS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1043">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="d6d14-1044">Adicione o parâmetro `--workspace` a `vm create` para habilitar o workspace de análise de logs automaticamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1044">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="d6d14-1045">Versão de API de galerias atualizadas para 2019-07-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-1045">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1046">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1046">Core</span></span>

* <span data-ttu-id="d6d14-1047">Adição da verificação de sintaxe para o parâmetro `--set` no comando de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="d6d14-1047">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-1048">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1048">IoT</span></span>

* <span data-ttu-id="d6d14-1049">Correção de um problema em que o `iot hub show` retornaria incorretamente um erro com "recurso não encontrado"</span><span class="sxs-lookup"><span data-stu-id="d6d14-1049">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1050">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1050">Monitor</span></span>

* <span data-ttu-id="d6d14-1051">Adição de suporte para CRUD a `monitor log-analytics workspace`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1051">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1052">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1052">Network</span></span>

* <span data-ttu-id="d6d14-1053">Adição de suporte para vinculação virtual entre locatários para `network private-dns link vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1053">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="d6d14-1054">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `network vnet subnet list` para exigir os parâmetros `--resource-group` e `--vnet-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1054">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1055">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1055">SQL</span></span>

* <span data-ttu-id="d6d14-1056">Adição de comandos a `sql mi ad-admin` que dão suporte à configuração de um administrador do AAD em instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1056">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1057">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1057">Storage</span></span>

* <span data-ttu-id="d6d14-1058">Adição do parâmetro `--preserve-s2s-access-tier``storage copy` para preservar a camada de acesso durante a cópia do serviço para serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-1058">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="d6d14-1059">Adição do parâmetro `--enable-large-file-share` a `storage account [create|update]` para dar suporte a compartilhamentos de arquivos grandes para a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1059">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="d6d14-1060">24 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1060">September 24, 2019</span></span>

<span data-ttu-id="d6d14-1061">Versão 2.0.74</span><span class="sxs-lookup"><span data-stu-id="d6d14-1061">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1062">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1062">ACR</span></span>

* <span data-ttu-id="d6d14-1063">Inclusão de um parâmetro `--type` obrigatório em `acr config retention update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1063">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="d6d14-1064">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro renomeado `--name -n` foi alterado para `--registry -r ` para o grupo de comando `acr config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1064">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-1065">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1065">AKS</span></span>

* <span data-ttu-id="d6d14-1066">Inclusão do parâmetro `--load-balancer-sku` no comando `aks create`, o que permite criar um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1066">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="d6d14-1067">Inclusão dos parâmetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` e `--load-balancer-outbound-ip-prefixes` nos comandos `aks [create|update]`, o que permite atualizar o perfil do balanceador de carga de um cluster do AKS com SLB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1067">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="d6d14-1068">Inclusão do parâmetro `--vm-set-type` no comando `aks create`, o que permite especificar os tipos de VM de um cluster do AKS (vmas ou vmss)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1068">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-1069">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1069">ARM</span></span>

* <span data-ttu-id="d6d14-1070">Inclusão do parâmetro `--handle-extended-json-format` no comando `group deployment create` para compatibilidade com várias linhas e comentários no modelo JSON</span><span class="sxs-lookup"><span data-stu-id="d6d14-1070">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-1071">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1071">Compute</span></span>

* <span data-ttu-id="d6d14-1072">Inclusão do parâmetro `--terminate-notification-time` nos comandos `vmss [create|update]` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1072">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="d6d14-1073">Inclusão do parâmetro `--enable-terminate-notification` no comando `vmss update` para compatibilidade com a capacidade de configurar o encerramento de eventos agendados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1073">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="d6d14-1074">Inclusão dos parâmetros `--priority,`, `--eviction-policy,` e `--max-billing` nos comandos `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1074">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="d6d14-1075">Alteração de `disk create` para permitir a especificação do tamanho exato do carregamento de disco</span><span class="sxs-lookup"><span data-stu-id="d6d14-1075">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="d6d14-1076">Inclusão de compatibilidade com instantâneos incrementais para discos gerenciados para `snapshot create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1076">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-1077">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1077">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-1078">Inclusão do parâmetro `--type <key-type>` no comando `cosmosdb keys list` para mostrar a chave, as chaves somente leitura ou cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1078">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="d6d14-1079">Adicionado o comando `cosmosdb keys regenerate`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1079">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="d6d14-1080">[PRETERIDO] Comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` e `cosmosdb list-read-only-keys` preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1080">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d6d14-1081">EventGrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-1081">EventGrid</span></span>

* <span data-ttu-id="d6d14-1082">Correção do texto de ajuda do ponto de extremidade para fazer referência ao parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1082">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-1083">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1083">Key Vault</span></span>

* <span data-ttu-id="d6d14-1084">Correção do problema em que fazer logon com um locatário (`login -t`) poderia causar uma falha no `keyvault create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1084">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1085">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1085">Monitor</span></span>

* <span data-ttu-id="d6d14-1086">Correção do problema em que o caractere `:` não era permitido no argumento `--condition` para `monitor metrics alert create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1086">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="d6d14-1087">Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-1087">Policy</span></span>

* <span data-ttu-id="d6d14-1088">Inclusão de compatibilidade com a API de Política, versão de 01/06/2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1088">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="d6d14-1089">Inclusão do parâmetro `--enforcement-mode` no comando `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1089">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1090">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1090">Storage</span></span>

* <span data-ttu-id="d6d14-1091">Inclusão do parâmetro `--blob-type` no comando `az storage copy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1091">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="d6d14-1092">10 de setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1092">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1093">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1093">ACR</span></span>

* <span data-ttu-id="d6d14-1094">Adição do grupo de comandos `acr config retention` para configurar a política de retenção</span><span class="sxs-lookup"><span data-stu-id="d6d14-1094">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-1095">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1095">AKS</span></span>

* <span data-ttu-id="d6d14-1096">Adição de suporte para integração do ACR com os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1096">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="d6d14-1097">Adição do parâmetro `--attach-acr` a `aks [create|update]` para anexar um ACR a um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1097">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="d6d14-1098">Adição do parâmetro `--detach-acr` a `aks update` para desanexar o ACR de um cluster do AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1098">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-1099">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1099">ARM</span></span>

* <span data-ttu-id="d6d14-1100">Atualização para uso da versão de API 2019-05-10</span><span class="sxs-lookup"><span data-stu-id="d6d14-1100">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1101">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1101">Batch</span></span>

* <span data-ttu-id="d6d14-1102">Adição de novas definições de configuração JSON de `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1102">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="d6d14-1103">Adição de `MountConfigurations` para montagens do sistema de arquivos (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1103">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="d6d14-1104">Adição da propriedade opcional `publicIPs` a `NetworkConfiguration` para IPs públicos em pools (confira https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obter detalhes)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1104">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="d6d14-1105">Adição de suporte para galerias de imagens compartilhadas a `--image`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1105">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="d6d14-1106">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `--start-task-wait-for-success` em `batch pool create` para `true`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1106">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="d6d14-1107">[ALTERAÇÃO SIGNIFICATIVA] Alteração do valor padrão de `Scope` em `AutoUserSpecification` para sempre ser Pool (anteriormente, `Task` em nós do Windows e `Pool` em nós do Linux)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1107">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="d6d14-1108">Esse argumento só pode ser definido em uma configuração JSON com `--json-file`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1108">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1109">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1109">HDInsight</span></span>

* <span data-ttu-id="d6d14-1110">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="d6d14-1110">GA release</span></span>
* <span data-ttu-id="d6d14-1111">[ALTERAÇÃO SIGNIFICATIVA] Alteração do parâmetro `--workernode-count/-c` de `az hdinsight resize` para ser obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1111">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-1112">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1112">Key Vault</span></span>

* <span data-ttu-id="d6d14-1113">Correção do problema em que as sub-redes não podiam ser excluídas das regras da rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1113">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="d6d14-1114">Correção do problema em que sub-redes e endereços IP duplicados podiam ser adicionados às regras da rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1114">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1115">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1115">Network</span></span>

* <span data-ttu-id="d6d14-1116">Adição do parâmetro `--interval` a `network watcher flow-log` para definir o valor do intervalo de análise de tráfego</span><span class="sxs-lookup"><span data-stu-id="d6d14-1116">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="d6d14-1117">Adição de `network application-gateway identity` para gerenciar a identidade do gateway</span><span class="sxs-lookup"><span data-stu-id="d6d14-1117">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="d6d14-1118">Adição de suporte para definir a ID do Key Vault como `network application-gateway ssl-cert`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1118">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="d6d14-1119">Adicionado `network express-route peering peer-connection [show|list]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1119">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="d6d14-1120">Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-1120">Policy</span></span>

* <span data-ttu-id="d6d14-1121">Atualização para uso da versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-1121">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="d6d14-1122">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1122">August 27, 2019</span></span>

<span data-ttu-id="d6d14-1123">Versão 2.0.72</span><span class="sxs-lookup"><span data-stu-id="d6d14-1123">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1124">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1124">ACR</span></span>

* <span data-ttu-id="d6d14-1125">[ALTERAÇÃO SIGNIFICATIVA] Remoção da compatibilidade com o SKU `classic`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1125">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="d6d14-1126">Gerenciamento de API</span><span class="sxs-lookup"><span data-stu-id="d6d14-1126">API Management</span></span>

* <span data-ttu-id="d6d14-1127">[VERSÃO PRÉVIA] Adição do grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1127">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1128">AppService</span></span>

* <span data-ttu-id="d6d14-1129">Correção do problema com o comando `webapp webjob continuous start` ao especificar um slot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1129">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="d6d14-1130">Alteração de `webapp up` para detectar a pasta `env` e removê-la do arquivo usado para implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1130">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-1131">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1131">Keyvault</span></span>

* <span data-ttu-id="d6d14-1132">Correção de um bug no `keyvault secret set` que ignorava o argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1132">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1133">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1133">Network</span></span>

* <span data-ttu-id="d6d14-1134">Adição de suporte para endereços IPv6 a argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1134">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="d6d14-1135">Adição de novos comandos `network private-endpoint [create|update|list-types]` para o gerenciamento de ponto de extremidade privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1135">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="d6d14-1136">Adição do grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1136">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="d6d14-1137">Adicionados os argumentos `--private-endpoint-network-policies` e `--private-link-service-network-policies` para `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1137">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1138">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-1138">RBAC</span></span>

* <span data-ttu-id="d6d14-1139">Correção de um problema com `ad app update --homepage` em que a página inicial não era atualizada</span><span class="sxs-lookup"><span data-stu-id="d6d14-1139">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="d6d14-1140">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-1140">ServiceFabric</span></span>

* <span data-ttu-id="d6d14-1141">Adição de suporte para nomes de Key Vault grafados com maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1141">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="d6d14-1142">Correção de um problema ao usar certificados no Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1142">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="d6d14-1143">Correção de um problema com o uso de arquivos de certificado PFX</span><span class="sxs-lookup"><span data-stu-id="d6d14-1143">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="d6d14-1144">Correção de um problema com `sf cluster certificate add` quando o grupo de recursos do Key Vault não era especificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1144">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="d6d14-1145">Correção de um problema em que `sf cluster set` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-1145">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="d6d14-1146">SignalR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1146">SignalR</span></span>

* <span data-ttu-id="d6d14-1147">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1147">Added new commands:</span></span>
  * <span data-ttu-id="d6d14-1148">`signalr cors`: gerenciar CORS do SignalR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1148">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="d6d14-1149">`signalr restart`: reiniciar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1149">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="d6d14-1150">`signalr update`: atualizar um serviço do SignalR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1150">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="d6d14-1151">Adicionado o argumento `--service-mode` para `signalr create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1151">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1152">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1152">Storage</span></span>

* <span data-ttu-id="d6d14-1153">Adicionado o comando `storage account revoke-delegation-keys`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1153">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="d6d14-1154">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1154">August 13, 2019</span></span>

<span data-ttu-id="d6d14-1155">Versão 2.0.71</span><span class="sxs-lookup"><span data-stu-id="d6d14-1155">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1156">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1156">AppService</span></span>

* <span data-ttu-id="d6d14-1157">Um problema de falha de slots com os comandos `webapp webjob continuous` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1157">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1158">BotService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1158">BotService</span></span>

* <span data-ttu-id="d6d14-1159">[ALTERAÇÃO SIGNIFICATIVA] O suporte para a criação de bots SDK v3 foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1159">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="d6d14-1160">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="d6d14-1160">CognitiveServices</span></span>

* <span data-ttu-id="d6d14-1161">Adicionados os comandos `cognitiveservices account network-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1161">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-1162">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1162">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-1163">Removido o aviso ao atualizar vários locais de gravação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1163">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="d6d14-1164">Foram adicionados os comandos CRUD para o CosmosDB SQL, MongoDB, Cassandra, Gremlin e Recursos de tabela e taxa de transferência do recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1164">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1165">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1165">HDInsight</span></span>

<span data-ttu-id="d6d14-1166">Esta versão contém um grande número de alterações da falha.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1166">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="d6d14-1167">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1167">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="d6d14-1168">`--storage-default-container` renomeado para `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1168">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="d6d14-1169">`--storage-default-filesystem` renomeado para `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1169">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="d6d14-1170">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--name` de `application create` foi alterado para representar o nome do aplicativo em vez do nome do cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-1170">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="d6d14-1171">O argumento `--cluster-name` foi adicionado a `application create` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="d6d14-1171">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="d6d14-1172">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros renomeados para `application create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1172">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="d6d14-1173">`--application-type` renomeado para `--type`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1173">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="d6d14-1174">`--marketplace-identifier` renomeado para `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1174">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="d6d14-1175">`--https-endpoint-access-mode` renomeado para `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1175">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="d6d14-1176">Renomeado de `--https-endpoint-destination-port` para `--destination-port`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1176">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="d6d14-1177">[ALTERAÇÃO SIGNIFICATIVA] Parâmetros removidos para `application create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1177">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="d6d14-1178">[ALTERAÇÃO DA FALHA] Renomeado de `--target-instance-count` para `--workernode-count` para `hdinsight resize`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1178">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="d6d14-1179">[ALTERAÇÃO SIGNIFICATIVA] Todos os comandos no grupo `hdinsight script-action` foram alterados para usar o parâmetro `--name` como o nome da ação de script.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1179">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="d6d14-1180">O argumento `--cluster-name` foi adicionado a todos os comandos `hdinsight script-action` para substituir a funcionalidade `--name` antiga</span><span class="sxs-lookup"><span data-stu-id="d6d14-1180">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="d6d14-1181">[ALTERAÇÃO SIGNIFICATIVA] Renomeado de `--script-execution-id` para `--execution-id` para todos os comandos `hdinsight script-action`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1181">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="d6d14-1182">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight script-action show` renomeado para `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1182">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="d6d14-1183">[ALTERAÇÃO DA FALHA] Os parâmetros foram alterados para `hdinsight script-action execute --roles` para serem separados por espaços em vez de separados por vírgula</span><span class="sxs-lookup"><span data-stu-id="d6d14-1183">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="d6d14-1184">[ALTERAÇÃO SIGNIFICATIVA] O parâmetro `--persisted` de `hdinsight script-action list` foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1184">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="d6d14-1185">O parâmetro `hdinsight create --cluster-configurations` foi alterado para aceitar um caminho para um arquivo JSON local ou uma cadeia de caracteres JSON</span><span class="sxs-lookup"><span data-stu-id="d6d14-1185">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="d6d14-1186">Adicionado o comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1186">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="d6d14-1187">Alterado `hdinsight monitor enable --workspace` para aceitar uma ID do workspace ou nome do workspace do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-1187">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="d6d14-1188">O argumento `hdinsight monitor enable --primary-key`, que será necessário caso uma ID do workspace seja fornecida como o parâmetro, foi adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1188">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="d6d14-1189">Foram adicionados mais exemplos e atualização das descrições das mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-1189">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-1190">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1190">Interactive</span></span>

* <span data-ttu-id="d6d14-1191">Um erro no carregamento foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1191">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="d6d14-1192">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1192">Kubernetes</span></span>

* <span data-ttu-id="d6d14-1193">Alterado para usar `https` se a porta do contêiner do painel estiver usando `https`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1193">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1194">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1194">Network</span></span>

* <span data-ttu-id="d6d14-1195">O argumento `--yes` foi adicionado a `network dns record-set cname delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1195">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-1196">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-1196">Profile</span></span>

* <span data-ttu-id="d6d14-1197">O argumento `--resource-type` foi adicionado a `account get-access-token` para obter tokens de acesso de recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1197">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="d6d14-1198">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-1198">ServiceFabric</span></span>

* <span data-ttu-id="d6d14-1199">Todas as versões de sistema operacional com suporte para criação do cluster sf foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1199">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="d6d14-1200">Foi corrigido o bug de validação do certificado primário</span><span class="sxs-lookup"><span data-stu-id="d6d14-1200">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1201">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1201">Storage</span></span>

* <span data-ttu-id="d6d14-1202">Adicionado o comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1202">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="d6d14-1203">30 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1203">July 30, 2019</span></span>

<span data-ttu-id="d6d14-1204">Versão 2.0.70</span><span class="sxs-lookup"><span data-stu-id="d6d14-1204">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1205">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1205">ACR</span></span>

* <span data-ttu-id="d6d14-1206">Corrigido o problema #9952 (uma regressão no comando `acr pack build`)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1206">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="d6d14-1207">Removido o nome da imagem do construtor padrão em `acr pack build`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1207">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1208">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1208">Appservice</span></span>

* <span data-ttu-id="d6d14-1209">Alterado `webapp config ssl` para mostrar uma mensagem se um recurso não for encontrado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1209">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="d6d14-1210">Corrigido o problema em que `functionapp create` não aceita o tipo de conta de armazenamento `Standard_RAGRS`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1210">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="d6d14-1211">Corrigido um problema em que `webapp up` falharia se fosse executado usando versões mais antigas do Python</span><span class="sxs-lookup"><span data-stu-id="d6d14-1211">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1212">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1212">Network</span></span>

* <span data-ttu-id="d6d14-1213">Removido parâmetro inválido `--ids` de `network nic ip-config add` (corrige o #9861)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1213">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="d6d14-1214">Corrige o #9604.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1214">Fixes #9604.</span></span> <span data-ttu-id="d6d14-1215">Adicionado o parâmetro `--root-certs` ao `network application-gateway http-settings [create|update]` para dar suporte a certificados raiz confiáveis associados ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1215">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="d6d14-1216">Fixado argumento `--subscription` para `network dns record-set ns create` (#9965)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1216">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1217">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-1217">RBAC</span></span>

* <span data-ttu-id="d6d14-1218">Adicionado o comando `user update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1218">Added `user update` command</span></span>
* <span data-ttu-id="d6d14-1219">[PRETERIDO] Preterido `--upn-or-object-id` de comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-1219">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="d6d14-1220">Usar argumento de substituição `--id`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1220">Use replacement argument `--id`</span></span>
* <span data-ttu-id="d6d14-1221">Adicionado argumento `--id` para comandos relacionados ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-1221">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1222">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1222">SQL</span></span>

* <span data-ttu-id="d6d14-1223">Adicionados comandos de gerenciamento para chaves de instância gerenciada e protetor de TDE</span><span class="sxs-lookup"><span data-stu-id="d6d14-1223">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1224">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1224">Storage</span></span>

* <span data-ttu-id="d6d14-1225">Adicionado o comando `storage remove`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1225">Added `storage remove` command</span></span>
* <span data-ttu-id="d6d14-1226">Corrigido um problema com `storage blob update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1226">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1227">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1227">VM</span></span>

* <span data-ttu-id="d6d14-1228">Alterado `list-skus` para usar versão de API mais recente a fim de externar detalhes de zona</span><span class="sxs-lookup"><span data-stu-id="d6d14-1228">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="d6d14-1229">Alterado o padrão de `--single-placement-group` para `false` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1229">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="d6d14-1230">Adicionada a capacidade de selecionar SKUs de armazenamento ZRS para `[snapshot|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1230">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="d6d14-1231">Adicionado novo grupo de comandos `vm host` para dar suporte a hosts dedicados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1231">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="d6d14-1232">Adicionados parâmetros `--host` e `--host-group` em `vm create` para definir o host dedicado da VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1232">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="d6d14-1233">16 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1233">July 16, 2019</span></span>

<span data-ttu-id="d6d14-1234">Versão 2.0.69</span><span class="sxs-lookup"><span data-stu-id="d6d14-1234">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1235">Appservice</span></span>

* <span data-ttu-id="d6d14-1236">Os comandos `webapp identity` foram alterados para retornar uma mensagem de erro apropriada se o nome do aplicativo ou ResourceGroupName for inválido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1236">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="d6d14-1237">`webapp list` corrigido para retornar o valor correto para numberOfSites se nenhum ResourceGroup foi fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1237">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="d6d14-1238">Corrigidos os efeitos colaterais de `appservice plan create` e `webapp create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1238">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1239">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1239">Core</span></span>

* <span data-ttu-id="d6d14-1240">Corrigido um problema em que `--subscription` aparecia apesar de não ser aplicável</span><span class="sxs-lookup"><span data-stu-id="d6d14-1240">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1241">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1241">Batch</span></span>

* <span data-ttu-id="d6d14-1242">[ALTERAÇÃO SIGNIFICATIVA]`batch pool node-agent-skus list` foi substituído por `batch pool supported-images list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1242">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="d6d14-1243">Adicionado suporte para regras de segurança bloqueando o acesso de rede a um pool com base na porta de origem do tráfego ao usar a opção `--json-file` de `batch pool create network`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1243">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="d6d14-1244">Suporte adicionado para executar a tarefa no diretório de trabalho de contêiner ou no diretório de trabalho de tarefa em lotes ao usar a opção `--json-file` de `batch task create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1244">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="d6d14-1245">Corrigido o erro na opção `--application-package-references` de `batch pool create` em que ela funcionaria apenas com padrões</span><span class="sxs-lookup"><span data-stu-id="d6d14-1245">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d6d14-1246">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1246">Eventhubs</span></span>

* <span data-ttu-id="d6d14-1247">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1247">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1248">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1248">RDBMS</span></span>

* <span data-ttu-id="d6d14-1249">Adicionado um parâmetro opcional para especificar a réplica de SKU para criar o comando de réplica</span><span class="sxs-lookup"><span data-stu-id="d6d14-1249">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="d6d14-1250">Corrigido o problema com a falha no teste de CI com a criação de réplica de MySQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1250">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="d6d14-1251">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1251">Relay</span></span>

* <span data-ttu-id="d6d14-1252">Corrigido o problema com a conexão híbrida quando a autorização do cliente desabilitava [#8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1252">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="d6d14-1253">Parâmetro `--requires-transport-security` adicionado a `relay wcfrelay create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1253">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="d6d14-1254">Barramento de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-1254">Servicebus</span></span>

* <span data-ttu-id="d6d14-1255">Adicionada validação para o parâmetro `--rights` dos comandos `authorizationrule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1255">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1256">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1256">Storage</span></span>

* <span data-ttu-id="d6d14-1257">Habilitar AADDS de arquivos para atualização da conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1257">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="d6d14-1258">Problema corrigido `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1258">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="d6d14-1259">2 de julho de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1259">July 2, 2019</span></span>

<span data-ttu-id="d6d14-1260">Versão 2.0.68</span><span class="sxs-lookup"><span data-stu-id="d6d14-1260">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1261">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1261">Core</span></span>

* <span data-ttu-id="d6d14-1262">Agora, os módulos de comando são consolidados em um único Python distribuível.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1262">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="d6d14-1263">Isso substitui o uso direto de muitos pacotes `azure-cli-` no PyPI.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1263">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="d6d14-1264">Assim, o tamanho da instalação será reduzido e apenas os usuários que tiverem instalado diretamente por meio do `pip` serão afetados.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1264">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1265">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1265">ACR</span></span>

* <span data-ttu-id="d6d14-1266">Foi adicionado o suporte para gatilhos de temporizador para tarefa</span><span class="sxs-lookup"><span data-stu-id="d6d14-1266">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1267">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1267">Appservice</span></span>

* <span data-ttu-id="d6d14-1268">O `functionapp create` foi alterado para habilitar o Application Insights por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1268">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="d6d14-1269">[ALTERAÇÃO SIGNIFICATIVA] Foi removido o comando `functionapp devops-build` preterido.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1269">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="d6d14-1270">Agora, use o novo comando `az functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1270">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="d6d14-1271">Foi adicionado o suporte ao plano de aplicativo de funções Consumo em Linux ao `functionapp deployment config-zip`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1271">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-1272">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1272">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-1273">Foi adicionado o suporte para desabilitar a TTL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1273">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="d6d14-1274">DLS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1274">DLS</span></span>

* <span data-ttu-id="d6d14-1275">Versão atualizada do ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1275">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="d6d14-1276">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6d14-1276">Feedback</span></span>

* <span data-ttu-id="d6d14-1277">Ao relatar um comando de extensão com falha, agora, o `az feedback` tenta abrir o navegador na URL do projeto/repositório da extensão por meio do índice</span><span class="sxs-lookup"><span data-stu-id="d6d14-1277">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1278">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1278">HDInsight</span></span>

* <span data-ttu-id="d6d14-1279">[ALTERAÇÃO SIGNIFICATIVA] O nome do grupo de comandos `oms` foi alterado para `monitor`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1279">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="d6d14-1280">[ALTERAÇÃO SIGNIFICATIVA]`--http-password/-p` tornou-se um parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="d6d14-1280">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="d6d14-1281">Foram adicionados preenchedores para o preenchedor dos parâmetros `--cluster-admin-account` e `cluster-users-group-dns`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1281">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="d6d14-1282">O parâmetro `cluster-users-group-dns` foi alterado para ser obrigatório quando `—esp` estiver presente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1282">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="d6d14-1283">Foi adicionado um tempo limite para todos os preenchedores automáticos de argumento existentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1283">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="d6d14-1284">Foi adicionado um tempo limite para transformar o nome do recurso na ID de recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1284">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="d6d14-1285">Os preenchedores automáticos foram alterados para selecionar recursos de qualquer grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1285">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="d6d14-1286">Pode ser um grupo de recursos diferente daquele especificado com `-g`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1286">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="d6d14-1287">Foi adicionado o suporte para os parâmetros `--sub-domain-suffix` e `--disable_gateway_auth` no comando `hdinsight application create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1287">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="d6d14-1288">Serviços gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1288">Managed Services</span></span>

* <span data-ttu-id="d6d14-1289">Introdução ao módulo de comando de serviço gerenciado em versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-1289">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-1290">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-1290">Profile</span></span>
* <span data-ttu-id="d6d14-1291">Suprimir o argumento `--subscription` para o comando de logoff</span><span class="sxs-lookup"><span data-stu-id="d6d14-1291">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1292">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-1292">RBAC</span></span>

* <span data-ttu-id="d6d14-1293">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--password` foi removido de `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1293">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="d6d14-1294">Foi adicionado o parâmetro `--assignee-principal-type` ao comando `create` para evitar falhas intermitentes causadas pela latência de replicação do servidor do AAD Graph</span><span class="sxs-lookup"><span data-stu-id="d6d14-1294">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="d6d14-1295">Foi corrigida uma falha em `ad signed-in-user` ao listar objetos de propriedade</span><span class="sxs-lookup"><span data-stu-id="d6d14-1295">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="d6d14-1296">Foi corrigido um problema em que o `ad sp` não localizava o aplicativo certo de uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-1296">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1297">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1297">RDBMS</span></span>

* <span data-ttu-id="d6d14-1298">Foi adicionado o suporte à replicação para o MariaDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1298">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1299">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1299">SQL</span></span>

* <span data-ttu-id="d6d14-1300">Valores permitidos documentados para `sql db create --sample-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1300">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1301">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1301">Storage</span></span>

* <span data-ttu-id="d6d14-1302">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1302">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="d6d14-1303">Foi adicionado o suporte ao token SAS de delegação de usuário com `--as-user` para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1303">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="d6d14-1304">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1304">VM</span></span>

* <span data-ttu-id="d6d14-1305">Foi corrigido o bug em que o `vmss create` retornava uma mensagem de erro quando era executado com `--no-wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1305">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="d6d14-1306">Foi removida a validação do lado do cliente de `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1306">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="d6d14-1307">Não falha quando `--single-placement-group` é definido como `true` e `--instance-count` é maior que 100 ou quando são especificadas zonas de disponibilidade, mas deixa essa validação para o serviço de computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1307">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="d6d14-1308">Foi corrigido o bug em que o `[vm|vmss] extension image list` falhava quando era usado com `--latest`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1308">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="d6d14-1309">18 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1309">June 18, 2019</span></span>

<span data-ttu-id="d6d14-1310">Versão 2.0.67</span><span class="sxs-lookup"><span data-stu-id="d6d14-1310">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1311">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1311">Core</span></span>

<span data-ttu-id="d6d14-1312">Esta versão apresenta uma nova marca [Versão prévia] para comunicar com mais clareza aos clientes quando um comando, um grupo de comandos ou um argumento está no status de versão prévia.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1312">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="d6d14-1313">Anteriormente, essa informação era transmitida no texto de ajuda ou, implicitamente, pelo número da versão do módulo de comando.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1313">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="d6d14-1314">A CLI removerá os números de versão dos pacotes individuais no futuro.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1314">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="d6d14-1315">Se um comando estiver em versão prévia, todos os seus argumentos também estarão.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1315">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="d6d14-1316">Se um grupo de comandos for rotulado com o status de versão prévia, então todos os seus comandos e argumentos também serão considerados em versão prévia.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1316">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="d6d14-1317">Como resultado dessa alteração, diversos grupos de comandos podem parecer surgir "de repente" com o status de versão prévia com esta liberação.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1317">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="d6d14-1318">O que realmente aconteceu é que a maioria dos pacotes já estava com status de versão prévia, mas estão sendo consideradas GA com esta liberação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1318">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1319">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1319">ACR</span></span>
* <span data-ttu-id="d6d14-1320">Adicionado o comando 'acr check-health'</span><span class="sxs-lookup"><span data-stu-id="d6d14-1320">Added 'acr check-health' command</span></span>
* <span data-ttu-id="d6d14-1321">Melhorado o tratamento de erro para tokens do AAD e para recuperar comandos externos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1321">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1322">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1322">ACS</span></span>
* <span data-ttu-id="d6d14-1323">Comandos preteridos do ACS agora ficam ocultos da exibição da ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-1323">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1324">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1324">AMS</span></span>
* <span data-ttu-id="d6d14-1325">[ALTERAÇÃO SIGNIFICATIVA] Alterada para retornar cadeias de caracteres de tempo da ISO 8601 para archive-window-length e key-frame-interval-duration</span><span class="sxs-lookup"><span data-stu-id="d6d14-1325">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1326">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1326">AppService</span></span>
* <span data-ttu-id="d6d14-1327">Adicionado roteamento com base no local para `webapp deleted list` e `webapp deleted restore`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1327">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="d6d14-1328">Corrigido problema em que a URL de destino registrada do webapp ("Não é possível iniciar o aplicativo em...") não era clicável no Azure Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d6d14-1328">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="d6d14-1329">Corrigido um problema em que a criação de aplicativos com algumas SKUs falhava com um erro de AlwaysOn</span><span class="sxs-lookup"><span data-stu-id="d6d14-1329">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="d6d14-1330">Adicionada a pré-validação para o `[appservice|webapp] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1330">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="d6d14-1331">Corrigido o `[webapp|functionapp] traffic-routing` para usar o actionHostName correto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1331">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="d6d14-1332">Adicionado o suporte de slot para comandos `functionapp`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1332">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1333">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1333">Batch</span></span>
* <span data-ttu-id="d6d14-1334">Corrigida a regressão de autenticação do AAD causada pela geração de relatórios de erros superagressiva para autenticação de chave compartilhada</span><span class="sxs-lookup"><span data-stu-id="d6d14-1334">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-1335">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d6d14-1335">BatchAI</span></span>
* <span data-ttu-id="d6d14-1336">Agora os comandos do BatchAI estão preteridos e ocultos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1336">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1337">BotService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1337">BotService</span></span>
* <span data-ttu-id="d6d14-1338">Adição das mensagens de aviso "suporte descontinuado"/"modo de manutenção" para os comandos compatíveis com a v3 do SDK</span><span class="sxs-lookup"><span data-stu-id="d6d14-1338">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-1339">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1339">CosmosDB</span></span>
* <span data-ttu-id="d6d14-1340">[PRETERIDO] Preterido o comando `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1340">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="d6d14-1341">Adicionado o comando `cosmosdb keys list` – substitui o `cosmosdb list-keys`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1341">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="d6d14-1342">`cosmsodb create/update`: Adicionado novo formato para --location a fim de permitir a configuração da propriedade "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="d6d14-1342">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="d6d14-1343">Formato antigo preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1343">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d6d14-1344">EventGrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-1344">EventGrid</span></span>
* <span data-ttu-id="d6d14-1345">Adicionados comandos do `eventgrid domain` para operações de CRUD no domínio</span><span class="sxs-lookup"><span data-stu-id="d6d14-1345">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="d6d14-1346">Adicionados comandos do `eventgrid domain topic` para operações de CRUD nos tópicos do domínio</span><span class="sxs-lookup"><span data-stu-id="d6d14-1346">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="d6d14-1347">Adicionado argumento do `--odata-query` ao `eventgrid [topic|event-subscription] list` para filtrar os resultados usando a sintaxe do OData</span><span class="sxs-lookup"><span data-stu-id="d6d14-1347">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="d6d14-1348">`event-subscription create/update`: Adicionado o servicebusqueue como novos valores para o parâmetro `--endpoint-type`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1348">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="d6d14-1349">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para `--included-event-types All` com `eventgrid event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1349">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1350">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1350">HDInsight</span></span>
* <span data-ttu-id="d6d14-1351">Adicionado suporte para o parâmetro `--ssh-public-key` no comando `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1351">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-1352">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1352">IoT</span></span>
* <span data-ttu-id="d6d14-1353">Adicionado suporte para regenerar as chaves da política de autorização</span><span class="sxs-lookup"><span data-stu-id="d6d14-1353">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="d6d14-1354">Adicionados SDK e suporte para o serviço de provisionamento de repositórios do DigitalTwin</span><span class="sxs-lookup"><span data-stu-id="d6d14-1354">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1355">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1355">Network</span></span>
* <span data-ttu-id="d6d14-1356">Adicionado suporte de zona para o Gateway da NAT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1356">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="d6d14-1357">Adicionado o comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1357">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="d6d14-1358">Corrigido o problema com o `dns zone import` em que os usuários não conseguiam importar registros do curinga A</span><span class="sxs-lookup"><span data-stu-id="d6d14-1358">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="d6d14-1359">Corrigido o problema com o `watcher flow-log configure` em que o registro de fluxo não podia ser habilitado em determinadas regiões</span><span class="sxs-lookup"><span data-stu-id="d6d14-1359">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1360">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1360">Resource</span></span>
* <span data-ttu-id="d6d14-1361">Adicionado o comando do `az rest` para fazer chamadas REST</span><span class="sxs-lookup"><span data-stu-id="d6d14-1361">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="d6d14-1362">Corrigido o erro ao usar o `policy assignment list` com um grupo de recursos ou o nível de assinatura `--scope`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1362">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="d6d14-1363">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d6d14-1363">ServiceBus</span></span>
* <span data-ttu-id="d6d14-1364">Corrigido o problema com o `servicebus topic create --max-size`[nº9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1364">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1365">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1365">SQL</span></span>
* <span data-ttu-id="d6d14-1366">Alterado o `--location` para ser opcional para `sql [server|mi] create` – usa o local do grupo de recursos se não especificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1366">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="d6d14-1367">Corrigido o erro "objeto 'NoneType' não é iterável" para `sql db list-editions --available`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1367">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="d6d14-1368">SQLVm</span><span class="sxs-lookup"><span data-stu-id="d6d14-1368">SQLVm</span></span>
* <span data-ttu-id="d6d14-1369">[ALTERAÇÃO DA FALHA] Alterado `sql vm create` para exigir o parâmetro `--license-type`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1369">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="d6d14-1370">Alterado para permitir a configuração da SKU da imagem do SQL ao criar ou atualizar uma VM do SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1370">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1371">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1371">Storage</span></span>
* <span data-ttu-id="d6d14-1372">Corrigido o problema com a chave de conta ignorada para `storage container generate-sas`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1372">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="d6d14-1373">Corrigido o problema com o `storage blob sync` no Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-1373">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1374">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1374">VM</span></span>
* <span data-ttu-id="d6d14-1375">[VERSÃO PRÉVIA] Adicionados os comandos `vm image template` para criar imagens de VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1375">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="d6d14-1376">4 de junho de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1376">June 4, 2019</span></span>

<span data-ttu-id="d6d14-1377">Versão 2.0.66</span><span class="sxs-lookup"><span data-stu-id="d6d14-1377">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1378">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1378">Core</span></span>
* <span data-ttu-id="d6d14-1379">Foi corrigido o bug em que os comandos falhavam quando `--output yaml` era usado com `--query`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1379">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1380">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1380">ACR</span></span>
* <span data-ttu-id="d6d14-1381">Foi adicionado o grupo de comando 'pack acr' para a criação de Tarefas de build rápida usando Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1381">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1382">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1382">ACS</span></span>
* <span data-ttu-id="d6d14-1383">Permitir a opção de habilitar/desabilitar o complemento kube-dashboard do AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1383">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="d6d14-1384">Imprimir uma mensagem amigável quando a assinatura não estiver na lista de permissões para usar o Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-1384">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1385">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1385">Batch</span></span>
* <span data-ttu-id="d6d14-1386">Melhoria no tratamento de erro quando você não está conectado a uma conta \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span><span class="sxs-lookup"><span data-stu-id="d6d14-1386">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-1387">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1387">IoT</span></span>
* <span data-ttu-id="d6d14-1388">Foi adicionado o suporte para failover manual</span><span class="sxs-lookup"><span data-stu-id="d6d14-1388">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1389">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1389">Network</span></span>
* <span data-ttu-id="d6d14-1390">Foram adicionados os comandos `network application-gateway waf-policy` para oferecer suporte às regras de WAF personalizadas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1390">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="d6d14-1391">Adicionados os argumentos `--waf-policy` e `--max-capacity` para `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1391">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="d6d14-1392">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1392">Resource</span></span>
* <span data-ttu-id="d6d14-1393">Melhoria da mensagem de erro do `deployment create` quando não há nenhum TTY disponível</span><span class="sxs-lookup"><span data-stu-id="d6d14-1393">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1394">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1394">Role</span></span>
* <span data-ttu-id="d6d14-1395">O texto da Ajuda foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1395">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-1396">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1396">Compute</span></span>
* <span data-ttu-id="d6d14-1397">Foi adicionado o suporte para `vm create` para as VMs de uma imagem gerenciada com LUNs de disco de dados que não começam em 0 ou que ignoram números</span><span class="sxs-lookup"><span data-stu-id="d6d14-1397">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="d6d14-1398">21 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1398">May 21, 2019</span></span>

<span data-ttu-id="d6d14-1399">Versão 2.0.65</span><span class="sxs-lookup"><span data-stu-id="d6d14-1399">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1400">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1400">Core</span></span>
* <span data-ttu-id="d6d14-1401">Foram adicionados comentários melhores para erros de autenticação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1401">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="d6d14-1402">Corrigido um problema em que a CLI carregava extensões que não eram compatíveis com a versão do núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1402">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="d6d14-1403">Corrigido um problema com a inicialização quando `clouds.config` está corrompido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1403">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1404">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1404">ACR</span></span>
* <span data-ttu-id="d6d14-1405">Foi adicionado suporte das Identidades Gerenciadas para Tarefas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1405">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1406">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1406">ACS</span></span>
* <span data-ttu-id="d6d14-1407">Corrigido o comando `openshift create` quando usado com o cliente AAD do consumidor</span><span class="sxs-lookup"><span data-stu-id="d6d14-1407">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1408">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1408">AppService</span></span>
* <span data-ttu-id="d6d14-1409">[PRETERIDO] Preterido o comando `functionapp devops-build` – Será removido na próxima versão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1409">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="d6d14-1410">`functionapp devops-pipeline` foi alterado para buscar o log de build do Azure DevOps no modo detalhado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1410">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="d6d14-1411">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--use_local_settings` foi removido do comando `functionapp devops-pipeline` – não estava operacional</span><span class="sxs-lookup"><span data-stu-id="d6d14-1411">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="d6d14-1412">`webapp up` foi alterado para retornar uma saída JSON se `--logs` não for usado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1412">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="d6d14-1413">Foi adicionado suporte para escrever recursos padrão para a configuração local de `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1413">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="d6d14-1414">Foi adicionado suporte para `webapp up` reimplantar um aplicativo sem usar o argumento `--location`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1414">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="d6d14-1415">Corrigido um problema em que o valor do SKU gratuito não funcionava na criação do ASP do SKU gratuito do Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-1415">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1416">BotService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1416">BotService</span></span>
* <span data-ttu-id="d6d14-1417">Alterado para permitir todas as capitalizações para parâmetros `--lang` em todos os comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1417">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="d6d14-1418">Descrição atualizada do módulo de comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-1418">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-1419">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1419">Consumption</span></span>
* <span data-ttu-id="d6d14-1420">O parâmetro obrigatório ausente foi adicionado para executar `consumption usage list --billing-period-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1420">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-1421">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1421">IoT</span></span>
* <span data-ttu-id="d6d14-1422">Suporte adicionado para listar todas as chaves</span><span class="sxs-lookup"><span data-stu-id="d6d14-1422">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1423">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1423">Network</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="d6d14-1425">O argumento `--nat-gateway` foi adicionado a `network vnet subnet [create|update]` para anexar a um gateway NAT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1425">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="d6d14-1426">Corrigido o problema de `dns zone import`, em que os nomes de registro não correspondiam ao tipo de registro</span><span class="sxs-lookup"><span data-stu-id="d6d14-1426">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1427">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1427">RDBMS</span></span>
* <span data-ttu-id="d6d14-1428">Suporte a postgres e mysql adicionado para replicação geográfica</span><span class="sxs-lookup"><span data-stu-id="d6d14-1428">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1429">RBAC</span><span class="sxs-lookup"><span data-stu-id="d6d14-1429">RBAC</span></span>
* <span data-ttu-id="d6d14-1430">Adição de suporte do escopo de grupo de gerenciamento a `role assignment`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1430">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1431">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1431">Storage</span></span>
* <span data-ttu-id="d6d14-1432">`storage blob sync`: adicionar um comando de sincronização ao armazenamento de blobs</span><span class="sxs-lookup"><span data-stu-id="d6d14-1432">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="d6d14-1433">Computação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1433">Compute</span></span>
* <span data-ttu-id="d6d14-1434">`--computer-name` foi adicionado a `vm create` para configurar o nome do computador da VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1434">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="d6d14-1435">`--ssh-key-value` foi renomeado para `--ssh-key-values` para `[vm|vmss] create` – Agora, pode aceitar vários valores de chave pública ou caminhos ssh</span><span class="sxs-lookup"><span data-stu-id="d6d14-1435">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="d6d14-1436">__Observação__: Isso **não** é uma alteração da falha – `--ssh-key-value` será analisado corretamente, pois corresponde somente a `--ssh-key-values`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1436">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="d6d14-1437">O argumento `--type` de `ppg create` foi alterado para ser opcional</span><span class="sxs-lookup"><span data-stu-id="d6d14-1437">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="d6d14-1438">6 de maio de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1438">May 6, 2019</span></span>

<span data-ttu-id="d6d14-1439">Versão 2.0.64</span><span class="sxs-lookup"><span data-stu-id="d6d14-1439">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1440">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1440">ACS</span></span>
* <span data-ttu-id="d6d14-1441">[ALTERAÇÃO SIGNIFICATIVA] O sinalizador `--fqdn` foi removido dos comandos `openshift`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1441">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="d6d14-1442">Alterado para usar a versão da API do Red Hat OpenShift no Azure em disponibilidade geral</span><span class="sxs-lookup"><span data-stu-id="d6d14-1442">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="d6d14-1443">O sinalizador `customer-admin-group-id` foi adicionado a `openshift create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1443">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="d6d14-1444">[GA] `(PREVIEW)` foi removido da opção `aks create``--network-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1444">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1445">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1445">Appservice</span></span>
* <span data-ttu-id="d6d14-1446">[PRETERIDO] O comando `functionapp devops-build` foi preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1446">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="d6d14-1447">Renomeado para `functionapp devops-pipeline`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1447">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="d6d14-1448">Corrigido ao obter o nome de usuário correto para cloudshell que estava causando a falha em `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1448">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="d6d14-1449">Documentação `appservice plan --sku` atualizada para refletir o appserviceplans com suporte</span><span class="sxs-lookup"><span data-stu-id="d6d14-1449">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="d6d14-1450">Adicionado argumentos opcionais para o grupo de recursos e plano a `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1450">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="d6d14-1451">Adicionado suporte a `webapp ssh` para respeitar a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1451">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="d6d14-1452">Adicionado suporte `appserviceplan create` para a SKU gratuita do Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-1452">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="d6d14-1453">Alterado `webapp up` para ter uma suspensão de 30 segundos depois de definir appsetting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para lidar com a inicialização a frio kudu</span><span class="sxs-lookup"><span data-stu-id="d6d14-1453">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="d6d14-1454">Adicionado suporte para runtime `powershell` a `functionapp create` no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-1454">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="d6d14-1455">Adicionado o comando `create-remote-connection`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1455">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1456">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1456">Batch</span></span>
* <span data-ttu-id="d6d14-1457">Corrigido o bug no validador para as opções `--application-package-references`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1457">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1458">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1458">Botservice</span></span>
* <span data-ttu-id="d6d14-1459">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para criar um Bot de Aplicativo Web vazio por padrão (ou seja, nenhum bot será implantado no Serviço de Aplicativo)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1459">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="d6d14-1460">O sinalizador `--echo` foi adicionado ao `bot create` para usar o comportamento antigo com `-v v4`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1460">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="d6d14-1461">[ALTERAÇÃO SIGNIFICATIVA] O valor padrão de `--version` foi alterado para `v4`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1461">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="d6d14-1462">__OBSERVAÇÃO:__ `bot prepare-publish` ainda usa o padrão antigo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1462">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="d6d14-1463">[ALTERAÇÃO SIGNIFICATIVA]`--lang` foi alterado para não definir mais `Csharp` como padrão.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1463">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="d6d14-1464">Se o comando exigir `--lang` e ele não for fornecido, o comando será um erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-1464">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="d6d14-1465">[ALTERAÇÃO SIGNIFICATIVA] Os argumentos `--appid` e `--password` foram alterados para `bot create` ser obrigatório e agora podem ser criados por meio de `ad app create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1465">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="d6d14-1466">Foi adicionada validação a `--appid` e `--password`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1466">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="d6d14-1467">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4` foi alterado para não criar ou usar uma Conta de Armazenamento ou o Application Insights</span><span class="sxs-lookup"><span data-stu-id="d6d14-1467">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="d6d14-1468">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v3` foi alterado para exigir uma região em que o Application Insights está disponível</span><span class="sxs-lookup"><span data-stu-id="d6d14-1468">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="d6d14-1469">[ALTERAÇÃO SIGNIFICATIVA] O `bot update` foi alterado para afetar somente as propriedades específicas de um bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1469">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="d6d14-1470">[ALTERAÇÃO SIGNIFICATIVA] Os sinalizadores `--lang` foram alterados para aceitar `Javascript` em vez de `Node`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1470">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="d6d14-1471">[ALTERAÇÃO SIGNIFICATIVA] O `Node` foi removido como um valor `--lang` permitido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1471">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="d6d14-1472">[ALTERAÇÃO SIGNIFICATIVA] O `bot create -v v4 -k webapp` foi alterado para não definir mais `SCM_DO_BUILD_DURING_DEPLOYMENT` como verdadeiro.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1472">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="d6d14-1473">Todas as implantações por meio do Kudu atuarão de acordo com o comportamento padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1473">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="d6d14-1474">O `bot download` foi alterado para os bots sem arquivos `.bot` para criar o arquivo de configuração específico a um idioma com os valores das Configurações de Aplicativo do bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1474">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="d6d14-1475">Adicionado o suporte `Typescript` para `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1475">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="d6d14-1476">Uma mensagem de aviso foi adicionada a `bot prepare-deploy` para os bots `Javascript` e `Typescript` para quando `--code-dir` não contiver `package.json`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1476">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="d6d14-1477">O `bot prepare-deploy` foi alterado para retornar `true`, se bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1477">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="d6d14-1478">O log detalhado foi adicionado a `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1478">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="d6d14-1479">Mais regiões disponíveis do Application Insights foram adicionadas ao `az bot create -v v3`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1479">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="d6d14-1480">Configurar</span><span class="sxs-lookup"><span data-stu-id="d6d14-1480">Configure</span></span>
* <span data-ttu-id="d6d14-1481">Adicionado suporte para configurações de valor padrão do argumento baseado em pasta</span><span class="sxs-lookup"><span data-stu-id="d6d14-1481">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d6d14-1482">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1482">Eventhubs</span></span>
* <span data-ttu-id="d6d14-1483">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1483">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="d6d14-1484">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1484">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1485">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1485">Network</span></span>
* <span data-ttu-id="d6d14-1486">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--cache` foi substituído por `--defer` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1486">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="d6d14-1487">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-1487">Policy Insights</span></span>
* <span data-ttu-id="d6d14-1488">Suporte adicionado a `--expand PolicyEvaluationDetails` para detalhes de avaliação de política de consulta no recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1488">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1489">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1489">Role</span></span>
* <span data-ttu-id="d6d14-1490">[PRETERIDO] Alterado argumento ocultar '--password' `create-for-rbac` - suporte será removido em maio de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1490">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="d6d14-1491">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-1491">Service Bus</span></span>
* <span data-ttu-id="d6d14-1492">Adicionados os comandos `namespace network-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1492">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="d6d14-1493">O argumento `--default-action` foi adicionado às regras de rede de `namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1493">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="d6d14-1494">`topic [create|update]` foi fixado para permitir suporte a `--max-size` para valores de 10, 20, 40 e 80 GB com a SKU Premium</span><span class="sxs-lookup"><span data-stu-id="d6d14-1494">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1495">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1495">SQL</span></span>
* <span data-ttu-id="d6d14-1496">Adicionados os comandos `sql virtual-cluster [list|show|delete]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1496">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1497">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1497">VM</span></span>
* <span data-ttu-id="d6d14-1498">O `--protect-from-scale-in` e o `--protect-from-scale-set-actions` foram adicionados a `vmss update` para habilitar atualizações à política de proteção das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1498">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="d6d14-1499">Adicionado a `--instance-id` e `vmss update` para habilitar atualização genérica das instâncias de VM VMSS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1499">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="d6d14-1500">`--instance-id` foi adicionado a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1500">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="d6d14-1501">Adição do novo grupo de comandos `ppg` para gerenciar Grupos de Posicionamento de Proximidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-1501">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="d6d14-1502">Adicionado a `--ppg`, `[vm|vmss] create` e `vm availability-set create` para gerenciar PPGs</span><span class="sxs-lookup"><span data-stu-id="d6d14-1502">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="d6d14-1503">Parâmetro `--hyper-v-generation` adicionado a `image create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1503">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="d6d14-1504">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1504">April 23, 2019</span></span>

<span data-ttu-id="d6d14-1505">Versão 2.0.63</span><span class="sxs-lookup"><span data-stu-id="d6d14-1505">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1506">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1506">ACS</span></span>
* <span data-ttu-id="d6d14-1507">Alterado `aks get-credentials` para solicitar substituição dos valores duplicados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1507">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="d6d14-1508">Removido `(PREVIEW)` dos comandos de espaços de desenvolvimento "aks use-dev-espaces" e "aks remove-dev-espaces"</span><span class="sxs-lookup"><span data-stu-id="d6d14-1508">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1509">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1509">AMS</span></span>
* <span data-ttu-id="d6d14-1510">Corrigido o bug com a atualização de filtros de conta e de ativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1510">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1511">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1511">AppService</span></span>
* <span data-ttu-id="d6d14-1512">Adicionado suporte para o ASE e o tempo limite para `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1512">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="d6d14-1513">Adicionado suporte para o estabelecimento de CI CD em um pipeline do Azure DevOps de um repositório do Github para aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="d6d14-1513">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="d6d14-1514">Adicionado argumento `--github-pat` a `functionapp devops-build create` para aceitar o token de acesso pessoal do Github</span><span class="sxs-lookup"><span data-stu-id="d6d14-1514">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="d6d14-1515">Adicionado argumento `--github-repository` a `functionapp devops-build create` para aceitar o repositório Github que contém um código-fonte functionapp</span><span class="sxs-lookup"><span data-stu-id="d6d14-1515">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="d6d14-1516">Problema corrigido em que `az webapp up --logs` estava falhando com um erro e atualização da versão .NETCORE padrão para 2.1</span><span class="sxs-lookup"><span data-stu-id="d6d14-1516">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="d6d14-1517">Configurações de functionapp desnecessárias removidas durante a criação de um aplicativo de funções com plano de consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1517">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="d6d14-1518">Alterado `webapp up` para que a cadeia de caracteres padrão asp agora acrescente o número no final para criar um novo ASP com base nas opções de SKU</span><span class="sxs-lookup"><span data-stu-id="d6d14-1518">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="d6d14-1519">Adicionado `-b` como uma opção a `webapp up` para iniciar o aplicativo no navegador</span><span class="sxs-lookup"><span data-stu-id="d6d14-1519">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="d6d14-1520">Alterado `webapp deployment source config zip` para lidar com a variável de ambiente `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1520">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="d6d14-1521">Gerenciador de Implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1521">Deployment Manager</span></span>
* <span data-ttu-id="d6d14-1522">[VERSÃO PRÉVIA] Criar e gerenciar artefatos que dão suporte a distribuições</span><span class="sxs-lookup"><span data-stu-id="d6d14-1522">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="d6d14-1523">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-1523">Lab</span></span>
* <span data-ttu-id="d6d14-1524">Corrigido o bug que causa uma saída inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-1524">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1525">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1525">Network</span></span>
* <span data-ttu-id="d6d14-1526">Adicionada delegação de servidor de nome automática a `dns zone create` no pai durante a criação da zona filho</span><span class="sxs-lookup"><span data-stu-id="d6d14-1526">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1527">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1527">Resource</span></span>
* <span data-ttu-id="d6d14-1528">[PRETERIDO] Argumentos `--link-id`, `--target-id` e `--filter-string` preteridos de `resource link`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1528">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="d6d14-1529">Use os argumentos `--link`, `--target` e `--filter`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1529">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="d6d14-1530">Corrigido o problema em que os comandos `resource link [create|update]` não funcionavam</span><span class="sxs-lookup"><span data-stu-id="d6d14-1530">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="d6d14-1531">Corrigido um problema em que a exclusão usando uma ID de recurso poderia causar falha no erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-1531">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1532">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1532">SQL</span></span>
* <span data-ttu-id="d6d14-1533">Adicionado suporte para fuso horário personalizado nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1533">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="d6d14-1534">Alterado para permitir que o nome do pool Elástico seja usado com `sql db update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1534">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="d6d14-1535">Adicionado o suporte `--no-wait` para `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1535">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="d6d14-1536">Adicionado o comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1536">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1537">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1537">Storage</span></span>
* <span data-ttu-id="d6d14-1538">Corrigido o problema com tokens SAS com codificação dupla em `storage blob generate-sas`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1538">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1539">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1539">VM</span></span>
* <span data-ttu-id="d6d14-1540">Adicionado sinalizador `--skip-shutdown` a `vm|vmss stop` para desligar as VMs sem o desligamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1540">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="d6d14-1541">Adicionado argumento `--storage-account-type` a `sig image-version create` para definir o tipo de conta do perfil de publicação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1541">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="d6d14-1542">Adicionado argumento `--target-regions` a `sig image-version create` para permitir definir os tipos de conta de armazenamento específico da região</span><span class="sxs-lookup"><span data-stu-id="d6d14-1542">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="d6d14-1543">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1543">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1544">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1544">Core</span></span>
* <span data-ttu-id="d6d14-1545">Correção do problema em que algumas extensões mostraram uma versão do `Unknown` e não podiam ser atualizadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1545">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1546">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1546">ACR</span></span>
* <span data-ttu-id="d6d14-1547">Adição de suporte para execução de uma imagem sem contexto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1547">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1548">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1548">AMS</span></span>
* [PRETERIDO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [ALTERAÇÃO SIGNIFICATIVA]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="d6d14-1551">Adição de suporte para novos parâmetros de criptografia em `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1551">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="d6d14-1552">Adição de novo parâmetro `--filters` a `ams streaming-locator create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1552">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1553">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1553">AppService</span></span>
* <span data-ttu-id="d6d14-1554">Adicionado o suporte `--logs` para `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1554">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="d6d14-1555">Correção de problemas do comando `functionapp devops-build create` de geração de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1555">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="d6d14-1556">Melhoria do tratamento de erros e indicadores `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1556">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="d6d14-1557">[ALTERAÇÃO SIGNIFICATIVA] Remoção do sinalizador `--local-git` para o comando `devops-build`; a detecção de git local e a manipulação são obrigatórias para a criação de pipelines do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="d6d14-1557">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="d6d14-1558">Adição de suporte para a criação de planos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-1558">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="d6d14-1559">Adição da capacidade de trocar um plano sob um aplicativo de funções usando `functionapp update --plan`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1559">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="d6d14-1560">Adição de suporte para configurações de expansão de plano Premium do Azure Functions</span><span class="sxs-lookup"><span data-stu-id="d6d14-1560">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-1561">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-1561">CDN</span></span>
* <span data-ttu-id="d6d14-1562">Adição de suporte para `Microsoft_Standard` e `Standard_ChinaCdn`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1562">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="d6d14-1563">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6d14-1563">Feedback</span></span>
* <span data-ttu-id="d6d14-1564">Alteração de `feedback` para mostrar metadados em comandos executados recentemente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1564">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="d6d14-1565">Alteração de `feedback` para solicitar o auxílio do usuário no processo de criação de problema abrindo um navegador e usando um modelo de problema</span><span class="sxs-lookup"><span data-stu-id="d6d14-1565">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="d6d14-1566">Alteração do `feedback` para imprimir o corpo do problema ao executar com '--verbose'</span><span class="sxs-lookup"><span data-stu-id="d6d14-1566">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1567">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1567">Monitor</span></span>
* <span data-ttu-id="d6d14-1568">Correção de um problema em que “count” não era um valor permitido com `metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1568">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="d6d14-1569">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1569">Network</span></span>
* <span data-ttu-id="d6d14-1570">Correção do formato de tabela que não estava sendo exibido com `vnet-gateway list-bgp-peer-status`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1570">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="d6d14-1571">Adição dos comandos `list-request-headers` e `list-response-headers` para `application-gateway rewrite-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1571">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="d6d14-1572">Adição do comando `list-server-variables` para `application-gateway rewrite-rule condition`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1572">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="d6d14-1573">Correção de um problema em que a atualização do estado do link em uma porta express-route geraria uma exceção de atributo desconhecido `express-route port update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1573">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="d6d14-1574">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1574">PrivateDNS</span></span>
* <span data-ttu-id="d6d14-1575">Adição de `network private-dns` para zonas de DNS privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1575">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1576">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1576">Resource</span></span>
* <span data-ttu-id="d6d14-1577">Correção do problema com `deployment create` e `group deployment create`, em que um arquivo de parâmetros com um conjunto vazio de parâmetros não funcionaria</span><span class="sxs-lookup"><span data-stu-id="d6d14-1577">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1578">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1578">Role</span></span>
* <span data-ttu-id="d6d14-1579">Correção de `create-for-rbac` para lidar corretamente com `--years`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1579">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="d6d14-1580">[ALTERAÇÃO SIGNIFICATIVA] Alteração de `role assignment delete` para solicitar ao excluir todas as atribuições na assinatura incondicionalmente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1580">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1581">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1581">SQL</span></span>
* <span data-ttu-id="d6d14-1582">Atualização de `sql mi [create|update]` com as propriedades proxyOverride e publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="d6d14-1582">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1583">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1583">Storage</span></span>
* <span data-ttu-id="d6d14-1584">[ALTERAÇÃO SIGNIFICATIVA] Remoção do resultado de `storage blob delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1584">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="d6d14-1585">Adição de `--full-uri` a `storage blob generate-sas` para criar o URI completo para o blob com SAS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1585">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="d6d14-1586">Adição de `--file-snapshot` a `storage file copy start` para copiar arquivo do instantâneo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1586">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="d6d14-1587">Alteração de `storage blob copy cancel` para mostrar apenas o erro em vez da exceção para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="d6d14-1587">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="d6d14-1588">26 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1588">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="d6d14-1589">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1589">Core</span></span>
* <span data-ttu-id="d6d14-1590">Correção de problemas com incompatibilidade da extensão de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1590">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="d6d14-1591">Agora o tratamento de erros encaminha os clientes para a página de problemas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1591">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="d6d14-1592">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-1592">Cloud</span></span>
* <span data-ttu-id="d6d14-1593">Erro de “assinatura não encontrada” corrigido em `cloud set`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1593">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1594">ACR</span></span>
* <span data-ttu-id="d6d14-1595">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1595">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="d6d14-1596">`--auth-mode` adicionado aos comandos `acr build`, `acr run`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1596">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="d6d14-1597">Grupo de comandos “acr task credential” adicionado para gerenciar as credenciais de uma Tarefa</span><span class="sxs-lookup"><span data-stu-id="d6d14-1597">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="d6d14-1598">“--no-wait” adicionado ao comando `acr build`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1598">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1599">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1599">AppService</span></span>
* <span data-ttu-id="d6d14-1600">Bug corrigido onde `webapp up` não estava lidando corretamente com a execução do diretório vazio ou do cenário de código desconhecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1600">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="d6d14-1601">Bug corrigido onde os slots não funcionavam para `[webapp|functionapp] config ssl bind`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1601">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="d6d14-1602">Serviço de BOT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1602">BOT Service</span></span>
* <span data-ttu-id="d6d14-1603">`bot prepare-deploy` adicionado para se preparar para a implantação de bots via `webapp`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1603">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="d6d14-1604">`bot create --kind registration` alterado para mostrar a senha se ela não for fornecida</span><span class="sxs-lookup"><span data-stu-id="d6d14-1604">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="d6d14-1605">[ALTERAÇÃO SIGNIFICATIVA]`--endpoint` alterado em `bot create --kind registration` como padrão para uma cadeia de caracteres vazia, em vez de ser requerido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1605">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="d6d14-1606">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1606">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-1607">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-1607">CDN</span></span>
* <span data-ttu-id="d6d14-1608">Adicionado o suporte ao `--no-wait` para `cdn endpoint [create|update|start|stop|delete|load|purge]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1608">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* [ALTERAÇÃO SIGNIFICATIVA]: `cdn endpoint create` alterado para o comportamento de cache da cadeia de consulta padrão.
[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour. <span data-ttu-id="d6d14-1610">Não há mais padrão para "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="d6d14-1610">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="d6d14-1611">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-1611">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-1612">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="d6d14-1612">Cosmosdb</span></span>
* <span data-ttu-id="d6d14-1613">Suporte adicionado para `--enable-multiple-write-locations` na atualização da conta</span><span class="sxs-lookup"><span data-stu-id="d6d14-1613">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="d6d14-1614">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1614">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-1615">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1615">Interactive</span></span>
* <span data-ttu-id="d6d14-1616">Incompatibilidade corrigida com a extensão Interativa instalada por meio do azdev</span><span class="sxs-lookup"><span data-stu-id="d6d14-1616">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1617">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1617">Monitor</span></span>
* <span data-ttu-id="d6d14-1618">Alterado para permitir o valor de dimensão `*` para `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1618">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1619">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1619">Network</span></span>
* <span data-ttu-id="d6d14-1620">Grupo de comandos `rewrite-rule` adicionado em `application-gateway`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1620">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-1621">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-1621">Profile</span></span>
* <span data-ttu-id="d6d14-1622">Suporte de conta no nível do locatário para a identidade de serviço gerenciado adicionado em `login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1622">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="d6d14-1623">Postgres</span><span class="sxs-lookup"><span data-stu-id="d6d14-1623">Postgres</span></span> 
* <span data-ttu-id="d6d14-1624">Adicionados os comandos postgresql `replica` e `restart server`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1624">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="d6d14-1625">Alterado para obter o local padrão do grupo de recursos quando não fornecido para criar servidores e adicionar validação para os dias de retenção</span><span class="sxs-lookup"><span data-stu-id="d6d14-1625">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1626">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1626">Resource</span></span>
* <span data-ttu-id="d6d14-1627">Saída da tabela aperfeiçoada para `deployment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1627">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="d6d14-1628">Corrigido o problema com `deployment [create|validate]` onde o tipo secureObject não era reconhecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1628">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="d6d14-1629">Grafo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1629">Graph</span></span>
* <span data-ttu-id="d6d14-1630">Adicionado o suporte ao `--end-date` para `ad [app|sp] credential reset`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1630">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="d6d14-1631">Suporte adicionado para acrescentar permissões com `ad app permission add`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1631">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="d6d14-1632">Bug corrigido com `ad app permission list` quando não havia nenhuma permissão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1632">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="d6d14-1633">`ad sp delete` alterado para ignorar a exclusão da atribuição de função se a conta atual não tem nenhuma assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-1633">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="d6d14-1634">`ad app create` alterado para `--identifier-uris` passar para lista vazia como padrão se não fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1634">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1635">armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1635">storage</span></span>
* <span data-ttu-id="d6d14-1636">`--snapshot` adicionado a `storage file download-batch` para baixar de um instantâneo de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1636">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="d6d14-1637">Barra de progresso `storage blob [download-batch|upload-batch]` alterada para ser menos detalhada e indicar o blob atual</span><span class="sxs-lookup"><span data-stu-id="d6d14-1637">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="d6d14-1638">Problema corrigido com `storage account update` ao atualizar os parâmetros de criptografia</span><span class="sxs-lookup"><span data-stu-id="d6d14-1638">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="d6d14-1639">Problema corrigido onde `storage blob show` falharia ao usar o oauth (`--auth-mode=login`)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1639">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1640">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1640">VM</span></span>
* <span data-ttu-id="d6d14-1641">Adicionado o comando `image update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1641">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="d6d14-1642">12 de março de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1642">March 12, 2019</span></span>

<span data-ttu-id="d6d14-1643">Versão 2.0.60</span><span class="sxs-lookup"><span data-stu-id="d6d14-1643">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1644">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1644">Core</span></span>

* <span data-ttu-id="d6d14-1645">Foi corrigido um erro incorreto no `cloud set` sobre assinatura não encontrada.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1645">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1646">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1646">ACR</span></span>

* <span data-ttu-id="d6d14-1647">Corrigidas fontes redundantes na importação de imagem.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1647">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1648">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1648">ACS</span></span>

* <span data-ttu-id="d6d14-1649">Alteração para ignorar o parâmetro `--listen-address` para `aks browse` se ele não for compatível com kubectl</span><span class="sxs-lookup"><span data-stu-id="d6d14-1649">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="d6d14-1650">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1650">AppService</span></span>

* <span data-ttu-id="d6d14-1651">Adicionado `[webapp|functionapp] deployment list-publishing-credentials` para obter a URL de publicação do Kudu e suas credenciais.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1651">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="d6d14-1652">Removida a instrução de impressão errônea de `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1652">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="d6d14-1653">Corrigido `functionapp` para definir a imagem correta do runtime nos planos do Serviço de Aplicativo no Linux.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1653">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="d6d14-1654">Removida a marca de versão prévia do `webapp up` e adicionadas melhorias ao comando.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1654">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1655">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1655">Botservice</span></span>

* <span data-ttu-id="d6d14-1656">Adicionado `SCM_DO_BUILD_DURING_DEPLOYMENT` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1656">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="d6d14-1657">Adicionados `Microsoft-BotFramework-AppId` e `Microsoft-BotFramework-AppPassword` às Configurações de Aplicativo do modelo ARM para Bots de Aplicativo Web v4.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1657">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="d6d14-1658">Removidas as aspas simples da saída de comando `bot publish`, no final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1658">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="d6d14-1659">Alterado `bot publish` para que seja assíncrono.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1659">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-1660">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-1660">Container</span></span>

* <span data-ttu-id="d6d14-1661">Adicionado o argumento `--no-wait` para `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1661">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="d6d14-1662">EventHub</span><span class="sxs-lookup"><span data-stu-id="d6d14-1662">EventHub</span></span>

* <span data-ttu-id="d6d14-1663">Adicionado o sinalizador `--skip-empty-archives` a `eventhub create|update` para dar suporte a arquivos vazios na captura.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1663">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="d6d14-1664">Localizar</span><span class="sxs-lookup"><span data-stu-id="d6d14-1664">Find</span></span>

* <span data-ttu-id="d6d14-1665">Atualização de funcionalidade principal</span><span class="sxs-lookup"><span data-stu-id="d6d14-1665">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1666">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1666">HDInsight</span></span>

* <span data-ttu-id="d6d14-1667">Adicionado o parâmetro `--storage-account-managed-identity` a `hdinsight create` para oferecer suporte ao MSI do ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1667">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1668">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1668">Network</span></span>

* <span data-ttu-id="d6d14-1669">Corrigido o problema com `vpn-connection update`, onde a atualização de uma conexão VPN entre gateways em assinaturas diferentes falharia.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1669">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1670">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d6d14-1670">Rdbms</span></span>

* <span data-ttu-id="d6d14-1671">Correções secundárias para obter a localização padrão do grupo de recursos, quando não fornecida, para criar servidores e adicionar validação nos dias de retenção.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1671">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1672">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1672">Role</span></span>

* <span data-ttu-id="d6d14-1673">Corrigido `role definition update` para usar ID a fim de resolver a definição corretamente.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1673">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="d6d14-1674">Alterado `ad app credential reset` para remover a suposição de que a entidade de serviço do aplicativo já existe.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1674">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d6d14-1675">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-1675">Service Fabric</span></span>

* <span data-ttu-id="d6d14-1676">Corrigido o problema com o fato de `sf cluster list` não ser iterável.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1676">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="d6d14-1677">26 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1677">February 26, 2019</span></span>

<span data-ttu-id="d6d14-1678">Versão 2.0.59</span><span class="sxs-lookup"><span data-stu-id="d6d14-1678">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1679">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1679">Core</span></span>

* <span data-ttu-id="d6d14-1680">Corrigido o problema onde algumas instâncias usando `--subscription NAME` produziriam uma exceção</span><span class="sxs-lookup"><span data-stu-id="d6d14-1680">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1681">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1681">ACR</span></span>

* <span data-ttu-id="d6d14-1682">Parâmetro `--target` adicionado para os comandos `acr build`, `acr task create` e `acr task update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1682">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="d6d14-1683">Melhor tratamento de erros para os comandos de execução quando não conectado ao Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-1683">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1684">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1684">ACS</span></span>

* <span data-ttu-id="d6d14-1685">Opção `--listen-address` adicionada a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1685">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1686">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1686">AppService</span></span>

* <span data-ttu-id="d6d14-1687">Adicionado o comando `functionapp devops-build`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1687">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-1688">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-1688">Batch</span></span>
* <span data-ttu-id="d6d14-1689">[ALTERAÇÃO SIGNIFICATIVA] Comando `batch pool upgrade os` removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1689">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="d6d14-1690">[ALTERAÇÃO SIGNIFICATIVA] Propriedade `Pacakges` removida das respostas `Application`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1690">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="d6d14-1691">Comando `batch application package list` adicionado para listar os pacotes de um aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1691">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="d6d14-1692">[ALTERAÇÃO SIGNIFICATIVA]`--application-id` alterado para `--application-name` em todos os comandos `batch application`,</span><span class="sxs-lookup"><span data-stu-id="d6d14-1692">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="d6d14-1693">O argumento `--json-file` foi adicionado aos comandos para a solicitação de resposta da API bruta</span><span class="sxs-lookup"><span data-stu-id="d6d14-1693">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="d6d14-1694">Validação atualizada para incluir automaticamente `https://` em todos os pontos de extremidade, se ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1694">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-1695">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1695">CosmosDB</span></span>

* <span data-ttu-id="d6d14-1696">O subgrupo `network-rule` foi adicionado com os comandos `add`, `remove` e `list` para gerenciar as regras de VNET de uma conta do Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1696">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="d6d14-1697">Kusto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1697">Kusto</span></span>

* <span data-ttu-id="d6d14-1698">[ALTERAÇÃO SIGNIFICATIVA] Os tipos `hot_cache_period` e `soft_delete_period` foram alterados do banco de dados para o formato de duração ISO8601</span><span class="sxs-lookup"><span data-stu-id="d6d14-1698">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1699">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1699">Network</span></span>

* <span data-ttu-id="d6d14-1700">Adicionado o argumento `--express-route-gateway-bypass` para `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1700">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="d6d14-1701">Foram adicionados os grupos de comando a partir das extensões `express-route`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1701">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="d6d14-1702">Os grupos de comando `express-route gateway` e `express-route port` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1702">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="d6d14-1703">Adicionado o argumento `--legacy-mode` para `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1703">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="d6d14-1704">Os argumentos `--allow-classic-operations` e `--express-route-port` foram adicionados a `express-route [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1704">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="d6d14-1705">Adicionado o argumento `--gateway-default-site` para `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1705">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="d6d14-1706">Os comandos `ipsec-policy` foram adicionados a `vnet-gateway`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1706">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1707">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1707">Resource</span></span>

* <span data-ttu-id="d6d14-1708">Foi corrigido o problema com `deployment create` em que o campo do tipo diferencia letras maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1708">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="d6d14-1709">Foi adicionado o suporte para arquivo de parâmetros de URI a `policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1709">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="d6d14-1710">Foi adicionado o suporte para parâmetros de URI e definições a `policy set-definition update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1710">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="d6d14-1711">Foi corrigido o tratamento de parâmetros e regras para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1711">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="d6d14-1712">Foi corrigido o problema com `resource show/update/delete/tag/invoke-action` em que as IDs de assinatura cruzada não respeitaram corretamente a ID da assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-1712">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1713">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1713">Role</span></span>

* <span data-ttu-id="d6d14-1714">Foi adicionado o suporte para as funções do aplicativo a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1714">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1715">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1715">VM</span></span>

* <span data-ttu-id="d6d14-1716">Foi corrigido o problema com `vm create where ` – a rede acelerada não foi habilitada por padrão no Ubuntu 18.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-1716">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="d6d14-1717">12 de fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1717">February 12, 2019</span></span>

<span data-ttu-id="d6d14-1718">Versão 2.0.58</span><span class="sxs-lookup"><span data-stu-id="d6d14-1718">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1719">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1719">Core</span></span>

* <span data-ttu-id="d6d14-1720">`az --version` agora exibe uma notificação se você tiver pacotes para atualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-1720">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="d6d14-1721">A regressão em que `--ids` não pode ser usado com a saída JSON foi corrigida</span><span class="sxs-lookup"><span data-stu-id="d6d14-1721">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1722">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1722">ACR</span></span>
* <span data-ttu-id="d6d14-1723">[ALTERAÇÃO SIGNIFICATIVA] O grupo de comandos `acr build-task` foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1723">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="d6d14-1724">[ALTERAÇÃO SIGNIFICATIVA] As opções `--tag` e `--manifest` de `acr repository delete` foram removidas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1724">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1725">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1725">ACS</span></span>
* <span data-ttu-id="d6d14-1726">Suporte adicionado a `aks [enable-addons|disable-addons]` para nomes que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1726">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="d6d14-1727">Suporte adicionado para a operação de atualização do Azure Active Directory usando `aks update-credentials --reset-aad`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1727">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="d6d14-1728">Um esclarecimento informando que `--output` é ignorado para `aks get-credentials` foi adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1728">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1729">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1729">AMS</span></span>
* <span data-ttu-id="d6d14-1730">Adicionados os comandos `ams streaming-endpoint [start | stop | create | update] wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1730">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="d6d14-1731">Adicionados os comandos `ams live-event [create | start | stop | reset] wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1731">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1732">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1732">Appservice</span></span>
* <span data-ttu-id="d6d14-1733">Foi adicionada a capacidade de criar e configurar funções usando contêineres de ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1733">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="d6d14-1734">Suporte adicionado para a atualização das configurações de aplicativos Web por meio de JSON</span><span class="sxs-lookup"><span data-stu-id="d6d14-1734">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="d6d14-1735">A ajuda foi aprimorada para `appservice-plan-update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1735">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="d6d14-1736">Suporte adicionado para o App Insights para auxiliar na criação de aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="d6d14-1736">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="d6d14-1737">Os problemas com o SSH do aplicativo Web foram corrigidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1737">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1738">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1738">Botservice</span></span>
* <span data-ttu-id="d6d14-1739">A experiência do usuário para `bot publish` foi aprimorada</span><span class="sxs-lookup"><span data-stu-id="d6d14-1739">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="d6d14-1740">Foram adicionados avisos de tempos limite ao executar `npm install` durante `az bot publish`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1740">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="d6d14-1741">O caractere inválido `.` de `--name` em `az bot create` foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1741">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="d6d14-1742">Alteração para interromper a geração aleatória de nomes de recursos durante a criação do Armazenamento do Azure, Plano do Serviço de Aplicativo, Aplicativo Web/de funções e Application Insights</span><span class="sxs-lookup"><span data-stu-id="d6d14-1742">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="d6d14-1743">[PRETERIDO] O argumento `--proj-name` foi preterido em favor de `--proj-file-path`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1743">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="d6d14-1744">`az bot publish` foi alterado para remover arquivos de implantação do Node.js do IIS buscados, caso eles já não existissem</span><span class="sxs-lookup"><span data-stu-id="d6d14-1744">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="d6d14-1745">Foi adicionado o argumento `--keep-node-modules` para `az bot publish` para não excluir a pasta `node_modules` no Serviço de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1745">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="d6d14-1746">O par chave-valor `"publishCommand"` foi adicionado à saída de `az bot create` durante a criação de uma função do Azure ou bot de aplicativo Web</span><span class="sxs-lookup"><span data-stu-id="d6d14-1746">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="d6d14-1747">O valor de `"publishCommand"` é um comando `az bot publish` que é automaticamente preenchido com os parâmetros necessários para publicar o bot recém-criado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1747">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="d6d14-1748">O `"WEBSITE_NODE_DEFAULT_VERSION"` foi atualizado no modelo do ARM para que os bots de SDK v4 usem 10.14.1 em vez de 8.9.4</span><span class="sxs-lookup"><span data-stu-id="d6d14-1748">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-1749">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1749">Key Vault</span></span>
* <span data-ttu-id="d6d14-1750">Foi corrigido o problema com `keyvault secret backup`, em que alguns usuários recebiam um erro `unexpected_keyword` ao usar `--id`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1750">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1751">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1751">Monitor</span></span>
* <span data-ttu-id="d6d14-1752">`monitor metrics alert [create|update]` foi alterado para permitir o valor dimensional `*`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1752">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1753">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1753">Network</span></span>
* <span data-ttu-id="d6d14-1754">`dns zone export` foi alterado para garantir que CNAMEs exportados fossem FQDNs</span><span class="sxs-lookup"><span data-stu-id="d6d14-1754">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="d6d14-1755">O parâmetro `--gateway-name` foi adicionado a `nic ip-config address-pool [add|remove]` para dar suporte a pools de endereços de back-end de gateway de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1755">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="d6d14-1756">Os argumentos `--traffic-analytics` e `--workspace` foram adicionados a `network watcher flow-log configure` para dar suporte à análise de tráfego por meio de um espaço de trabalho do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-1756">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="d6d14-1757">`--idle-timeout` e `--floating-ip` foram adicionados a `lb inbound-nat-pool [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1757">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d6d14-1758">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-1758">Policy Insights</span></span>
* <span data-ttu-id="d6d14-1759">Os comandos `policy remediation` foram adicionados para dar suporte a recursos de correção de política de recursos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1759">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1760">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1760">RDBMS</span></span>
* <span data-ttu-id="d6d14-1761">A mensagem e os parâmetros de comando de ajuda foram aprimorados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1761">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-1762">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-1762">Redis</span></span>
* <span data-ttu-id="d6d14-1763">Foram adicionados comandos para gerenciar regras de firewall (criar, atualizar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1763">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="d6d14-1764">Foram adicionados comandos para gerenciar links do servidor (criar, excluir, mostrar, listar)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1764">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="d6d14-1765">Foram adicionados comandos para gerenciar o agendamento de patches (criar, atualizar, excluir, mostrar)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1765">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="d6d14-1766">Suporte adicionado para Zonas de Disponibilidade e versão mínima de TLS para criar Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-1766">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="d6d14-1767">[ALTERAÇÃO SIGNIFICATIVA] Os comandos `redis update-settings` e `redis list-all` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1767">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="d6d14-1768">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro para `redis create`: “configurações de locatário” não é aceito no formato chave[=valor]</span><span class="sxs-lookup"><span data-stu-id="d6d14-1768">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="d6d14-1769">[PRETERIDO] Uma mensagem de aviso foi adicionada para preterir o comando `redis import-method`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1769">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1770">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1770">Role</span></span>
* <span data-ttu-id="d6d14-1771">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido dos comandos `vm` para esta localização</span><span class="sxs-lookup"><span data-stu-id="d6d14-1771">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="d6d14-1772">SQL VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1772">SQL VM</span></span>
* <span data-ttu-id="d6d14-1773">[PRETERIDO] O argumento `--boostrap-acc-pwd` foi preterido devido a um erro de digitação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1773">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1774">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1774">VM</span></span>
* <span data-ttu-id="d6d14-1775">`vm list-skus` foi alterado para permitir o uso de `--all` no lugar de `--all true`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1775">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="d6d14-1776">Adicionado `vmss run-command [invoke | list | show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1776">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="d6d14-1777">Foi corrigido o bug em que `vmss encryption enable` falhava se fosse executado anteriormente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1777">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="d6d14-1778">[ALTERAÇÃO SIGNIFICATIVA] O comando `az identity` foi movido para os comandos `role`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1778">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="d6d14-1779">31 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1779">January 31, 2019</span></span>

<span data-ttu-id="d6d14-1780">Versão 2.0.57</span><span class="sxs-lookup"><span data-stu-id="d6d14-1780">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1781">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1781">Core</span></span>

* <span data-ttu-id="d6d14-1782">Hotfix para o [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="d6d14-1782">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="d6d14-1783">28 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1783">January 28, 2019</span></span>

<span data-ttu-id="d6d14-1784">Versão 2.0.56</span><span class="sxs-lookup"><span data-stu-id="d6d14-1784">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1785">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1785">ACR</span></span>
* <span data-ttu-id="d6d14-1786">Suporte adicionado para regras de rede virtual/IP</span><span class="sxs-lookup"><span data-stu-id="d6d14-1786">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1787">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1787">ACS</span></span>
* <span data-ttu-id="d6d14-1788">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="d6d14-1788">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="d6d14-1789">Comandos do OpenShift gerenciado foram adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1789">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="d6d14-1790">Suporte adicionado para operações de atualização da entidade de serviço com `aks update-credentials -reset-service-principal`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1790">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-1791">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1791">AMS</span></span>
* <span data-ttu-id="d6d14-1792">[ALTERAÇÃO SIGNIFICATIVA]`ams asset get-streaming-locators` renomeado para `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1792">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="d6d14-1793">[ALTERAÇÃO SIGNIFICATIVA]`ams streaming-locator get-content-keys` renomeado para `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1793">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1794">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1794">Appservice</span></span>
* <span data-ttu-id="d6d14-1795">Suporte adicionado para o App Insights no `functionapp create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1795">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="d6d14-1796">Suporte adicionado para a criação do plano de serviço de aplicativo (incluindo Elástico Premium) para Aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="d6d14-1796">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="d6d14-1797">Foram corrigidos os problemas com de configuração de aplicativo com os planos Elástico Premium</span><span class="sxs-lookup"><span data-stu-id="d6d14-1797">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-1798">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-1798">Container</span></span>
* <span data-ttu-id="d6d14-1799">Adicionado o comando `container start`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1799">Added `container start` command</span></span>
* <span data-ttu-id="d6d14-1800">Alteração para permitir o uso de valores decimais para CPU durante a criação do contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-1800">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d6d14-1801">EventGrid</span><span class="sxs-lookup"><span data-stu-id="d6d14-1801">EventGrid</span></span>
* <span data-ttu-id="d6d14-1802">Parâmetro `--deadletter-endpoint` adicionado a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1802">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="d6d14-1803">Storagequeue e hybridconnection foram adicionados como novos valores para 'event-subscription [create|update] --endpoint-type\`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1803">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="d6d14-1804">Os parâmetros `--max-delivery-attempts` e `--event-ttl` foram adicionados a `event-subscription create` para especificar a política de repetição para eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1804">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="d6d14-1805">Uma mensagem de aviso foi adicionada a `event-subscription [create|update]` quando o webhook como destino for usado para uma assinatura de evento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1805">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="d6d14-1806">O parâmetro source-resource-id foi adicionado para todos os comandos relacionados a eventos e marcar todos os outros parâmetros relacionados ao recurso de origem como preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1806">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1807">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1807">HDInsight</span></span>
* <span data-ttu-id="d6d14-1808">[ALTERAÇÃO SIGNIFICATIVA] Os parâmetros `--virtual-network` e `--subnet-name` de `hdinsight [application] create` foram removidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1808">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="d6d14-1809">[ALTERAÇÃO SIGNIFICATIVA]`hdinsight create --storage-account` foi alterado para aceitar o nome ou ID da conta de armazenamento, em vez de pontos de extremidade de blob</span><span class="sxs-lookup"><span data-stu-id="d6d14-1809">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="d6d14-1810">Parâmetros `--vnet-name` e `--subnet-name` adicionados a `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1810">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="d6d14-1811">Suporte adicionado para a criptografia de disco e Enterprise Security Package ao `hdinsight create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1811">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="d6d14-1812">Adicionado o comando `hdinsight rotate-disk-encryption-key`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1812">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="d6d14-1813">Adicionado o comando `hdinsight update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1813">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-1814">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-1814">IoT</span></span>
* <span data-ttu-id="d6d14-1815">O formato de codificação foi adicionado ao comando routing-endpoint</span><span class="sxs-lookup"><span data-stu-id="d6d14-1815">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="d6d14-1816">Kusto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1816">Kusto</span></span>
* <span data-ttu-id="d6d14-1817">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-1817">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-1818">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1818">Monitor</span></span>
* <span data-ttu-id="d6d14-1819">A comparação de ID foi alterada para diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1819">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-1820">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-1820">Profile</span></span>
* <span data-ttu-id="d6d14-1821">A conta de nível de locatário foi habilitada para a identidade de serviço gerenciada de `login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1821">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1822">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1822">Network</span></span>
* <span data-ttu-id="d6d14-1823">Foi corrigido o problema com `express-route update`: em que o argumento `--bandwidth` era ignorado</span><span class="sxs-lookup"><span data-stu-id="d6d14-1823">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="d6d14-1824">Foi corrigido o problema com `ddos-protection update` em que definir a compreensão levava ao rastreamento de pilha</span><span class="sxs-lookup"><span data-stu-id="d6d14-1824">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1825">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1825">Resource</span></span>
* <span data-ttu-id="d6d14-1826">Suporte adicionado para o arquivo de parâmetros de URI à `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1826">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="d6d14-1827">Suporte adicionado para a identidade gerenciada à `policy assignment [create|list|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1827">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="d6d14-1828">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1828">SQL Virtual Machine</span></span>
* <span data-ttu-id="d6d14-1829">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-1829">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1830">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1830">Storage</span></span>
* <span data-ttu-id="d6d14-1831">Alteração na correção para atualizar apenas as propriedades que são alteradas no mesmo objeto</span><span class="sxs-lookup"><span data-stu-id="d6d14-1831">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="d6d14-1832">#8021 foi corrigido, dados binários são codificados em base 64 quando retornados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1832">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1833">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1833">VM</span></span>
* <span data-ttu-id="d6d14-1834">Alteração de `vm encryption enable` para validar o cofre de chaves de criptografia de disco e se esse cofre de chaves de criptografia de chave existe</span><span class="sxs-lookup"><span data-stu-id="d6d14-1834">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="d6d14-1835">O sinalizador `--force` foi adicionado a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1835">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="d6d14-1836">15 de janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="d6d14-1836">January 15, 2019</span></span>

<span data-ttu-id="d6d14-1837">Versão 2.0.55</span><span class="sxs-lookup"><span data-stu-id="d6d14-1837">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1838">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1838">ACR</span></span>
* <span data-ttu-id="d6d14-1839">Alteração para permitir forçar o envio por push de um gráfico Helm que não existe</span><span class="sxs-lookup"><span data-stu-id="d6d14-1839">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="d6d14-1840">Alteração para permitir operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1840">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="d6d14-1841">[PRETERIDO] O parâmetro `--resource-group` foi preterido nos comandos:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1841">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="d6d14-1842">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1842">ACS</span></span>
* <span data-ttu-id="d6d14-1843">Suporte adicionado para novas regiões ACI</span><span class="sxs-lookup"><span data-stu-id="d6d14-1843">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1844">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1844">Appservice</span></span>
* <span data-ttu-id="d6d14-1845">Foi corrigido o problema com o carregamento de certificados para aplicativos que são hospedados em um ASE, em que o RG do ASE e o RG do aplicativo são diferentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1845">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="d6d14-1846">Alteração de `webapp up` para usar a SKU P1V1 como padrão para Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-1846">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="d6d14-1847">`[webapp|functionapp] deployment source config-zip` foi corrigido para mostrar a mensagem de erro adequada quando uma implantação falhar</span><span class="sxs-lookup"><span data-stu-id="d6d14-1847">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="d6d14-1848">Adicionado o comando `webapp ssh`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1848">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1849">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1849">Botservice</span></span>
* <span data-ttu-id="d6d14-1850">Atualizações de status de implantação foram adicionadas a `bot create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1850">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="d6d14-1851">Configurar</span><span class="sxs-lookup"><span data-stu-id="d6d14-1851">Configure</span></span>
* <span data-ttu-id="d6d14-1852">`none` foi adicionado como um formato de saída configurável</span><span class="sxs-lookup"><span data-stu-id="d6d14-1852">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-1853">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1853">CosmosDB</span></span>
* <span data-ttu-id="d6d14-1854">Suporte adicionado para criar o banco de dados com taxa de transferência compartilhada</span><span class="sxs-lookup"><span data-stu-id="d6d14-1854">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-1855">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-1855">HDInsight</span></span>
* <span data-ttu-id="d6d14-1856">Foram adicionados comandos para o gerenciamento de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1856">Added commands for managing applications</span></span>
* <span data-ttu-id="d6d14-1857">Foram adicionados comandos para o gerenciamento de ações de script</span><span class="sxs-lookup"><span data-stu-id="d6d14-1857">Added commands for managing script actions</span></span>
* <span data-ttu-id="d6d14-1858">Foram adicionados comandos para o gerenciamento do Operations Management Suite (OMS)</span><span class="sxs-lookup"><span data-stu-id="d6d14-1858">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="d6d14-1859">Suporte adicionado para listar a utilização regional ao `hdinsight list-usage`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1859">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="d6d14-1860">[ALTERAÇÃO SIGNIFICATIVA] O tipo de cluster padrão de `hdinsight create` foi removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1860">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1861">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1861">Network</span></span>
* <span data-ttu-id="d6d14-1862">Adicionados os argumentos `--custom-headers` e `--status-code-ranges` para `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1862">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="d6d14-1863">Novos tipos de roteamento foram adicionados: Subrede e múltiplos valores</span><span class="sxs-lookup"><span data-stu-id="d6d14-1863">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="d6d14-1864">Adicionados os argumentos `--custom-headers` e `--subnets` para `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1864">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="d6d14-1865">Foi corrigido o problema no qual fornecer `--vnets ""` a `ddos-protection update` causava um erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-1865">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1866">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1866">Role</span></span>
* <span data-ttu-id="d6d14-1867">[PRETERIDO] O argumento `--password` foi preterido para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1867">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="d6d14-1868">Como alternativa, use senhas seguras geradas pela CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-1868">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="d6d14-1869">Segurança</span><span class="sxs-lookup"><span data-stu-id="d6d14-1869">Security</span></span>
* <span data-ttu-id="d6d14-1870">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-1870">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1871">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1871">Storage</span></span>
* <span data-ttu-id="d6d14-1872">[ALTERAÇÃO SIGNIFICATIVA] O número padrão de resultados de `storage [blob|file|container|share] list` foi alterado para 5.000.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1872">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="d6d14-1873">Use `--num-results *` para o comportamento original de retornar todos os resultados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1873">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="d6d14-1874">Parâmetro `--marker` adicionado a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1874">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="d6d14-1875">Um marcador de log foi adicionado para a próxima página ao STDERR de `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1875">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="d6d14-1876">O comando `storage blob service-properties update` foi adicionado com suporte para sites estáticos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1876">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1877">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1877">VM</span></span>
* <span data-ttu-id="d6d14-1878">`vm [disk|unmanaged-disk]` e `vmss disk` foram alterados para que tenham parâmetros mais consistentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-1878">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="d6d14-1879">Suporte adicionado para referência cruzada de imagem de locatário a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1879">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d6d14-1880">O bug de configuração padrão foi corrigido em `vm diagnostics get-default-config --windows-os`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1880">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="d6d14-1881">O argumento `--provision-after-extensions` foi adicionado a `vmss extension set` para definir quais extensões deverão ser provisionadas antes da extensão ser definida</span><span class="sxs-lookup"><span data-stu-id="d6d14-1881">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="d6d14-1882">O argumento `--replica-count` foi adicionado a `sig image-version update` para definir a contagem de replicação padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1882">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="d6d14-1883">Foi corrigido o bug com `image create --source` em que o disco do sistema operacional de origem era confundido com uma VM do mesmo nome, mesmo se a ID de recurso completa fosse fornecida</span><span class="sxs-lookup"><span data-stu-id="d6d14-1883">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="d6d14-1884">20 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-1884">December 20, 2018</span></span>

<span data-ttu-id="d6d14-1885">Versão 2.0.54</span><span class="sxs-lookup"><span data-stu-id="d6d14-1885">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="d6d14-1886">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1886">Appservice</span></span>
* <span data-ttu-id="d6d14-1887">Corrigido o problema que causava falha na reimplantação do `webapp up`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1887">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="d6d14-1888">Adicionado suporte para listar e restaurar instantâneos de aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="d6d14-1888">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="d6d14-1889">Adicionado suporte para o sinalizador `--runtime` para aplicativos de funções do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-1889">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="d6d14-1890">IoT Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-1890">IoTCentral</span></span>
* <span data-ttu-id="d6d14-1891">Corrigida a chamada à API do comando de atualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-1891">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1892">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1892">Role</span></span>
* <span data-ttu-id="d6d14-1893">[ALTERAÇÃO SIGNIFICATIVA]`ad [app|sp] list` alterado para listar somente os 100 primeiros objetos por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1893">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-1894">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1894">SQL</span></span>
* <span data-ttu-id="d6d14-1895">Adicionado suporte para ordenação personalizada nas instâncias gerenciadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1895">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1896">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1896">VM</span></span>
* <span data-ttu-id="d6d14-1897">Parâmetro `---os-type` adicionado a `disk create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1897">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="d6d14-1898">18 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-1898">December 18, 2018</span></span>

<span data-ttu-id="d6d14-1899">Versão 2.0.53</span><span class="sxs-lookup"><span data-stu-id="d6d14-1899">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="d6d14-1900">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1900">ACR</span></span>
* <span data-ttu-id="d6d14-1901">Adicionado suporte para importação de imagem de Registros de Contêiner externos</span><span class="sxs-lookup"><span data-stu-id="d6d14-1901">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="d6d14-1902">Simplificado o layout da tabela para a lista de tarefas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1902">Condensed the table layout for task list</span></span>
* <span data-ttu-id="d6d14-1903">Adicionado suporte para URLs do Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="d6d14-1903">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-1904">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1904">ACS</span></span>
* <span data-ttu-id="d6d14-1905">Adicionada visualização dos nós virtuais</span><span class="sxs-lookup"><span data-stu-id="d6d14-1905">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="d6d14-1906">Removido “(VISUALIZAÇÃO)” de argumentos do AAD para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1906">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="d6d14-1907">[PRETERIDO] Comandos `az acs` preteridos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1907">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="d6d14-1908">O serviço ACS será desativado em 31 de janeiro de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-1908">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="d6d14-1909">Adicionado suporte da Política de Rede durante a criação de novos clusters AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-1909">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="d6d14-1910">Removido o requisito do argumento `--nodepool-name` para `aks scale` se houver apenas um pool de nós</span><span class="sxs-lookup"><span data-stu-id="d6d14-1910">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1911">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1911">Appservice</span></span>
* <span data-ttu-id="d6d14-1912">Corrigido o problema em que `webapp config container` não honra o parâmetro `--slot`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1912">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="d6d14-1913">Serviço de bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-1913">Botservice</span></span>
* <span data-ttu-id="d6d14-1914">Suporte adicionado para análise do arquivo `.bot` ao chamar `bot show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1914">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="d6d14-1915">Corrigido o bug de provisionamento do AppInsights</span><span class="sxs-lookup"><span data-stu-id="d6d14-1915">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="d6d14-1916">Corrigido o bug de espaço em branco ao lidar com caminhos de arquivo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1916">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="d6d14-1917">Reduzidas as chamadas de rede do Kudu</span><span class="sxs-lookup"><span data-stu-id="d6d14-1917">Reduced Kudu network calls</span></span>
* <span data-ttu-id="d6d14-1918">Melhorias de UX para comandos gerais</span><span class="sxs-lookup"><span data-stu-id="d6d14-1918">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-1919">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1919">Consumption</span></span>
* <span data-ttu-id="d6d14-1920">Corrigidos os bugs da API de orçamento ao mostrar notificações</span><span class="sxs-lookup"><span data-stu-id="d6d14-1920">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-1921">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-1921">CosmosDB</span></span>
* <span data-ttu-id="d6d14-1922">Suporte adicionado para atualizar a conta de vários mestres para mestre único</span><span class="sxs-lookup"><span data-stu-id="d6d14-1922">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="d6d14-1923">Mapas</span><span class="sxs-lookup"><span data-stu-id="d6d14-1923">Maps</span></span>
* <span data-ttu-id="d6d14-1924">Adicionado suporte ao SKU S1 para `maps account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1924">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1925">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1925">Network</span></span>
* <span data-ttu-id="d6d14-1926">Adicionado suporte para `--format` e `--log-version` para `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1926">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="d6d14-1927">Corrigido o problema com `dns zone update` em que usar "" para limpar a resolução e o registro de redes virtuais não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-1927">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-1928">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-1928">Resource</span></span>
* <span data-ttu-id="d6d14-1929">Corrigido o tratamento do parâmetro de escopo para grupos de gerenciamento do `policy assignment [create|list|delete|show|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1929">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="d6d14-1930">Adicionado o novo comando `resource wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1930">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-1931">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1931">Storage</span></span>
*  <span data-ttu-id="d6d14-1932">Adicionada a capacidade de atualizar a versão do esquema de log para serviços de armazenamento no `storage logging update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1932">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1933">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1933">VM</span></span>
* <span data-ttu-id="d6d14-1934">Corrigida a falha em `vm identity remove` quando a VM especificada não tem nenhuma identidade de serviço gerenciado atribuída</span><span class="sxs-lookup"><span data-stu-id="d6d14-1934">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="d6d14-1935">4 de dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-1935">December 4, 2018</span></span>

<span data-ttu-id="d6d14-1936">Versão 2.0.52</span><span class="sxs-lookup"><span data-stu-id="d6d14-1936">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="d6d14-1937">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1937">Core</span></span>
* <span data-ttu-id="d6d14-1938">Adicionado suporte para provisionamento de recursos de locatários cruzados para a entidade de serviço de multilocatários</span><span class="sxs-lookup"><span data-stu-id="d6d14-1938">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="d6d14-1939">Corrigido o bug onde as ids enviadas por pipe de um comando com a saída tsv eram analisados incorretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1939">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1940">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1940">Appservice</span></span>
* <span data-ttu-id="d6d14-1941">[VERSÃO PRÉVIA] Adicionado o comando `webapp up` que ajuda a criar e implantar conteúdo em aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1941">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="d6d14-1942">Corrigido um bug no aplicativo com base em contêiner do Windows devido à alteração de back-end</span><span class="sxs-lookup"><span data-stu-id="d6d14-1942">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1943">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1943">Network</span></span>
* <span data-ttu-id="d6d14-1944">Adicionado o argumento `--exclusion` a `application-gateway waf-config set` para dar suporte a exclusões de WAF</span><span class="sxs-lookup"><span data-stu-id="d6d14-1944">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-1945">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-1945">Role</span></span>
* <span data-ttu-id="d6d14-1946">Adicionado suporte para identificadores personalizados para a credencial de senha</span><span class="sxs-lookup"><span data-stu-id="d6d14-1946">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="d6d14-1947">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1947">VM</span></span>
* <span data-ttu-id="d6d14-1948">[PRETERIDO] Parâmetro `vm extension [show|wait] --expand` preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-1948">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="d6d14-1949">Adicionado parâmetro `--force` a `vm restart` para reimplantar as VMs sem resposta</span><span class="sxs-lookup"><span data-stu-id="d6d14-1949">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="d6d14-1950">Alterado `[vm|vmss] create --authentication-type` para aceitar "todos" para criar uma VM com senha e autenticação SSH</span><span class="sxs-lookup"><span data-stu-id="d6d14-1950">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="d6d14-1951">Adicionado parâmetro `image create --os-disk-caching` para definir o cache de disco do sistema operacional para uma imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-1951">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="d6d14-1952">20 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-1952">November 20, 2018</span></span>

<span data-ttu-id="d6d14-1953">Versão 2.0.51</span><span class="sxs-lookup"><span data-stu-id="d6d14-1953">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="d6d14-1954">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1954">Core</span></span>
* <span data-ttu-id="d6d14-1955">Logon do MSI alterado para não reutilizar o nome da assinatura na identidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-1955">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1956">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1956">ACR</span></span>
* <span data-ttu-id="d6d14-1957">Token de contexto adicionado à etapa da tarefa</span><span class="sxs-lookup"><span data-stu-id="d6d14-1957">Added context token to task step</span></span>
* <span data-ttu-id="d6d14-1958">Suporte adicionado para definir segredos na execução do acr para espelhar a tarefa do acr</span><span class="sxs-lookup"><span data-stu-id="d6d14-1958">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="d6d14-1959">Suporte aprimorado para `--top` e `--orderby` para os comandos `show-tags` e `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1959">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-1960">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-1960">Appservice</span></span>
* <span data-ttu-id="d6d14-1961">Tempo limite padrão para a implantação do zip alterado para sondar o status aumentado para 5 minutos, também adicionando uma propriedade de tempo limite para personalizar esse valor</span><span class="sxs-lookup"><span data-stu-id="d6d14-1961">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="d6d14-1962">Padrão `node_version` atualizado.</span><span class="sxs-lookup"><span data-stu-id="d6d14-1962">Updated the default `node_version`.</span></span> <span data-ttu-id="d6d14-1963">Redefinir a ação de troca de slots durante uma troca de duas fases preserva todas as configurações do aplicativo e cadeias de conexão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1963">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="d6d14-1964">Verificação da SKU no lado do cliente removida para o Linux criar o plano do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1964">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="d6d14-1965">Erro corrigido ao tentar obter o status de implantação do zip</span><span class="sxs-lookup"><span data-stu-id="d6d14-1965">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="d6d14-1966">Iot Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-1966">IotCentral</span></span>
* <span data-ttu-id="d6d14-1967">Verificação de disponibilidade do subdomínio adicionada ao criar um aplicativo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-1967">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-1968">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-1968">KeyVault</span></span>
* <span data-ttu-id="d6d14-1969">Bug corrigido em que os erros podem ter sido ignorados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1969">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-1970">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-1970">Network</span></span>
* <span data-ttu-id="d6d14-1971">Subcomandos `root-cert` adicionados a `application-gateway` para lidar com os certificados de raiz confiável</span><span class="sxs-lookup"><span data-stu-id="d6d14-1971">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="d6d14-1972">Opções `--min-capacity` e `--custom-error-pages` adicionadas a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-1972">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="d6d14-1973">`--zones` adicionado para suporte da zona de disponibilidade a `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1973">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="d6d14-1974">Argumentos `--file-upload-limit`, `--max-request-body-size` e `--request-body-check` a `application-gateway waf-config set` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1974">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-1975">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d6d14-1975">Rdbms</span></span>
* <span data-ttu-id="d6d14-1976">Comandos vnet do mariadb adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-1976">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="d6d14-1977">Rbac</span><span class="sxs-lookup"><span data-stu-id="d6d14-1977">Rbac</span></span>
* <span data-ttu-id="d6d14-1978">Um problema corrigido ao tentar atualizar credenciais inalteradas em `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1978">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="d6d14-1979">Avisos de saída adicionados para comunicar alterações de falha em um futuro próximo para `ad [app|sp] list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1979">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="d6d14-1980">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1980">Storage</span></span>
* <span data-ttu-id="d6d14-1981">Melhor manipulação de casos incomuns para os comandos da cópia de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-1981">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="d6d14-1982">Corrigido o problema em que `storage blob copy start-batch` não usava credenciais de logon quando as contas de origem e destino eram iguais</span><span class="sxs-lookup"><span data-stu-id="d6d14-1982">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="d6d14-1983">Bug corrigido com `storage [blob|file] url` em que `sas_token` não foi incorporado na URL</span><span class="sxs-lookup"><span data-stu-id="d6d14-1983">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="d6d14-1984">Aviso de alteração da falha adicionado a `[blob|container] list`: produzirá apenas os primeiros 5.000 resultados por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-1984">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-1985">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-1985">VM</span></span>
* <span data-ttu-id="d6d14-1986">Suporte adicionado a `[vm|vmss] create --storage-sku` para especificar a SKU da conta de armazenamento para o SO gerenciado e os discos de dados separadamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-1986">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="d6d14-1987">Parâmetros do nome da versão alterados de `sig image-version` para `--image-version -e`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1987">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="d6d14-1988">Argumento `sig image-version` preterido `--image-version-name`, substituído por `--image-version`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1988">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="d6d14-1989">Suporte adicionado para usar o disco local do SO a `[vm|vmss] create --ephemeral-os-disk`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1989">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="d6d14-1990">Adicionado o suporte ao `--no-wait` para `snapshot create/update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1990">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="d6d14-1991">Adicionado o comando `snapshot wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1991">Added `snapshot wait` command</span></span>
* <span data-ttu-id="d6d14-1992">Suporte adicionado para usar o nome da instância com `[vm|vmss] extension set --extension-instance-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-1992">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="d6d14-1993">6 de novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-1993">November 6, 2018</span></span>

<span data-ttu-id="d6d14-1994">Versão 2.0.50</span><span class="sxs-lookup"><span data-stu-id="d6d14-1994">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-1995">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-1995">Core</span></span>
* <span data-ttu-id="d6d14-1996">Foi adicionado suporte para o serviço principal sn + autenticação do emissor</span><span class="sxs-lookup"><span data-stu-id="d6d14-1996">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-1997">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-1997">ACR</span></span>
* <span data-ttu-id="d6d14-1998">Foi adicionado suporte para eventos de git de solicitação de pull e de confirmação para o gatilho de origem da tarefa</span><span class="sxs-lookup"><span data-stu-id="d6d14-1998">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="d6d14-1999">Alterado para usar o padrão do Dockerfile se ele não for especificado no comando de compilação</span><span class="sxs-lookup"><span data-stu-id="d6d14-1999">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2000">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2000">ACS</span></span>
* <span data-ttu-id="d6d14-2001">[ALTERAÇÃO SIGNIFICATIVA]`enable_cloud_console_aks_browse` foi removido para habilitar 'az aks browse' por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2001">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="d6d14-2002">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d6d14-2002">Advisor</span></span>
* <span data-ttu-id="d6d14-2003">Versão de GA</span><span class="sxs-lookup"><span data-stu-id="d6d14-2003">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-2004">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2004">AMS</span></span>
* <span data-ttu-id="d6d14-2005">Novos grupos de comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2005">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="d6d14-2006">Novos comandos adicionados:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2006">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="d6d14-2007">Adicionados parâmetros de criptografia com suporte para `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2007">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="d6d14-2008">O suporte adicionado para `ams transform output remove` agora pode ser executado passando o índice de saída a ser removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2008">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="d6d14-2009">Adicionados os argumentos `--correlation-data` e `--label` ao grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2009">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="d6d14-2010">Adicionados os argumentos `--storage-account` e `--container` ao grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2010">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="d6d14-2011">Foram adicionados valores padrões para o horário de expiração (agora +23h) e permissões (Leitura) no comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2011">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="d6d14-2012">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming locator` foi substituído por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2012">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="d6d14-2013">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--content-keys` de `ams streaming locator` foi atualizado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2013">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="d6d14-2014">[ALTERAÇÃO SIGNIFICATIVA]`--content-policy-name` foi renomeado como `--content-key-policy-name` no comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2014">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="d6d14-2015">[ALTERAÇÃO SIGNIFICATIVA] O comando `ams streaming policy` foi substituído por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2015">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="d6d14-2016">[ALTERAÇÃO SIGNIFICATIVA] O argumento `--preset-names` foi substituído por `--preset` no grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2016">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="d6d14-2017">Agora, você só pode definir uma saída/predefinição de cada vez (para adicionar mais, é preciso executar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="d6d14-2017">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="d6d14-2018">Além disso, você pode definir StandardEncoderPreset personalizado passando o caminho para seu JSON personalizado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2018">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="d6d14-2019">[ALTERAÇÃO SIGNIFICATIVA]`--output-asset-names ` foi renomeado como `--output-assets` no comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2019">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="d6d14-2020">Agora, ele aceita uma lista separada por espaços dos ativos no formato 'assetName=label'.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2020">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="d6d14-2021">Um ativo sem rótulo pode ser enviado assim: 'assetName='</span><span class="sxs-lookup"><span data-stu-id="d6d14-2021">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2022">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2022">AppService</span></span>
* <span data-ttu-id="d6d14-2023">Um bug no `az webapp config backup update` que impede a configuração de um agendamento de backup foi corrigido, caso ele ainda não tenha sido definido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2023">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="d6d14-2024">Configurar</span><span class="sxs-lookup"><span data-stu-id="d6d14-2024">Configure</span></span>
* <span data-ttu-id="d6d14-2025">O YAML foi adicionado às opções de formato de saída</span><span class="sxs-lookup"><span data-stu-id="d6d14-2025">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2026">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2026">Container</span></span>
* <span data-ttu-id="d6d14-2027">Alterado para mostrar a identidade ao exportar um grupo de contêineres para yaml</span><span class="sxs-lookup"><span data-stu-id="d6d14-2027">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="d6d14-2028">EventHub</span><span class="sxs-lookup"><span data-stu-id="d6d14-2028">EventHub</span></span>
* <span data-ttu-id="d6d14-2029">O sinalizador `--enable-kafka` foi adicionado para dar suporte ao Kafka no `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2029">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2030">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2030">Interactive</span></span>
* <span data-ttu-id="d6d14-2031">O interativo agora instala a extensão `interactive` que permite atualizações e suporte mais rápidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2031">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2032">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2032">Monitor</span></span>
* <span data-ttu-id="d6d14-2033">Foi adicionado suporte para nomes de métricas, que incluem os caracteres barra (/) e ponto (.) para `--condition` em `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2033">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2034">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2034">Network</span></span>
* <span data-ttu-id="d6d14-2035">Os nomes de comandos `network interface-endpoint` foram preteridos em benefício de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2035">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="d6d14-2036">Foi corrigido um problema onde um argumento `--peer-circuit` em `express-route peering connection create` não aceitaria uma ID</span><span class="sxs-lookup"><span data-stu-id="d6d14-2036">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="d6d14-2037">Foi corrigido um problema onde `--ip-tags` não funcionava corretamente com `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2037">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="d6d14-2038">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2038">Profile</span></span>
* <span data-ttu-id="d6d14-2039">`--use-cert-sn-issuer` foi adicionado a `az login` para logon da entidade de serviço com rolagens automáticas de certificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2039">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2040">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2040">RDBMS</span></span>
* <span data-ttu-id="d6d14-2041">Adicionados comandos da réplica mysql</span><span class="sxs-lookup"><span data-stu-id="d6d14-2041">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2042">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2042">Resource</span></span>
* <span data-ttu-id="d6d14-2043">Adicionado suporte para grupos de gerenciamento e assinaturas aos comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2043">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2044">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2044">Role</span></span>
* <span data-ttu-id="d6d14-2045">Adicionado suporte para gerenciamento de permissões de API, usuário conectado e gerenciamento de senhas dos aplicativos e certificados de credenciais</span><span class="sxs-lookup"><span data-stu-id="d6d14-2045">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="d6d14-2046">`ad sp create-for-rbac` foi alterado para esclarecer a confusão entre o displayName e o nome da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2046">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="d6d14-2047">Suporte adicionado para conceder permissões a aplicativos do AAD</span><span class="sxs-lookup"><span data-stu-id="d6d14-2047">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2048">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2048">Storage</span></span>
* <span data-ttu-id="d6d14-2049">Suporte adicionado para se conectar aos serviços de armazenamento somente com SAS e pontos de extremidade (sem um nome de conta ou uma chave), conforme descrito em `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2049">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2050">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2050">VM</span></span>
* <span data-ttu-id="d6d14-2051">O argumento `storage-sku` foi adicionado a `image create` para definir o tipo de conta de armazenamento padrão da imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-2051">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="d6d14-2052">O bug com `vm resize` onde a opção `--no-wait` faz com que o comando falhasse foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2052">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="d6d14-2053">O formato de saída da tabela `vm encryption show` para mostrar o status foi alterado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2053">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="d6d14-2054">`vm secret format` foi alterado para exigir a saída json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2054">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="d6d14-2055">Avisa o usuário e assume como padrão a saída json se um formato de saída indesejado for escolhido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2055">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="d6d14-2056">Validação de argumento aprimorado para `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2056">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="d6d14-2057">23 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2057">October 23, 2018</span></span>

<span data-ttu-id="d6d14-2058">Versão 2.0.49</span><span class="sxs-lookup"><span data-stu-id="d6d14-2058">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2059">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2059">Core</span></span>
* <span data-ttu-id="d6d14-2060">Corrigido o problema com `--ids` onde `--subscription` teria precedência sobre a assinatura em `--ids`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2060">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="d6d14-2061">Adicionados avisos explícitos quando parâmetros seriam ignorados pelo uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2061">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2062">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2062">ACR</span></span>
* <span data-ttu-id="d6d14-2063">Corrigido um problema de codificação de ACR Build no Python2</span><span class="sxs-lookup"><span data-stu-id="d6d14-2063">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-2064">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-2064">CDN</span></span>
* <span data-ttu-id="d6d14-2065">[ALTERAÇÃO SIGNIFICATIVA] Alterado o comportamento de armazenamento em cache da cadeia de caracteres de consulta padrão de `cdn endpoint create` para não assumir o padrão "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="d6d14-2065">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="d6d14-2066">Agora, ele é definido pelo serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2066">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2067">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2067">Container</span></span>
* <span data-ttu-id="d6d14-2068">Adicionado `Private` como um tipo válido para passar para '--ip-address'</span><span class="sxs-lookup"><span data-stu-id="d6d14-2068">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="d6d14-2069">Alterado para permitir o uso somente de ID de sub-rede para configurar uma rede virtual para o grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d6d14-2069">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="d6d14-2070">Alterado para permitir o uso de nome de rede virtual ou ID de recurso para habilitar o uso de redes virtuais de diferentes grupos de recursos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2070">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="d6d14-2071">Adicionado `--assign-identity` para adicionar uma identidade MSI a um grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d6d14-2071">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="d6d14-2072">Adicionado `--scope` para criar uma atribuição de função para a identidade MSI atribuída pelo sistema</span><span class="sxs-lookup"><span data-stu-id="d6d14-2072">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="d6d14-2073">Adicionado um aviso ao criar um grupo de contêineres com uma imagem sem um processo de execução longa</span><span class="sxs-lookup"><span data-stu-id="d6d14-2073">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="d6d14-2074">Corrigidos os problemas de saída da tabela para comandos `list` e `show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2074">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-2075">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2075">CosmosDB</span></span>
* <span data-ttu-id="d6d14-2076">Adicionado o suporte `--enable-multiple-write-locations` para `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2076">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2077">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2077">Interactive</span></span>
* <span data-ttu-id="d6d14-2078">Alterado para garantir que o parâmetro de assinatura global seja exibido nos parâmetros</span><span class="sxs-lookup"><span data-stu-id="d6d14-2078">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="d6d14-2079">Central da IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2079">IoT Central</span></span>
* <span data-ttu-id="d6d14-2080">Adicionadas opções de nome de exibição e modelo para criação de aplicativos de IoT Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-2080">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="d6d14-2081">[ALTERAÇÃO SIGNIFICATIVA] Removido o suporte para a SKU F1; Use a SKU S1</span><span class="sxs-lookup"><span data-stu-id="d6d14-2081">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2082">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2082">Monitor</span></span>
* <span data-ttu-id="d6d14-2083">Alterações para `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2083">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="d6d14-2084">Adicionado suporte para listar todos os eventos no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2084">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="d6d14-2085">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2085">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d6d14-2086">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-2086">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="d6d14-2087">Adicionado `--namespace` como alias para a opção preterida `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2087">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="d6d14-2088">Preterido `--filters` porque não há valores diferentes daqueles com opções fortemente tipadas compatíveis com o serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2088">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="d6d14-2089">Alterações para `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2089">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="d6d14-2090">Adicionado o parâmetro `--offset` para criar consultas de tempo mais facilmente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2090">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="d6d14-2091">Melhorada a validação para `--start-time` e `--end-time` para usar um intervalo mais amplo de formatos ISO8601 e formatos de data/hora mais amigáveis ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-2091">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="d6d14-2092">Melhorada a validação para os argumentos `--event-hub` e `--event-hub-rule` para `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2092">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2093">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2093">Network</span></span>
* <span data-ttu-id="d6d14-2094">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic create`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="d6d14-2094">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="d6d14-2095">Adicionados os argumentos `--app-gateway-address-pools` e `--gateway-name` para `nic ip-config create/update`, para dar suporte à adição de pools de endereços de back-end do gateway de aplicativo a um NIC</span><span class="sxs-lookup"><span data-stu-id="d6d14-2095">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="d6d14-2096">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d6d14-2096">ServiceBus</span></span>
* <span data-ttu-id="d6d14-2097">Adicionado `migration_state` somente leitura para MigrationConfigProperties para mostrar o atual estado de migração de namespace Standard para Premium do Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2097">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2098">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2098">SQL</span></span>
* <span data-ttu-id="d6d14-2099">Corrigidos `sql failover-group create` e `sql failover-group update` para trabalhar com a política de failover Manual</span><span class="sxs-lookup"><span data-stu-id="d6d14-2099">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2100">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2100">Storage</span></span>
* <span data-ttu-id="d6d14-2101">Corrigida a formatação de saída `az storage cors list`, todos os itens mostram a chave correta de "Serviço"</span><span class="sxs-lookup"><span data-stu-id="d6d14-2101">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="d6d14-2102">Adicionado o parâmetro `--bypass-immutability-policy` para a exclusão de contêiner bloqueado pela política de imutabilidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-2102">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2103">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2103">VM</span></span>
* <span data-ttu-id="d6d14-2104">Aplicado o modo `None` de armazenamento em cache de disco para as séries Lv/Lv2 de computadores no `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2104">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="d6d14-2105">Atualizada a lista de tamanhos com suporte compatíveis com a aceleração de rede para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2105">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="d6d14-2106">Adicionado argumentos fortemente tipados para configurações de iops e mbps de ultra ssd para `disk create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2106">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="d6d14-2107">16 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2107">October 16, 2018</span></span>

<span data-ttu-id="d6d14-2108">Versão 2.0.48</span><span class="sxs-lookup"><span data-stu-id="d6d14-2108">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2109">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2109">VM</span></span>
* <span data-ttu-id="d6d14-2110">Corrigido o problema do SDK que causava falha durante a instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="d6d14-2110">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="d6d14-2111">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2111">October 9, 2018</span></span>

<span data-ttu-id="d6d14-2112">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="d6d14-2112">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2113">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2113">Core</span></span>
* <span data-ttu-id="d6d14-2114">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="d6d14-2114">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2115">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2115">ACR</span></span>
* <span data-ttu-id="d6d14-2116">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="d6d14-2116">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2117">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2117">ACS</span></span>
* <span data-ttu-id="d6d14-2118">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="d6d14-2118">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="d6d14-2119">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="d6d14-2119">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="d6d14-2120">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2120">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="d6d14-2121">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2121">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2122">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2122">Container</span></span>
* <span data-ttu-id="d6d14-2123">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um runtime específico</span><span class="sxs-lookup"><span data-stu-id="d6d14-2123">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="d6d14-2124">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-2124">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="d6d14-2125">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2125">Event Hub</span></span>
* <span data-ttu-id="d6d14-2126">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2126">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="d6d14-2127">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="d6d14-2127">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="d6d14-2128">Extensões</span><span class="sxs-lookup"><span data-stu-id="d6d14-2128">Extensions</span></span>
* <span data-ttu-id="d6d14-2129">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2129">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d6d14-2130">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d6d14-2130">HDInsight</span></span>
* <span data-ttu-id="d6d14-2131">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2131">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-2132">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2132">IoT</span></span>
* <span data-ttu-id="d6d14-2133">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2133">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-2134">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-2134">KeyVault</span></span>
* <span data-ttu-id="d6d14-2135">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2135">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2136">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2136">Network</span></span>
* <span data-ttu-id="d6d14-2137">Corrigido `network dns zone create`: O comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2137">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="d6d14-2138">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="d6d14-2138">See #6052</span></span>
* <span data-ttu-id="d6d14-2139">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2139">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="d6d14-2140">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="d6d14-2140">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="d6d14-2141">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2141">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="d6d14-2142">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2142">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="d6d14-2143">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2143">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="d6d14-2144">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2144">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2145">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2145">Role</span></span>
* <span data-ttu-id="d6d14-2146">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2146">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="d6d14-2147">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2147">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="d6d14-2148">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2148">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="d6d14-2149">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="d6d14-2149">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="d6d14-2150">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2150">Service Bus</span></span>
* <span data-ttu-id="d6d14-2151">[ALTERAÇÃO SIGNIFICATIVA]`list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="d6d14-2151">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2152">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2152">VM</span></span>
* <span data-ttu-id="d6d14-2153">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2153">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="d6d14-2154">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2154">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="d6d14-2155">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2155">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="d6d14-2156">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2156">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="d6d14-2157">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2157">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="d6d14-2158">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="d6d14-2158">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="d6d14-2159">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2159">September 21, 2018</span></span>

<span data-ttu-id="d6d14-2160">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="d6d14-2160">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2161">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2161">ACR</span></span>
* <span data-ttu-id="d6d14-2162">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2162">Added ACR Task commands</span></span>
* <span data-ttu-id="d6d14-2163">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2163">Added quick run command</span></span>
* <span data-ttu-id="d6d14-2164">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2164">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="d6d14-2165">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2165">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="d6d14-2166">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2166">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="d6d14-2167">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="d6d14-2167">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2168">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2168">ACS</span></span>
* <span data-ttu-id="d6d14-2169">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2169">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="d6d14-2170">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="d6d14-2170">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2171">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2171">AppService</span></span>

* <span data-ttu-id="d6d14-2172">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2172">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="d6d14-2173">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="d6d14-2173">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="d6d14-2174">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="d6d14-2174">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="d6d14-2175">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2175">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-2176">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2176">Batch</span></span>
* <span data-ttu-id="d6d14-2177">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="d6d14-2177">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="d6d14-2178">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2178">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="d6d14-2179">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2179">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="d6d14-2180">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2180">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d6d14-2181">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2181">Batch AI</span></span> 
* <span data-ttu-id="d6d14-2182">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2182">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d6d14-2183">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2183">Cognitive Services</span></span>
* <span data-ttu-id="d6d14-2184">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2184">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="d6d14-2185">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2185">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="d6d14-2186">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2186">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="d6d14-2187">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2187">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="d6d14-2188">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2188">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="d6d14-2189">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2189">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2190">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2190">Container</span></span>
* <span data-ttu-id="d6d14-2191">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="d6d14-2191">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="d6d14-2192">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2192">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="d6d14-2193">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="d6d14-2193">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="d6d14-2194">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="d6d14-2194">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="d6d14-2195">DataLake</span><span class="sxs-lookup"><span data-stu-id="d6d14-2195">Datalake</span></span>
* <span data-ttu-id="d6d14-2196">Comandos adicionados para regras da rede virtual</span><span class="sxs-lookup"><span data-stu-id="d6d14-2196">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="d6d14-2197">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2197">Interactive Shell</span></span>
* <span data-ttu-id="d6d14-2198">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2198">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="d6d14-2199">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2199">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-2200">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2200">IoT</span></span>
* <span data-ttu-id="d6d14-2201">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2201">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-2202">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d6d14-2202">Key Vault</span></span>
* <span data-ttu-id="d6d14-2203">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="d6d14-2203">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2204">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2204">Network</span></span>
* <span data-ttu-id="d6d14-2205">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="d6d14-2205">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="d6d14-2206">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2206">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="d6d14-2207">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="d6d14-2207">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="d6d14-2208">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="d6d14-2208">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="d6d14-2209">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2209">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="d6d14-2210">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2210">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="d6d14-2211">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2211">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="d6d14-2212">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2212">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="d6d14-2213">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2213">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="d6d14-2214">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2214">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="d6d14-2215">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2215">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="d6d14-2216">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2216">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="d6d14-2217">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2217">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="d6d14-2218">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2218">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="d6d14-2219">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2219">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="d6d14-2220">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="d6d14-2220">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="d6d14-2221">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2221">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="d6d14-2222">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2222">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2223">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2223">RDBMS</span></span>
* <span data-ttu-id="d6d14-2224">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2224">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="d6d14-2225">Reserva</span><span class="sxs-lookup"><span data-stu-id="d6d14-2225">Reservation</span></span>
* <span data-ttu-id="d6d14-2226">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2226">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="d6d14-2227">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="d6d14-2227">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="d6d14-2228">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2228">Manage App</span></span>
* <span data-ttu-id="d6d14-2229">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="d6d14-2229">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="d6d14-2230">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="d6d14-2230">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2231">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2231">Role</span></span>
* <span data-ttu-id="d6d14-2232">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="d6d14-2232">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="d6d14-2233">SignalR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2233">SignalR</span></span>
* <span data-ttu-id="d6d14-2234">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2234">First release</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2235">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2235">Storage</span></span>
* <span data-ttu-id="d6d14-2236">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="d6d14-2236">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="d6d14-2237">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="d6d14-2237">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2238">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2238">VM</span></span>
* <span data-ttu-id="d6d14-2239">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2239">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="d6d14-2240">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2240">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="d6d14-2241">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2241">August 28, 2018</span></span>

<span data-ttu-id="d6d14-2242">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="d6d14-2242">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2243">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2243">Core</span></span>

* <span data-ttu-id="d6d14-2244">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="d6d14-2244">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="d6d14-2245">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d6d14-2245">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2246">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2246">ACR</span></span>

* <span data-ttu-id="d6d14-2247">Adicionada uma solução alternativa para operações de runtime sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2247">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="d6d14-2248">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2248">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2249">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2249">ACS</span></span>

* <span data-ttu-id="d6d14-2250">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2250">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="d6d14-2251">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-2251">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2252">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2252">AppService</span></span>

* <span data-ttu-id="d6d14-2253">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="d6d14-2253">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="d6d14-2254">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2254">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="d6d14-2255">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2255">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-2256">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-2256">Backup</span></span>

* <span data-ttu-id="d6d14-2257">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2257">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="d6d14-2258">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="d6d14-2258">Bot Service</span></span>

* <span data-ttu-id="d6d14-2259">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2259">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d6d14-2260">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2260">Cognitive Services</span></span>

* <span data-ttu-id="d6d14-2261">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="d6d14-2261">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-2262">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2262">IoT</span></span>

* <span data-ttu-id="d6d14-2263">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2263">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2264">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2264">Monitor</span></span>

* <span data-ttu-id="d6d14-2265">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="d6d14-2265">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="d6d14-2266">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2266">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2267">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2267">Network</span></span>

* <span data-ttu-id="d6d14-2268">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2268">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2269">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2269">Resource</span></span>

* <span data-ttu-id="d6d14-2270">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2270">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2271">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2271">Storage</span></span>

* <span data-ttu-id="d6d14-2272">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2272">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2273">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2273">VM</span></span>

* <span data-ttu-id="d6d14-2274">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2274">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="d6d14-2275">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2275">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="d6d14-2276">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2276">Auguest 14, 2018</span></span>

<span data-ttu-id="d6d14-2277">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="d6d14-2277">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2278">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2278">Core</span></span>

* <span data-ttu-id="d6d14-2279">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2279">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="d6d14-2280">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="d6d14-2280">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="d6d14-2281">Telemetria</span><span class="sxs-lookup"><span data-stu-id="d6d14-2281">Telemetry</span></span>

* <span data-ttu-id="d6d14-2282">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="d6d14-2282">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2283">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2283">ACR</span></span>

* <span data-ttu-id="d6d14-2284">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2284">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="d6d14-2285">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2285">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2286">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2286">ACS</span></span>

* <span data-ttu-id="d6d14-2287">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-2287">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="d6d14-2288">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2288">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="d6d14-2289">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="d6d14-2289">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="d6d14-2290">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="d6d14-2290">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="d6d14-2291">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="d6d14-2291">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="d6d14-2292">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2292">AppService</span></span>

* <span data-ttu-id="d6d14-2293">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2293">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="d6d14-2294">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="d6d14-2294">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-2295">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2295">BatchAI</span></span>

* <span data-ttu-id="d6d14-2296">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2296">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="d6d14-2297">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2297">Container</span></span>

* <span data-ttu-id="d6d14-2298">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2298">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="d6d14-2299">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2299">IoT</span></span>

* <span data-ttu-id="d6d14-2300">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="d6d14-2300">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="d6d14-2301">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2301">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="d6d14-2302">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2302">Iot Central</span></span>

* <span data-ttu-id="d6d14-2303">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="d6d14-2303">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-2304">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-2304">KeyVault</span></span>


* <span data-ttu-id="d6d14-2305">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2305">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="d6d14-2306">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2306">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="d6d14-2307">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2307">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="d6d14-2308">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="d6d14-2308">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="d6d14-2309">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="d6d14-2309">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="d6d14-2310">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2310">Relay</span></span>

* <span data-ttu-id="d6d14-2311">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2311">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2312">Sql</span><span class="sxs-lookup"><span data-stu-id="d6d14-2312">Sql</span></span>

* <span data-ttu-id="d6d14-2313">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2313">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2314">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2314">Storage</span></span>

* <span data-ttu-id="d6d14-2315">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="d6d14-2315">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="d6d14-2316">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2316">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="d6d14-2317">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2317">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="d6d14-2318">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2318">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="d6d14-2319">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2319">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2320">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2320">VM</span></span>

* <span data-ttu-id="d6d14-2321">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2321">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="d6d14-2322">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2322">July 31, 2018</span></span>

<span data-ttu-id="d6d14-2323">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="d6d14-2323">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2324">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2324">ACR</span></span>

* <span data-ttu-id="d6d14-2325">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2325">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="d6d14-2326">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2326">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2327">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2327">ACS</span></span>

* <span data-ttu-id="d6d14-2328">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2328">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-2329">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2329">Batch</span></span>

* <span data-ttu-id="d6d14-2330">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="d6d14-2330">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2331">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2331">Container</span></span>

* <span data-ttu-id="d6d14-2332">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2332">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2333">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2333">Network</span></span>

* <span data-ttu-id="d6d14-2334">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d6d14-2334">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="d6d14-2335">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2335">Resource</span></span>

* <span data-ttu-id="d6d14-2336">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-2336">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="d6d14-2337">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-2337">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2338">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2338">Role</span></span>

* <span data-ttu-id="d6d14-2339">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d6d14-2339">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="d6d14-2340">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2340">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="d6d14-2341">Search</span><span class="sxs-lookup"><span data-stu-id="d6d14-2341">Search</span></span>

* <span data-ttu-id="d6d14-2342">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="d6d14-2342">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="d6d14-2343">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2343">Service Bus</span></span>

* <span data-ttu-id="d6d14-2344">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="d6d14-2344">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="d6d14-2345">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2345">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="d6d14-2346">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2346">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="d6d14-2347">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2347">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2348">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2348">Storage</span></span>

* <span data-ttu-id="d6d14-2349">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2349">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="d6d14-2350">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2350">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2351">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2351">VM</span></span>

* <span data-ttu-id="d6d14-2352">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2352">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="d6d14-2353">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2353">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="d6d14-2354">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2354">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="d6d14-2355">[ALTERAÇÃO SIGNIFICATIVA]`[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="d6d14-2355">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="d6d14-2356">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2356">July 18, 2018</span></span>

<span data-ttu-id="d6d14-2357">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="d6d14-2357">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2358">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2358">Core</span></span>

* <span data-ttu-id="d6d14-2359">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2359">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="d6d14-2360">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="d6d14-2360">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="d6d14-2361">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2361">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2362">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2362">ACR</span></span>

* <span data-ttu-id="d6d14-2363">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="d6d14-2363">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="d6d14-2364">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2364">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="d6d14-2365">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2365">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="d6d14-2366">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-2366">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2367">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2367">ACS</span></span>

* <span data-ttu-id="d6d14-2368">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="d6d14-2368">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2369">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2369">AppService</span></span>

* <span data-ttu-id="d6d14-2370">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="d6d14-2370">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-2371">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2371">Batch</span></span>

* <span data-ttu-id="d6d14-2372">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d6d14-2372">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="d6d14-2373">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2373">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d6d14-2374">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2374">Batch AI</span></span>

* <span data-ttu-id="d6d14-2375">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2375">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2376">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2376">Container</span></span>

* <span data-ttu-id="d6d14-2377">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="d6d14-2377">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="d6d14-2378">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="d6d14-2378">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2379">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2379">Network</span></span>

* <span data-ttu-id="d6d14-2380">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2380">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="d6d14-2381">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2381">Added `network nic wait`</span></span>
* <span data-ttu-id="d6d14-2382">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2382">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="d6d14-2383">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2383">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="d6d14-2384">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2384">Resource</span></span>

* <span data-ttu-id="d6d14-2385">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2385">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="d6d14-2386">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2386">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="d6d14-2387">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2387">Added `deployment wait` command</span></span>
* <span data-ttu-id="d6d14-2388">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d6d14-2388">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2389">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2389">SQL</span></span>

* <span data-ttu-id="d6d14-2390">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2390">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="d6d14-2391">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2391">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="d6d14-2392">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2392">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2393">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2393">Storage</span></span>

* <span data-ttu-id="d6d14-2394">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="d6d14-2394">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2395">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2395">VM</span></span>

* <span data-ttu-id="d6d14-2396">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2396">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="d6d14-2397">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2397">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="d6d14-2398">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2398">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d6d14-2399">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2399">July 3, 2018</span></span>

<span data-ttu-id="d6d14-2400">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="d6d14-2400">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-2401">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2401">AKS</span></span>

* <span data-ttu-id="d6d14-2402">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2402">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d6d14-2403">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2403">July 3, 2018</span></span>

<span data-ttu-id="d6d14-2404">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="d6d14-2404">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2405">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2405">Core</span></span>

* <span data-ttu-id="d6d14-2406">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2406">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2407">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2407">ACR</span></span>

* <span data-ttu-id="d6d14-2408">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2408">Added polling build status</span></span>
* <span data-ttu-id="d6d14-2409">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2409">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="d6d14-2410">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2410">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2411">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2411">ACS</span></span>

* <span data-ttu-id="d6d14-2412">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2412">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="d6d14-2413">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="d6d14-2413">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="d6d14-2414">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2414">Updated options for `aks browse` command.</span></span> <span data-ttu-id="d6d14-2415">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2415">Added `--listen-port` support</span></span>
* <span data-ttu-id="d6d14-2416">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2416">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="d6d14-2417">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="d6d14-2417">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="d6d14-2418">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2418">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2419">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2419">AppService</span></span>

* <span data-ttu-id="d6d14-2420">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2420">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="d6d14-2421">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-2421">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-2422">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-2422">Backup</span></span>

* <span data-ttu-id="d6d14-2423">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2423">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-2424">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2424">BatchAI</span></span>

* <span data-ttu-id="d6d14-2425">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2425">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="d6d14-2426">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-2426">Cloud</span></span>

* <span data-ttu-id="d6d14-2427">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-2427">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2428">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2428">Container</span></span>

* <span data-ttu-id="d6d14-2429">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="d6d14-2429">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="d6d14-2430">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-2430">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="d6d14-2431">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="d6d14-2431">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2432">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2432">Extension</span></span>

* <span data-ttu-id="d6d14-2433">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2433">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2434">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2434">Network</span></span>

* <span data-ttu-id="d6d14-2435">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="d6d14-2435">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2436">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d6d14-2436">Rdbms</span></span>

* <span data-ttu-id="d6d14-2437">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2437">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2438">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2438">Resource</span></span>

* <span data-ttu-id="d6d14-2439">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2439">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2440">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2440">VM</span></span>

* <span data-ttu-id="d6d14-2441">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="d6d14-2441">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="d6d14-2442">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2442">June 25, 2018</span></span>

<span data-ttu-id="d6d14-2443">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="d6d14-2443">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="d6d14-2444">CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2444">CLI</span></span>

* <span data-ttu-id="d6d14-2445">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2445">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="d6d14-2446">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2446">June 19, 2018</span></span>

<span data-ttu-id="d6d14-2447">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="d6d14-2447">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2448">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2448">Core</span></span>

* <span data-ttu-id="d6d14-2449">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2449">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2450">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2450">ACR</span></span>

* <span data-ttu-id="d6d14-2451">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="d6d14-2451">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="d6d14-2452">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2452">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2453">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2453">ACS</span></span>

* <span data-ttu-id="d6d14-2454">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2454">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="d6d14-2455">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2455">Added `--update` support</span></span>
* <span data-ttu-id="d6d14-2456">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2456">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="d6d14-2457">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2457">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="d6d14-2458">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2458">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="d6d14-2459">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2459">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="d6d14-2460">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2460">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="d6d14-2461">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2461">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2462">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2462">AppService</span></span>

* <span data-ttu-id="d6d14-2463">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="d6d14-2463">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="d6d14-2464">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2464">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-2465">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2465">Batch</span></span>

* <span data-ttu-id="d6d14-2466">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="d6d14-2466">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d6d14-2467">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2467">Batch AI</span></span>

* <span data-ttu-id="d6d14-2468">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2468">Added support for workspaces.</span></span> <span data-ttu-id="d6d14-2469">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2469">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="d6d14-2470">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2470">Added support for experiments.</span></span> <span data-ttu-id="d6d14-2471">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2471">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="d6d14-2472">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="d6d14-2472">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="d6d14-2473">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2473">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="d6d14-2474">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2474">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="d6d14-2475">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2475">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="d6d14-2476">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos workspaces</span><span class="sxs-lookup"><span data-stu-id="d6d14-2476">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="d6d14-2477">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="d6d14-2477">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="d6d14-2478">[ALTERAÇÃO SIGNIFICATIVA]`--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2478">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="d6d14-2479">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2479">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="d6d14-2480">[ALTERAÇÃO SIGNIFICATIVA]`--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2480">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="d6d14-2481">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2481">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="d6d14-2482">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2482">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="d6d14-2483">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2483">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="d6d14-2484">[ALTERAÇÃO SIGNIFICATIVA]`--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2484">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="d6d14-2485">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2485">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="d6d14-2486">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2486">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="d6d14-2487">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2487">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d6d14-2488">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2488">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="d6d14-2489">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2489">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="d6d14-2490">Mapas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2490">Maps</span></span>

* <span data-ttu-id="d6d14-2491">[ALTERAÇÃO SIGNIFICATIVA]`maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2491">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2492">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2492">Network</span></span>

* <span data-ttu-id="d6d14-2493">Suporte adicionado para `https` a `network lb probe create` [nº6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2493">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="d6d14-2494">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2494">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="d6d14-2495">#6502</span><span class="sxs-lookup"><span data-stu-id="d6d14-2495">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="d6d14-2496">Reservas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2496">Reservations</span></span>

* <span data-ttu-id="d6d14-2497">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2497">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="d6d14-2498">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2498">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="d6d14-2499">[ALTERAÇÃO SIGNIFICATIVA]`kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2499">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="d6d14-2500">[ALTERAÇÃO SIGNIFICATIVA]`capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2500">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="d6d14-2501">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2501">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="d6d14-2502">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2502">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2503">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2503">Role</span></span>

* <span data-ttu-id="d6d14-2504">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2504">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2505">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2505">SQL</span></span>

* <span data-ttu-id="d6d14-2506">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2506">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2507">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2507">Storage</span></span>

* <span data-ttu-id="d6d14-2508">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="d6d14-2508">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2509">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2509">VM</span></span>

* <span data-ttu-id="d6d14-2510">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2510">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="d6d14-2511">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2511">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="d6d14-2512">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2512">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d6d14-2513">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2513">June 13, 2018</span></span>

<span data-ttu-id="d6d14-2514">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="d6d14-2514">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2515">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2515">Core</span></span>

* <span data-ttu-id="d6d14-2516">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2516">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d6d14-2517">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2517">June 13, 2018</span></span>

<span data-ttu-id="d6d14-2518">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d6d14-2518">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-2519">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2519">AKS</span></span>

* <span data-ttu-id="d6d14-2520">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2520">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d6d14-2521">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="d6d14-2521">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="d6d14-2522">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2522">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d6d14-2523">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2523">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d6d14-2524">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2524">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2525">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2525">AppService</span></span>

* <span data-ttu-id="d6d14-2526">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="d6d14-2526">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d6d14-2527">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2527">June 5, 2018</span></span>

<span data-ttu-id="d6d14-2528">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d6d14-2528">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2529">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2529">Interactive</span></span>

* <span data-ttu-id="d6d14-2530">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2530">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d6d14-2531">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2531">June 5, 2018</span></span>

<span data-ttu-id="d6d14-2532">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d6d14-2532">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2533">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2533">Core</span></span>

* <span data-ttu-id="d6d14-2534">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2534">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d6d14-2535">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="d6d14-2535">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2536">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2536">ACR</span></span>

* <span data-ttu-id="d6d14-2537">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="d6d14-2537">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d6d14-2538">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2538">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d6d14-2539">AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2539">AKS</span></span>

* <span data-ttu-id="d6d14-2540">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="d6d14-2540">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-2541">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2541">Batch</span></span>

* <span data-ttu-id="d6d14-2542">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d6d14-2542">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-2543">IOT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2543">IOT</span></span>

* <span data-ttu-id="d6d14-2544">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="d6d14-2544">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2545">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2545">Network</span></span>

* <span data-ttu-id="d6d14-2546">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2546">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d6d14-2547">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="d6d14-2547">Policy Insights</span></span>

* <span data-ttu-id="d6d14-2548">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2548">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d6d14-2549">ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2549">ARM</span></span>

* <span data-ttu-id="d6d14-2550">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2550">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2551">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2551">SQL</span></span>

* <span data-ttu-id="d6d14-2552">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2552">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d6d14-2553">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2553">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d6d14-2554">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2554">Storage</span></span>

* <span data-ttu-id="d6d14-2555">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2555">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2556">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2556">VM</span></span>

* <span data-ttu-id="d6d14-2557">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2557">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d6d14-2558">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2558">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d6d14-2559">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2559">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d6d14-2560">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2560">May 22, 2018</span></span>

<span data-ttu-id="d6d14-2561">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d6d14-2561">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2562">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2562">Core</span></span>

* <span data-ttu-id="d6d14-2563">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2563">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2564">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2564">ACS</span></span>

* <span data-ttu-id="d6d14-2565">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2565">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d6d14-2566">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-2566">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2567">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2567">AppService</span></span>

* <span data-ttu-id="d6d14-2568">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="d6d14-2568">Improved generic update commands</span></span>
* <span data-ttu-id="d6d14-2569">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2569">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2570">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2570">Container</span></span>

* <span data-ttu-id="d6d14-2571">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="d6d14-2571">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d6d14-2572">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2572">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2573">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2573">Extension</span></span>

* <span data-ttu-id="d6d14-2574">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2574">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2575">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2575">Interactive</span></span>

* <span data-ttu-id="d6d14-2576">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="d6d14-2576">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d6d14-2577">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="d6d14-2577">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-2578">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-2578">KeyVault</span></span>

* <span data-ttu-id="d6d14-2579">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-2579">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2580">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2580">Network</span></span>

* <span data-ttu-id="d6d14-2581">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2581">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d6d14-2582">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2582">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2583">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2583">SQL</span></span>

* <span data-ttu-id="d6d14-2584">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2584">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d6d14-2585">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2585">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d6d14-2586">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2586">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="d6d14-2587">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6d14-2587">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d6d14-2588">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2588">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d6d14-2589">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2589">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d6d14-2590">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2590">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d6d14-2591">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2591">`edition`.</span></span> <span data-ttu-id="d6d14-2592">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2592">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d6d14-2593">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2593">`elasticPoolName`.</span></span> <span data-ttu-id="d6d14-2594">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2594">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d6d14-2595">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2595">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d6d14-2596">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2596">`edition`.</span></span> <span data-ttu-id="d6d14-2597">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2597">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d6d14-2598">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2598">`dtu`.</span></span> <span data-ttu-id="d6d14-2599">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2599">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d6d14-2600">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2600">`databaseDtuMin`.</span></span> <span data-ttu-id="d6d14-2601">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2601">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d6d14-2602">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2602">`databaseDtuMax`.</span></span> <span data-ttu-id="d6d14-2603">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2603">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d6d14-2604">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2604">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d6d14-2605">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2605">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2606">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2606">Storage</span></span>

* <span data-ttu-id="d6d14-2607">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2607">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d6d14-2608">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2608">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2609">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2609">VM</span></span>

* <span data-ttu-id="d6d14-2610">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2610">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d6d14-2611">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2611">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d6d14-2612">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2612">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d6d14-2613">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="d6d14-2613">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d6d14-2614">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2614">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d6d14-2615">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2615">May 7, 2018</span></span>

<span data-ttu-id="d6d14-2616">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d6d14-2616">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2617">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2617">Core</span></span>

* <span data-ttu-id="d6d14-2618">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2618">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d6d14-2619">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="d6d14-2619">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d6d14-2620">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2620">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d6d14-2621">#5591</span><span class="sxs-lookup"><span data-stu-id="d6d14-2621">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d6d14-2622">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2622">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d6d14-2623">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="d6d14-2623">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d6d14-2624">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2624">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d6d14-2625">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2625">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d6d14-2626">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="d6d14-2626">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2627">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2627">ACR</span></span>

* <span data-ttu-id="d6d14-2628">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2628">Added ACR Build commands</span></span>
* <span data-ttu-id="d6d14-2629">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-2629">Improved resource not found error messages</span></span>
* <span data-ttu-id="d6d14-2630">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="d6d14-2630">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d6d14-2631">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2631">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d6d14-2632">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2632">Improved repository commands error messages</span></span>
* <span data-ttu-id="d6d14-2633">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2633">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2634">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2634">ACS</span></span>

* <span data-ttu-id="d6d14-2635">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-2635">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d6d14-2636">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2636">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d6d14-2637">AMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2637">AMS</span></span>

* <span data-ttu-id="d6d14-2638">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-2638">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2639">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2639">Appservice</span></span>

* <span data-ttu-id="d6d14-2640">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2640">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d6d14-2641">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2641">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d6d14-2642">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-2642">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d6d14-2643">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="d6d14-2643">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d6d14-2644">Lote AI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2644">Batch AI</span></span>

* <span data-ttu-id="d6d14-2645">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-2645">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d6d14-2646">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2646">Cognitive Services</span></span>

* <span data-ttu-id="d6d14-2647">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create`[#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2647">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-2648">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2648">Consumption</span></span>

* <span data-ttu-id="d6d14-2649">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2649">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2650">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2650">Container</span></span>

* <span data-ttu-id="d6d14-2651">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-2651">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d6d14-2652">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2652">Cosmos DB</span></span>

* <span data-ttu-id="d6d14-2653">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2653">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d6d14-2654">DMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2654">DMS</span></span>

* <span data-ttu-id="d6d14-2655">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-2655">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2656">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2656">Extension</span></span>

* <span data-ttu-id="d6d14-2657">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2657">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2658">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2658">Interactive</span></span>

* <span data-ttu-id="d6d14-2659">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="d6d14-2659">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d6d14-2660">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="d6d14-2660">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d6d14-2661">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-2661">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d6d14-2662">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-2662">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d6d14-2663">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-2663">Lab</span></span>

* <span data-ttu-id="d6d14-2664">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2664">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2665">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2665">Network</span></span>

* <span data-ttu-id="d6d14-2666">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2666">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d6d14-2667">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2667">Profile</span></span>

* <span data-ttu-id="d6d14-2668">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="d6d14-2668">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d6d14-2669">[ALTERAÇÃO SIGNIFICATIVA]`--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2669">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d6d14-2670">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2670">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-2671">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-2671">Redis</span></span>

* <span data-ttu-id="d6d14-2672">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2672">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d6d14-2673">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2673">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d6d14-2674">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2674">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d6d14-2675">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2675">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d6d14-2676">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2676">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2677">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2677">Role</span></span>

* <span data-ttu-id="d6d14-2678">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2678">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2679">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2679">Storage</span></span>

* <span data-ttu-id="d6d14-2680">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2680">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d6d14-2681">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="d6d14-2681">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d6d14-2682">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2682">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d6d14-2683">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="d6d14-2683">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d6d14-2684">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="d6d14-2684">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2685">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2685">VM</span></span>

* <span data-ttu-id="d6d14-2686">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2686">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d6d14-2687">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-2687">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d6d14-2688">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2688">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d6d14-2689">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2689">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d6d14-2690">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2690">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d6d14-2691">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="d6d14-2691">Added write accelerator support</span></span>
* <span data-ttu-id="d6d14-2692">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2692">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d6d14-2693">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="d6d14-2693">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d6d14-2694">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="d6d14-2694">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d6d14-2695">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2695">April 10, 2018</span></span>

<span data-ttu-id="d6d14-2696">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d6d14-2696">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2697">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2697">ACR</span></span>

* <span data-ttu-id="d6d14-2698">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="d6d14-2698">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2699">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2699">ACS</span></span>

* <span data-ttu-id="d6d14-2700">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2700">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2701">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2701">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d6d14-2703">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2703">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-2704">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2704">BatchAI</span></span>

* <span data-ttu-id="d6d14-2705">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-2705">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="d6d14-2706">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-2706">Job level mounting</span></span>
  - <span data-ttu-id="d6d14-2707">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2707">Environment variables with secret values</span></span>
  - <span data-ttu-id="d6d14-2708">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="d6d14-2708">Performance counters settings</span></span>
  - <span data-ttu-id="d6d14-2709">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-2709">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="d6d14-2710">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="d6d14-2710">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="d6d14-2711">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="d6d14-2711">Usage and limits reporting</span></span>
  - <span data-ttu-id="d6d14-2712">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2712">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="d6d14-2713">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2713">Support for custom images</span></span>
  - <span data-ttu-id="d6d14-2714">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="d6d14-2714">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d6d14-2715">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-2715">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d6d14-2716">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="d6d14-2716">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d6d14-2717">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="d6d14-2717">National clouds are supported</span></span>
* <span data-ttu-id="d6d14-2718">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="d6d14-2718">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d6d14-2719">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2719">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d6d14-2720">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-2720">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d6d14-2721">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2721">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d6d14-2722">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2722">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d6d14-2723">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2723">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d6d14-2724">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2724">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d6d14-2725">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2725">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d6d14-2726">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="d6d14-2726">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d6d14-2727">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2727">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d6d14-2728">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-2728">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d6d14-2729">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2729">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d6d14-2730">[ALTERAÇÃO SIGNIFICATIVA]`--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2730">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d6d14-2731">Cobrança</span><span class="sxs-lookup"><span data-stu-id="d6d14-2731">Billing</span></span>

* <span data-ttu-id="d6d14-2732">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="d6d14-2732">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-2733">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2733">Consumption</span></span>

* <span data-ttu-id="d6d14-2734">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2734">Added `marketplace` commands</span></span>
* <span data-ttu-id="d6d14-2735">[ALTERAÇÃO SIGNIFICATIVA]`reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2735">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d6d14-2736">[ALTERAÇÃO SIGNIFICATIVA]`reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2736">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d6d14-2737">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2737">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d6d14-2738">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2738">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d6d14-2739">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2739">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2740">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2740">Container</span></span>

* <span data-ttu-id="d6d14-2741">Adição dos parâmetros de montagem de volume do Repositório Git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2741">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d6d14-2742">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2742">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2743">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2743">Extension</span></span>

* <span data-ttu-id="d6d14-2744">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="d6d14-2744">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2745">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2745">Interactive</span></span>

* <span data-ttu-id="d6d14-2746">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2746">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d6d14-2747">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-2747">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d6d14-2748">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2748">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2749">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2749">Network</span></span>

* <span data-ttu-id="d6d14-2750">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2750">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d6d14-2751">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2751">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d6d14-2752">#4910</span><span class="sxs-lookup"><span data-stu-id="d6d14-2752">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d6d14-2753">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2753">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="d6d14-2754">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2754">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d6d14-2755">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2755">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d6d14-2756">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2756">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d6d14-2757">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2757">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-2758">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2758">Profile</span></span>

* <span data-ttu-id="d6d14-2759">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2759">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d6d14-2760">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2760">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2761">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2761">RDBMS</span></span>

* <span data-ttu-id="d6d14-2762">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2762">Added `georestore` command</span></span>
* <span data-ttu-id="d6d14-2763">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2763">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2764">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2764">Resource</span></span>

* <span data-ttu-id="d6d14-2765">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2765">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d6d14-2766">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2766">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2767">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2767">SQL</span></span>

* <span data-ttu-id="d6d14-2768">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2768">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2769">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2769">Storage</span></span>

* <span data-ttu-id="d6d14-2770">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2770">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2771">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2771">VM</span></span>

* <span data-ttu-id="d6d14-2772">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2772">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d6d14-2773">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2773">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d6d14-2775">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2775">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d6d14-2776">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2776">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d6d14-2777">#5718</span><span class="sxs-lookup"><span data-stu-id="d6d14-2777">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d6d14-2778">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="d6d14-2778">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d6d14-2779">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2779">March 27, 2018</span></span>

<span data-ttu-id="d6d14-2780">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d6d14-2780">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2781">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2781">Core</span></span>

* <span data-ttu-id="d6d14-2782">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="d6d14-2782">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2783">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2783">ACS</span></span>

* <span data-ttu-id="d6d14-2784">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d6d14-2784">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2785">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2785">Appservice</span></span>

* <span data-ttu-id="d6d14-2786">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2786">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d6d14-2787">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2787">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-2788">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-2788">Backup</span></span>

* <span data-ttu-id="d6d14-2789">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2789">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d6d14-2790">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-2790">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d6d14-2791">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2791">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d6d14-2792">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2792">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2793">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2793">Container</span></span>

* <span data-ttu-id="d6d14-2794">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2794">Added `container exec` command.</span></span> <span data-ttu-id="d6d14-2795">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="d6d14-2795">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d6d14-2796">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2796">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2797">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2797">Extension</span></span>

* <span data-ttu-id="d6d14-2798">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-2798">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d6d14-2799">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2799">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d6d14-2800">[ALTERAÇÃO SIGNIFICATIVA]`extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2800">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2801">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2801">Interactive</span></span>

* <span data-ttu-id="d6d14-2802">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2802">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d6d14-2803">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2803">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d6d14-2804">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2804">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d6d14-2805">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="d6d14-2805">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d6d14-2806">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-2806">Lab</span></span>

* <span data-ttu-id="d6d14-2807">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2807">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2808">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2808">Monitor</span></span>

* <span data-ttu-id="d6d14-2809">Adicionado suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2809">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d6d14-2810">Corrigido [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="d6d14-2810">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d6d14-2811">Suporte adicionado para `--namespace` a `metrics list-definitions` [nº5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2811">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2812">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2812">Network</span></span>

* <span data-ttu-id="d6d14-2813">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="d6d14-2813">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-2814">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2814">Profile</span></span>

* <span data-ttu-id="d6d14-2815">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2815">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2816">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2816">RDBMS</span></span>

* <span data-ttu-id="d6d14-2817">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-2817">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2818">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2818">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d6d14-2820">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2820">Role</span></span>

* <span data-ttu-id="d6d14-2821">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2821">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d6d14-2822">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="d6d14-2822">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d6d14-2823">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2823">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d6d14-2824">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2824">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d6d14-2825">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2825">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2826">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2826">Storage</span></span>

* <span data-ttu-id="d6d14-2827">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2827">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d6d14-2828">Corrigido [#4049](https://github.com/Azure/azure-cli/issues/4049): problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="d6d14-2828">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2829">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2829">VM</span></span>

* <span data-ttu-id="d6d14-2830">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="d6d14-2830">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d6d14-2831">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2831">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d6d14-2832">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2832">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d6d14-2833">[ALTERAÇÃO SIGNIFICATIVA]`vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="d6d14-2833">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d6d14-2834">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2834">March 13, 2018</span></span>

<span data-ttu-id="d6d14-2835">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d6d14-2835">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-2836">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-2836">ACR</span></span>

* <span data-ttu-id="d6d14-2837">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2837">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d6d14-2838">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2838">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d6d14-2839">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2839">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2840">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2840">ACS</span></span>

* <span data-ttu-id="d6d14-2841">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2841">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d6d14-2842">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="d6d14-2842">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d6d14-2843">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d6d14-2843">Advisor</span></span>

* <span data-ttu-id="d6d14-2844">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2844">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d6d14-2845">[ALTERAÇÃO SIGNIFICATIVA]`advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2845">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d6d14-2846">[ALTERAÇÃO SIGNIFICATIVA]`advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2846">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="d6d14-2847">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2847">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d6d14-2848">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2848">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2849">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2849">Appservice</span></span>

* <span data-ttu-id="d6d14-2850">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2850">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d6d14-2851">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2851">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d6d14-2852">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2852">Eventhubs</span></span>

* <span data-ttu-id="d6d14-2853">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2853">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2854">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2854">Extension</span></span>

* <span data-ttu-id="d6d14-2855">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="d6d14-2855">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2856">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2856">Interactive</span></span>

* <span data-ttu-id="d6d14-2857">Corrigido [#5625](https://github.com/Azure/azure-cli/issues/5625): manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2857">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d6d14-2858">Corrigido [#3016](https://github.com/Azure/azure-cli/issues/3016): histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2858">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d6d14-2859">Corrigido [#5688](https://github.com/Azure/azure-cli/issues/5688): as conclusões não aparecerão se o carregamento da tabela de comando encontrar uma exceção</span><span class="sxs-lookup"><span data-stu-id="d6d14-2859">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d6d14-2860">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="d6d14-2860">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2861">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2861">Monitor</span></span>

* <span data-ttu-id="d6d14-2862">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2862">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d6d14-2863">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2863">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d6d14-2864">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2864">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d6d14-2865">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2865">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2866">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2866">Network</span></span>

* <span data-ttu-id="d6d14-2867">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2867">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d6d14-2868">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2868">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d6d14-2869">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-2869">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d6d14-2870">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2870">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-2871">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2871">Profile</span></span>

* <span data-ttu-id="d6d14-2872">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2872">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d6d14-2873">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2873">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-2874">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2874">RDBMS</span></span>

* <span data-ttu-id="d6d14-2875">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="d6d14-2875">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d6d14-2876">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2876">Service Bus</span></span>

* <span data-ttu-id="d6d14-2877">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-2877">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2878">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2878">Storage</span></span>

* <span data-ttu-id="d6d14-2879">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-2879">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d6d14-2880">Corrigido [#5286](https://github.com/Azure/azure-cli/issues/5286): os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="d6d14-2880">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2881">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2881">VM</span></span>

* <span data-ttu-id="d6d14-2882">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="d6d14-2882">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d6d14-2883">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2883">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d6d14-2884">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2884">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d6d14-2885">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="d6d14-2885">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d6d14-2886">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2886">February 27, 2018</span></span>

<span data-ttu-id="d6d14-2887">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d6d14-2887">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2888">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2888">Core</span></span>

* <span data-ttu-id="d6d14-2889">Corrigido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="d6d14-2889">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d6d14-2890">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="d6d14-2890">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d6d14-2891">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2891">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2892">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2892">ACS</span></span>

* <span data-ttu-id="d6d14-2893">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2893">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d6d14-2894">Problema corrigido: permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2894">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d6d14-2895">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2895">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d6d14-2896">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2896">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2897">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2897">Appservice</span></span>

* <span data-ttu-id="d6d14-2898">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d6d14-2898">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d6d14-2899">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2899">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d6d14-2900">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2900">Cognitive Services</span></span>

* <span data-ttu-id="d6d14-2901">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2901">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-2902">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2902">Consumption</span></span>

* <span data-ttu-id="d6d14-2903">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="d6d14-2903">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d6d14-2904">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="d6d14-2904">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2905">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2905">Container</span></span>

* <span data-ttu-id="d6d14-2906">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2906">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2907">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2907">Network</span></span>

* <span data-ttu-id="d6d14-2908">Corrigido [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2908">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2909">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2909">Resource</span></span>

* <span data-ttu-id="d6d14-2910">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="d6d14-2910">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2911">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2911">Role</span></span>

* <span data-ttu-id="d6d14-2912">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-2912">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2913">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2913">SQL</span></span>

* <span data-ttu-id="d6d14-2914">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-2914">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2915">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2915">Storage</span></span>

* <span data-ttu-id="d6d14-2916">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2916">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2917">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2917">VM</span></span>

* <span data-ttu-id="d6d14-2918">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2918">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d6d14-2919">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2919">February 13, 2018</span></span>

<span data-ttu-id="d6d14-2920">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d6d14-2920">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2921">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2921">Core</span></span>

* <span data-ttu-id="d6d14-2922">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2922">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2923">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2923">ACS</span></span>

* <span data-ttu-id="d6d14-2924">[ALTERAÇÃO SIGNIFICATIVA]`aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2924">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d6d14-2925">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2925">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d6d14-2926">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2926">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d6d14-2927">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2927">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d6d14-2928">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="d6d14-2928">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d6d14-2929">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2929">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d6d14-2930">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2930">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d6d14-2931">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2931">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2932">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2932">Appservice</span></span>

* <span data-ttu-id="d6d14-2933">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="d6d14-2933">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d6d14-2934">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2934">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-2935">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-2935">CDN</span></span>

* <span data-ttu-id="d6d14-2936">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2936">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-2937">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2937">Container</span></span>

* <span data-ttu-id="d6d14-2938">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="d6d14-2938">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d6d14-2939">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-2939">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-2940">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2940">CosmosDB</span></span>

* <span data-ttu-id="d6d14-2941">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="d6d14-2941">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-2942">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-2942">Extension</span></span>

* <span data-ttu-id="d6d14-2943">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2943">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d6d14-2944">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2944">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d6d14-2945">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6d14-2945">Feedback</span></span>

* <span data-ttu-id="d6d14-2946">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="d6d14-2946">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2947">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2947">Interactive</span></span>

* <span data-ttu-id="d6d14-2948">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d6d14-2948">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d6d14-2949">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-2949">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-2950">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-2950">IoT</span></span>

* <span data-ttu-id="d6d14-2951">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2951">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d6d14-2952">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2952">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d6d14-2953">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2953">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d6d14-2954">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="d6d14-2954">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-2955">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2955">Monitor</span></span>

* <span data-ttu-id="d6d14-2956">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2956">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2957">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2957">Network</span></span>

* <span data-ttu-id="d6d14-2958">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="d6d14-2958">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d6d14-2959">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-2959">Profile</span></span>

* <span data-ttu-id="d6d14-2960">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2960">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-2961">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-2961">Resource</span></span>

* <span data-ttu-id="d6d14-2962">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-2962">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-2963">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-2963">Role</span></span>

* <span data-ttu-id="d6d14-2964">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2964">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-2965">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-2965">SQL</span></span>

* <span data-ttu-id="d6d14-2966">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2966">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d6d14-2967">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2967">Added `sql db rename`</span></span>
* <span data-ttu-id="d6d14-2968">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="d6d14-2968">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-2969">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-2969">Storage</span></span>

* <span data-ttu-id="d6d14-2970">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="d6d14-2970">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-2971">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-2971">VM</span></span>

* <span data-ttu-id="d6d14-2972">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2972">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d6d14-2973">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2973">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d6d14-2974">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2974">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d6d14-2975">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-2975">January 31, 2018</span></span>

<span data-ttu-id="d6d14-2976">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d6d14-2976">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-2977">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2977">Core</span></span>

* <span data-ttu-id="d6d14-2978">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-2978">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d6d14-2979">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="d6d14-2979">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d6d14-2980">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="d6d14-2980">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d6d14-2981">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="d6d14-2981">Use `--verbose` to see</span></span>
* <span data-ttu-id="d6d14-2982">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="d6d14-2982">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-2983">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-2983">ACS</span></span>

* <span data-ttu-id="d6d14-2984">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-2984">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d6d14-2985">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2985">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-2986">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-2986">Appservice</span></span>

* <span data-ttu-id="d6d14-2987">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2987">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d6d14-2988">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="d6d14-2988">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-2989">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-2989">CDN</span></span>

* <span data-ttu-id="d6d14-2990">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2990">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-2991">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-2991">CosmosDB</span></span>

* <span data-ttu-id="d6d14-2992">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="d6d14-2992">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-2993">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-2993">Interactive</span></span>

* <span data-ttu-id="d6d14-2994">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="d6d14-2994">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-2995">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-2995">Network</span></span>

* <span data-ttu-id="d6d14-2996">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2996">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d6d14-2997">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="d6d14-2997">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d6d14-2998">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2998">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d6d14-2999">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-2999">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d6d14-3000">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3000">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d6d14-3001">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3001">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d6d14-3002">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3002">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d6d14-3003">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="d6d14-3003">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d6d14-3004">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3004">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="d6d14-3005">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3005">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3006">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3006">Profile</span></span>

* <span data-ttu-id="d6d14-3007">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="d6d14-3007">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3008">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3008">Resource</span></span>

* <span data-ttu-id="d6d14-3009">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3009">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3010">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3010">Storage</span></span>

* <span data-ttu-id="d6d14-3011">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="d6d14-3011">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d6d14-3012">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="d6d14-3012">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d6d14-3013">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3013">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="d6d14-3014">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3014">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d6d14-3015">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="d6d14-3015">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3016">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3016">VM</span></span>

* <span data-ttu-id="d6d14-3017">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="d6d14-3017">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d6d14-3018">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3018">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d6d14-3019">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3019">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d6d14-3020">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3020">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d6d14-3021">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="d6d14-3021">January 17, 2018</span></span>

<span data-ttu-id="d6d14-3022">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d6d14-3022">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-3023">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3023">ACR</span></span>

* <span data-ttu-id="d6d14-3024">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-3024">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d6d14-3025">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="d6d14-3025">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3026">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3026">ACS</span></span>

* <span data-ttu-id="d6d14-3027">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3027">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d6d14-3028">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3028">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3029">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3029">Appservice</span></span>

* <span data-ttu-id="d6d14-3030">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3030">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d6d14-3031">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3031">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d6d14-3032">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3032">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-3033">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-3033">Backup</span></span>

* <span data-ttu-id="d6d14-3034">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="d6d14-3034">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d6d14-3035">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3035">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d6d14-3036">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3036">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d6d14-3037">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="d6d14-3037">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d6d14-3038">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3038">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-3039">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3039">Batch</span></span>

* <span data-ttu-id="d6d14-3040">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="d6d14-3040">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d6d14-3041">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3041">Cloud</span></span>

* <span data-ttu-id="d6d14-3042">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3042">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-3043">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3043">Consumption</span></span>

* <span data-ttu-id="d6d14-3044">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3044">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d6d14-3045">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3045">Event Grid</span></span>

* <span data-ttu-id="d6d14-3046">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3046">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d6d14-3047">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3047">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d6d14-3048">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3048">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d6d14-3049">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3049">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d6d14-3050">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3050">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d6d14-3051">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3051">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d6d14-3052">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3052">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d6d14-3053">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3053">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-3054">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3054">Interactive</span></span>

* <span data-ttu-id="d6d14-3055">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="d6d14-3055">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d6d14-3056">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="d6d14-3056">Fixed errors on startup</span></span>
* <span data-ttu-id="d6d14-3057">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3057">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-3058">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-3058">IoT</span></span>

* <span data-ttu-id="d6d14-3059">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3059">Added support for device provisioning service</span></span>
* <span data-ttu-id="d6d14-3060">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-3060">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d6d14-3061">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-3061">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3062">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3062">Monitor</span></span>

* <span data-ttu-id="d6d14-3063">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3063">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d6d14-3064">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3064">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d6d14-3065">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3065">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3066">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3066">Network</span></span>

* <span data-ttu-id="d6d14-3067">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3067">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d6d14-3068">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3068">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3069">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3069">Profile</span></span>

* <span data-ttu-id="d6d14-3070">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-3070">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-3071">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-3071">Role</span></span>

* <span data-ttu-id="d6d14-3072">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3072">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d6d14-3073">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-3073">Service Fabric</span></span>

* <span data-ttu-id="d6d14-3074">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="d6d14-3074">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d6d14-3075">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3075">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3076">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3076">VM</span></span>

* <span data-ttu-id="d6d14-3077">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3077">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d6d14-3078">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="d6d14-3078">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d6d14-3079">[ALTERAÇÃO SIGNIFICATIVA]`externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="d6d14-3079">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d6d14-3080">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d6d14-3080">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d6d14-3081">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3081">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d6d14-3082">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3082">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d6d14-3083">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3083">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d6d14-3084">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3084">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d6d14-3085">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3085">December 19, 2017</span></span>

<span data-ttu-id="d6d14-3086">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d6d14-3086">Version 2.0.23</span></span>

* <span data-ttu-id="d6d14-3087">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="d6d14-3087">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-3088">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3088">Container</span></span>

* <span data-ttu-id="d6d14-3089">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3089">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3090">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3090">Network</span></span>

* <span data-ttu-id="d6d14-3091">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3091">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d6d14-3092">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3092">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3093">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3093">Storage</span></span>

* <span data-ttu-id="d6d14-3094">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="d6d14-3094">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3095">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3095">VM</span></span>

* <span data-ttu-id="d6d14-3096">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3096">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d6d14-3097">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3097">December 5, 2017</span></span>

<span data-ttu-id="d6d14-3098">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d6d14-3098">Version 2.0.22</span></span>

* <span data-ttu-id="d6d14-3099">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3099">Removed `az component` commands.</span></span> <span data-ttu-id="d6d14-3100">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3100">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-3101">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3101">Core</span></span>
* <span data-ttu-id="d6d14-3102">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="d6d14-3102">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d6d14-3103">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3103">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3104">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3104">ACS</span></span>

* <span data-ttu-id="d6d14-3105">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3105">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d6d14-3106">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3106">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d6d14-3107">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3107">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d6d14-3108">Supervisor</span><span class="sxs-lookup"><span data-stu-id="d6d14-3108">Advisor</span></span>

* <span data-ttu-id="d6d14-3109">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-3109">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3110">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3110">Appservice</span></span>

* <span data-ttu-id="d6d14-3111">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3111">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d6d14-3112">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3112">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d6d14-3113">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3113">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d6d14-3114">Consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3114">Consumption</span></span>

* <span data-ttu-id="d6d14-3115">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3115">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-3116">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3116">Container</span></span>

* <span data-ttu-id="d6d14-3117">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3117">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3118">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3118">Monitor</span></span>

* <span data-ttu-id="d6d14-3119">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3119">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3120">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3120">Resource</span></span>

* <span data-ttu-id="d6d14-3121">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3121">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-3122">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-3122">Role</span></span>

* <span data-ttu-id="d6d14-3123">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3123">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d6d14-3124">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="d6d14-3124">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d6d14-3125">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3125">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3126">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3126">SQL</span></span>

* <span data-ttu-id="d6d14-3127">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3127">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d6d14-3128">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3128">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3129">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3129">VM</span></span>

* <span data-ttu-id="d6d14-3130">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3130">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d6d14-3131">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3131">November 14, 2017</span></span>

<span data-ttu-id="d6d14-3132">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d6d14-3132">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-3133">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3133">ACR</span></span>

* <span data-ttu-id="d6d14-3134">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="d6d14-3134">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d6d14-3135">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3135">ACS</span></span>

* <span data-ttu-id="d6d14-3136">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3136">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d6d14-3137">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3137">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d6d14-3138">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3138">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d6d14-3139">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-3139">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d6d14-3140">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="d6d14-3140">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3141">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3141">Appservice</span></span>

* <span data-ttu-id="d6d14-3142">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="d6d14-3142">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d6d14-3143">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3143">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d6d14-3144">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3144">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d6d14-3145">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3145">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d6d14-3146">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-3146">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d6d14-3147">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3147">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-3148">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3148">Batch</span></span>

* <span data-ttu-id="d6d14-3149">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3149">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-3150">Batchai</span><span class="sxs-lookup"><span data-stu-id="d6d14-3150">Batchai</span></span>

* <span data-ttu-id="d6d14-3151">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3151">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d6d14-3152">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3152">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d6d14-3153">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3153">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d6d14-3154">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3154">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d6d14-3155">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3155">Cloud</span></span>

* <span data-ttu-id="d6d14-3156">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="d6d14-3156">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-3157">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3157">Container</span></span>

* <span data-ttu-id="d6d14-3158">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3158">Added support to open multiple ports</span></span>
* <span data-ttu-id="d6d14-3159">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3159">Added container group restart policy</span></span>
* <span data-ttu-id="d6d14-3160">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="d6d14-3160">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d6d14-3161">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3161">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d6d14-3162">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-3162">Data Lake Analytics</span></span>

* <span data-ttu-id="d6d14-3163">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3163">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d6d14-3164">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3164">Data Lake Store</span></span>

* <span data-ttu-id="d6d14-3165">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3165">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-3166">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3166">Extension</span></span>

* <span data-ttu-id="d6d14-3167">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="d6d14-3167">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d6d14-3168">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="d6d14-3168">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-3169">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-3169">IoT</span></span>

* <span data-ttu-id="d6d14-3170">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3170">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3171">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3171">Monitor</span></span>

* <span data-ttu-id="d6d14-3172">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3172">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3173">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3173">Network</span></span>

* <span data-ttu-id="d6d14-3174">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="d6d14-3174">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d6d14-3175">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3175">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d6d14-3176">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3176">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d6d14-3177">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3177">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d6d14-3178">Reservas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3178">Reservations</span></span>

* <span data-ttu-id="d6d14-3179">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-3179">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3180">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3180">Resource</span></span>

* <span data-ttu-id="d6d14-3181">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3181">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3182">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3182">SQL</span></span>

* <span data-ttu-id="d6d14-3183">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3183">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3184">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3184">Storage</span></span>

* <span data-ttu-id="d6d14-3185">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3185">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d6d14-3186">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="d6d14-3186">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d6d14-3187">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3187">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d6d14-3188">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3188">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d6d14-3189">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3189">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d6d14-3190">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3190">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d6d14-3191">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3191">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3192">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3192">VM</span></span>

* <span data-ttu-id="d6d14-3193">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3193">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d6d14-3194">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="d6d14-3194">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d6d14-3195">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3195">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d6d14-3196">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3196">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d6d14-3197">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3197">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d6d14-3198">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3198">October 24, 2017</span></span>

<span data-ttu-id="d6d14-3199">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d6d14-3199">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-3200">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3200">Core</span></span>

* <span data-ttu-id="d6d14-3201">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3201">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-3202">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3202">ACR</span></span>

* <span data-ttu-id="d6d14-3203">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3203">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d6d14-3204">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3204">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d6d14-3205">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="d6d14-3205">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3206">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3206">ACS</span></span>

* <span data-ttu-id="d6d14-3207">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3207">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d6d14-3208">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="d6d14-3208">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3209">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3209">Appservice</span></span>

* <span data-ttu-id="d6d14-3210">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3210">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d6d14-3211">Componente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3211">Component</span></span>

* <span data-ttu-id="d6d14-3212">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="d6d14-3212">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3213">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3213">Monitor</span></span>

* <span data-ttu-id="d6d14-3214">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3214">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3215">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3215">Resource</span></span>

* <span data-ttu-id="d6d14-3216">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3216">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d6d14-3217">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3217">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3218">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3218">VM</span></span>

* <span data-ttu-id="d6d14-3219">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3219">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d6d14-3220">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3220">October 9, 2017</span></span>

<span data-ttu-id="d6d14-3221">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d6d14-3221">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-3222">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3222">Core</span></span>

* <span data-ttu-id="d6d14-3223">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d6d14-3223">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3224">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3224">Appservice</span></span>

* <span data-ttu-id="d6d14-3225">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3225">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-3226">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3226">Batch</span></span>

* <span data-ttu-id="d6d14-3227">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-3227">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d6d14-3228">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="d6d14-3228">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d6d14-3229">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3229">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d6d14-3230">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3230">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d6d14-3231">Batchai</span><span class="sxs-lookup"><span data-stu-id="d6d14-3231">Batchai</span></span>

* <span data-ttu-id="d6d14-3232">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3232">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-3233">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-3233">Keyvault</span></span>

* <span data-ttu-id="d6d14-3234">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3234">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d6d14-3235">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3235">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d6d14-3236">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3236">Network</span></span>

* <span data-ttu-id="d6d14-3237">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="d6d14-3237">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d6d14-3238">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3238">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3239">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3239">Resource</span></span>

* <span data-ttu-id="d6d14-3240">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3240">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d6d14-3241">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-3241">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d6d14-3242">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3242">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d6d14-3243">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3243">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3244">Sql</span><span class="sxs-lookup"><span data-stu-id="d6d14-3244">Sql</span></span>

* <span data-ttu-id="d6d14-3245">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="d6d14-3245">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d6d14-3246">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3246">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d6d14-3247">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3247">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3248">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3248">Storage</span></span>

* <span data-ttu-id="d6d14-3249">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3249">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3250">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3250">Vm</span></span>

* <span data-ttu-id="d6d14-3251">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3251">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d6d14-3252">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3252">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d6d14-3253">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3253">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d6d14-3254">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3254">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d6d14-3255">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3255">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d6d14-3256">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3256">September 22, 2017</span></span>

<span data-ttu-id="d6d14-3257">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="d6d14-3257">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3258">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3258">Resource</span></span>

* <span data-ttu-id="d6d14-3259">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3259">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d6d14-3260">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="d6d14-3260">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d6d14-3261">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3261">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d6d14-3262">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3262">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3263">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3263">Network</span></span>

* <span data-ttu-id="d6d14-3264">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3264">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d6d14-3265">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3265">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d6d14-3266">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3266">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d6d14-3267">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3267">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d6d14-3268">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3268">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d6d14-3269">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3269">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d6d14-3270">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3270">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3271">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3271">Storage</span></span>

* <span data-ttu-id="d6d14-3272">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="d6d14-3272">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d6d14-3273">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3273">Eventgrid</span></span>

* <span data-ttu-id="d6d14-3274">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="d6d14-3274">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3275">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3275">SQL</span></span>

* <span data-ttu-id="d6d14-3276">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3276">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d6d14-3277">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3277">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d6d14-3278">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3278">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-3279">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-3279">Keyvault</span></span>

* <span data-ttu-id="d6d14-3280">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="d6d14-3280">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3281">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3281">VM</span></span>

* <span data-ttu-id="d6d14-3282">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3282">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d6d14-3283">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="d6d14-3283">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d6d14-3284">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3284">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d6d14-3285">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3285">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d6d14-3286">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3286">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d6d14-3287">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3287">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3288">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3288">ACS</span></span>

* <span data-ttu-id="d6d14-3289">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3289">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3290">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3290">Appservice</span></span>

* <span data-ttu-id="d6d14-3291">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3291">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d6d14-3292">Backup</span><span class="sxs-lookup"><span data-stu-id="d6d14-3292">Backup</span></span>

* <span data-ttu-id="d6d14-3293">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-3293">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d6d14-3294">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3294">September 11, 2017</span></span>

<span data-ttu-id="d6d14-3295">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d6d14-3295">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d6d14-3296">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3296">Core</span></span>

* <span data-ttu-id="d6d14-3297">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="d6d14-3297">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d6d14-3298">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3298">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3299">Acs</span><span class="sxs-lookup"><span data-stu-id="d6d14-3299">Acs</span></span>

* <span data-ttu-id="d6d14-3300">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3300">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d6d14-3301">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3301">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3302">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3302">Appservice</span></span>

* <span data-ttu-id="d6d14-3303">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3303">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-3304">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3304">CDN</span></span>

* <span data-ttu-id="d6d14-3305">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3305">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d6d14-3306">Extensão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3306">Extension</span></span>

* <span data-ttu-id="d6d14-3307">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-3307">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-3308">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-3308">Keyvault</span></span>

* <span data-ttu-id="d6d14-3309">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3309">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3310">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3310">Network</span></span>

* <span data-ttu-id="d6d14-3311">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3311">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d6d14-3312">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3312">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d6d14-3313">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3313">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d6d14-3314">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3314">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d6d14-3315">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3315">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3316">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3316">Resource</span></span>

* <span data-ttu-id="d6d14-3317">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3317">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d6d14-3318">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3318">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d6d14-3319">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="d6d14-3319">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d6d14-3320">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3320">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3321">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3321">SQL</span></span>

* <span data-ttu-id="d6d14-3322">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3322">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3323">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3323">VM</span></span>

* <span data-ttu-id="d6d14-3324">Corrigido: não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="d6d14-3324">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d6d14-3325">Corrigido: usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="d6d14-3325">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d6d14-3326">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3326">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d6d14-3327">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3327">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d6d14-3328">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="d6d14-3328">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d6d14-3329">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3329">August 31, 2017</span></span>

<span data-ttu-id="d6d14-3330">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d6d14-3330">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-3331">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d6d14-3331">Keyvault</span></span>

* <span data-ttu-id="d6d14-3332">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3332">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d6d14-3333">Sf</span><span class="sxs-lookup"><span data-stu-id="d6d14-3333">Sf</span></span>

* <span data-ttu-id="d6d14-3334">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3334">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3335">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3335">Storage</span></span>

* <span data-ttu-id="d6d14-3336">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="d6d14-3336">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d6d14-3337">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3337">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d6d14-3338">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3338">August 28, 2017</span></span>

<span data-ttu-id="d6d14-3339">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d6d14-3339">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d6d14-3340">CLI</span><span class="sxs-lookup"><span data-stu-id="d6d14-3340">CLI</span></span>

* <span data-ttu-id="d6d14-3341">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3341">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3342">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3342">ACS</span></span>

* <span data-ttu-id="d6d14-3343">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-3343">Corrected preview regions</span></span>
* <span data-ttu-id="d6d14-3344">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3344">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d6d14-3345">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3345">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3346">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3346">Appservice</span></span>

* <span data-ttu-id="d6d14-3347">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3347">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d6d14-3348">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3348">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d6d14-3349">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3349">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d6d14-3350">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3350">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d6d14-3351">Corrigido: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3351">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-3352">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-3352">IoT</span></span>

* <span data-ttu-id="d6d14-3353">Corrigido #3934: a criação de uma política não limpa mais as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3353">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3354">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3354">Network</span></span>

* <span data-ttu-id="d6d14-3355">[ALTERAÇÃO SIGNIFICATIVA]`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3355">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d6d14-3356">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3356">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d6d14-3357">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3357">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d6d14-3358">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3358">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d6d14-3359">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3359">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3360">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3360">Profile</span></span>

* <span data-ttu-id="d6d14-3361">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d6d14-3361">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d6d14-3362">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-3362">Service Fabric</span></span>

* <span data-ttu-id="d6d14-3363">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="d6d14-3363">Preview release</span></span>
* <span data-ttu-id="d6d14-3364">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-3364">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d6d14-3365">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d6d14-3365">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d6d14-3366">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="d6d14-3366">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3367">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3367">Storage</span></span>

* <span data-ttu-id="d6d14-3368">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="d6d14-3368">Enabled setting blob tier</span></span>
* <span data-ttu-id="d6d14-3369">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="d6d14-3369">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d6d14-3370">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="d6d14-3370">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d6d14-3371">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3371">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d6d14-3372">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3372">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d6d14-3373">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="d6d14-3373">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3374">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3374">VM</span></span>

* <span data-ttu-id="d6d14-3375">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3375">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d6d14-3376">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3376">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d6d14-3377">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3377">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d6d14-3378">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3378">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d6d14-3379">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="d6d14-3379">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d6d14-3380">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3380">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d6d14-3381">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3381">August 15, 2017</span></span>

<span data-ttu-id="d6d14-3382">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d6d14-3382">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3383">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3383">ACS</span></span>

* <span data-ttu-id="d6d14-3384">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3384">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3385">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3385">Appservice</span></span>

* <span data-ttu-id="d6d14-3386">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="d6d14-3386">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d6d14-3387">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3387">Event Grid</span></span>

* <span data-ttu-id="d6d14-3388">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="d6d14-3388">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d6d14-3389">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3389">August 11, 2017</span></span>

<span data-ttu-id="d6d14-3390">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d6d14-3390">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3391">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3391">ACS</span></span>

* <span data-ttu-id="d6d14-3392">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-3392">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-3393">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3393">Batch</span></span>

* <span data-ttu-id="d6d14-3394">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-3394">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d6d14-3395">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-3395">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d6d14-3396">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3396">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d6d14-3397">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3397">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d6d14-3398">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="d6d14-3398">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d6d14-3399">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="d6d14-3399">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d6d14-3400">Componente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3400">Component</span></span>

* <span data-ttu-id="d6d14-3401">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="d6d14-3401">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d6d14-3402">Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3402">Container</span></span>

* <span data-ttu-id="d6d14-3403">`create`: corrigido o problema em que o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3403">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d6d14-3404">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3404">Data Lake Store</span></span>

* <span data-ttu-id="d6d14-3405">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3405">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d6d14-3406">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3406">Event Grid</span></span>

* <span data-ttu-id="d6d14-3407">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="d6d14-3407">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3408">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3408">Network</span></span>

* <span data-ttu-id="d6d14-3409">`lb`: corrigido o problema em que os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3409">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d6d14-3410">`application-gateway {subresource} delete`: corrigido o problema em que `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3410">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d6d14-3411">`application-gateway http-settings update`: corrigido o problema em que `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3411">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d6d14-3412">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3412">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3413">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3413">Profile</span></span>

* <span data-ttu-id="d6d14-3414">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="d6d14-3414">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3415">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3415">Storage</span></span>

* <span data-ttu-id="d6d14-3416">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="d6d14-3416">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3417">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3417">VM</span></span>

* <span data-ttu-id="d6d14-3418">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3418">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d6d14-3419">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3419">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d6d14-3420">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="d6d14-3420">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d6d14-3421">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3421">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d6d14-3422">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3422">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d6d14-3423">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3423">July 28, 2017</span></span>

<span data-ttu-id="d6d14-3424">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d6d14-3424">Version 2.0.12</span></span>

* <span data-ttu-id="d6d14-3425">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3425">Added container commands</span></span>
* <span data-ttu-id="d6d14-3426">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3426">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d6d14-3427">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3427">Core</span></span>

* <span data-ttu-id="d6d14-3428">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3428">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d6d14-3429">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="d6d14-3429">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d6d14-3430">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="d6d14-3430">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d6d14-3431">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3431">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d6d14-3432">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-3432">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d6d14-3433">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3433">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d6d14-3434">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3434">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d6d14-3435">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3435">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d6d14-3436">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3436">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d6d14-3437">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="d6d14-3437">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d6d14-3438">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3438">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d6d14-3439">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3439">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d6d14-3440">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3440">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d6d14-3441">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d6d14-3441">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d6d14-3442">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d6d14-3442">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d6d14-3443">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3443">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d6d14-3444">ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3444">ACR</span></span>

* <span data-ttu-id="d6d14-3445">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3445">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d6d14-3446">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3446">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d6d14-3447">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3447">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d6d14-3448">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3448">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d6d14-3449">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3449">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d6d14-3450">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="d6d14-3450">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3451">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3451">ACS</span></span>

* <span data-ttu-id="d6d14-3452">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="d6d14-3452">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3453">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3453">Appservice</span></span>

* <span data-ttu-id="d6d14-3454">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3454">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d6d14-3455">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="d6d14-3455">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d6d14-3456">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3456">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d6d14-3457">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3457">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d6d14-3458">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3458">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d6d14-3459">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3459">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d6d14-3460">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3460">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d6d14-3461">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3461">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d6d14-3462">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3462">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d6d14-3463">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3463">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d6d14-3464">Lote</span><span class="sxs-lookup"><span data-stu-id="d6d14-3464">Batch</span></span>

* <span data-ttu-id="d6d14-3465">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="d6d14-3465">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d6d14-3466">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3466">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d6d14-3467">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3467">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d6d14-3468">CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3468">CDN</span></span>

* <span data-ttu-id="d6d14-3469">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="d6d14-3469">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d6d14-3470">Nuvem</span><span class="sxs-lookup"><span data-stu-id="d6d14-3470">Cloud</span></span>

* <span data-ttu-id="d6d14-3471">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="d6d14-3471">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d6d14-3472">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="d6d14-3472">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d6d14-3473">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3473">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d6d14-3474">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="d6d14-3474">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d6d14-3475">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3475">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-3476">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3476">CosmosDB</span></span>

* <span data-ttu-id="d6d14-3477">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3477">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d6d14-3478">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="d6d14-3478">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d6d14-3479">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-3479">Data Lake Analytics</span></span>

* <span data-ttu-id="d6d14-3480">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3480">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d6d14-3481">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3481">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d6d14-3482">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3482">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d6d14-3483">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3483">Data Lake Store</span></span>

* <span data-ttu-id="d6d14-3484">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3484">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d6d14-3485">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="d6d14-3485">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d6d14-3486">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3486">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d6d14-3487">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3487">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d6d14-3488">Interativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3488">Interactive</span></span>

* <span data-ttu-id="d6d14-3489">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="d6d14-3489">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d6d14-3490">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="d6d14-3490">Increased test coverage</span></span>
* <span data-ttu-id="d6d14-3491">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="d6d14-3491">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d6d14-3492">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3492">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d6d14-3493">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3493">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d6d14-3494">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3494">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d6d14-3495">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3495">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d6d14-3496">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3496">Added `--progress` flag</span></span>
* <span data-ttu-id="d6d14-3497">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="d6d14-3497">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d6d14-3498">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3498">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d6d14-3499">IoT</span><span class="sxs-lookup"><span data-stu-id="d6d14-3499">IoT</span></span>

* <span data-ttu-id="d6d14-3500">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3500">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d6d14-3501">(#3934)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3501">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d6d14-3502">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="d6d14-3502">Key vault</span></span>

* <span data-ttu-id="d6d14-3503">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3503">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d6d14-3504">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3504">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d6d14-3505">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3505">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d6d14-3506">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3506">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d6d14-3507">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3507">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d6d14-3508">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3508">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d6d14-3509">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3509">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d6d14-3510">(#3307)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3510">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d6d14-3511">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3511">Lab</span></span>

* <span data-ttu-id="d6d14-3512">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3512">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d6d14-3513">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3513">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3514">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3514">Monitor</span></span>

* <span data-ttu-id="d6d14-3515">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3515">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d6d14-3516">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3516">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d6d14-3517">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3517">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d6d14-3518">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3518">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d6d14-3519">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3519">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d6d14-3520">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3520">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d6d14-3521">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="d6d14-3521">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d6d14-3522">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="d6d14-3522">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d6d14-3523">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="d6d14-3523">`location` no longer required</span></span>
  * <span data-ttu-id="d6d14-3524">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="d6d14-3524">Add name and ID support for target</span></span>
  * <span data-ttu-id="d6d14-3525">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3525">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d6d14-3526">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="d6d14-3526">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d6d14-3527">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="d6d14-3527">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d6d14-3528">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="d6d14-3528">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d6d14-3529">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3529">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d6d14-3530">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3530">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3531">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3531">Network</span></span>

* <span data-ttu-id="d6d14-3532">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3532">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d6d14-3533">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3533">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d6d14-3534">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="d6d14-3534">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d6d14-3535">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="d6d14-3535">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d6d14-3536">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3536">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d6d14-3537">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3537">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d6d14-3538">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3538">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d6d14-3539">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3539">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d6d14-3540">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3540">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d6d14-3541">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3541">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d6d14-3542">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3542">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d6d14-3543">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3543">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d6d14-3544">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3544">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d6d14-3545">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3545">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d6d14-3546">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3546">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d6d14-3547">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3547">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d6d14-3548">Adicionado o suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para --dns-servers</span><span class="sxs-lookup"><span data-stu-id="d6d14-3548">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d6d14-3549">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3549">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d6d14-3550">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3550">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d6d14-3551">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3551">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d6d14-3552">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3552">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d6d14-3553">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3553">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d6d14-3554">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3554">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d6d14-3555">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d6d14-3555">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d6d14-3556">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d6d14-3556">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d6d14-3557">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d6d14-3557">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d6d14-3558">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="d6d14-3558">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3559">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3559">Profile</span></span>

* <span data-ttu-id="d6d14-3560">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3560">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d6d14-3561">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="d6d14-3561">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d6d14-3562">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3562">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d6d14-3563">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="d6d14-3563">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d6d14-3564">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3564">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d6d14-3565">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3565">RDBMS</span></span>

* <span data-ttu-id="d6d14-3566">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3566">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d6d14-3567">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3567">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d6d14-3568">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3568">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d6d14-3569">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3569">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3570">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3570">Resource</span></span>

* <span data-ttu-id="d6d14-3571">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3571">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d6d14-3572">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3572">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d6d14-3573">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3573">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d6d14-3574">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3574">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d6d14-3575">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3575">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d6d14-3576">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3576">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d6d14-3577">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3577">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d6d14-3578">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3578">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-3579">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-3579">Role</span></span>

* <span data-ttu-id="d6d14-3580">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3580">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d6d14-3581">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3581">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d6d14-3582">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3582">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d6d14-3583">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3583">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d6d14-3584">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3584">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d6d14-3585">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-3585">Service Fabric</span></span>
* <span data-ttu-id="d6d14-3586">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3586">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d6d14-3587">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3587">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d6d14-3588">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3588">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3589">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3589">SQL</span></span>

* <span data-ttu-id="d6d14-3590">Removido o parâmetro `sql server create` `--identity` desfeito</span><span class="sxs-lookup"><span data-stu-id="d6d14-3590">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d6d14-3591">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3591">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d6d14-3592">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3592">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3593">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3593">Storage</span></span>

* <span data-ttu-id="d6d14-3594">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3594">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d6d14-3595">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="d6d14-3595">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d6d14-3596">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3596">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d6d14-3597">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3597">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d6d14-3598">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3598">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d6d14-3599">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3599">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3600">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3600">VM</span></span>

* <span data-ttu-id="d6d14-3601">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="d6d14-3601">Support configuring nsg</span></span>
* <span data-ttu-id="d6d14-3602">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3602">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d6d14-3603">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3603">Support managed service identities</span></span>
* <span data-ttu-id="d6d14-3604">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3604">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d6d14-3605">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="d6d14-3605">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d6d14-3606">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3606">May 10, 2017</span></span>

<span data-ttu-id="d6d14-3607">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d6d14-3607">Version 2.0.6</span></span>

* <span data-ttu-id="d6d14-3608">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3608">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d6d14-3609">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3609">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d6d14-3610">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3610">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d6d14-3611">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3611">Include Cognitive Services module</span></span>
* <span data-ttu-id="d6d14-3612">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d6d14-3612">Include Service Fabric module</span></span>
* <span data-ttu-id="d6d14-3613">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3613">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d6d14-3614">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3614">Add support for CDN commands</span></span>
* <span data-ttu-id="d6d14-3615">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="d6d14-3615">Remove Container module</span></span>
* <span data-ttu-id="d6d14-3616">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3616">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d6d14-3617">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3617">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d6d14-3618">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3618">Core</span></span>

* <span data-ttu-id="d6d14-3619">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="d6d14-3619">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d6d14-3620">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3620">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d6d14-3621">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3621">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d6d14-3622">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3622">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d6d14-3623">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3623">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d6d14-3624">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3624">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d6d14-3625">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3625">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d6d14-3626">núcleo: permitir que o caminho do arquivo accessTokens.json seja configurável por meio de uma variável de ambiente ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3626">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d6d14-3627">núcleo: permitir que padrões configurados sejam aplicados em argumentos opcionais ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3627">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d6d14-3628">núcleo: desempenho aprimorado</span><span class="sxs-lookup"><span data-stu-id="d6d14-3628">core: Improved performance</span></span>
* <span data-ttu-id="d6d14-3629">núcleo: certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="d6d14-3629">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d6d14-3630">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="d6d14-3630">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3631">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3631">ACS</span></span>

* <span data-ttu-id="d6d14-3632">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6d14-3632">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d6d14-3633">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="d6d14-3633">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d6d14-3634">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="d6d14-3634">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d6d14-3635">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3635">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3636">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3636">AppService</span></span>

* <span data-ttu-id="d6d14-3637">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3637">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d6d14-3638">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3638">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d6d14-3639">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3639">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d6d14-3640">Exposição de argumentos para configurar a implantação e as “pilhas em runtime” em webapp create</span><span class="sxs-lookup"><span data-stu-id="d6d14-3640">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d6d14-3641">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3641">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d6d14-3642">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3642">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d6d14-3643">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="d6d14-3643">support slot swap with preview</span></span>
* <span data-ttu-id="d6d14-3644">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3644">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d6d14-3645">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3645">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d6d14-3646">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3646">CosmosDB</span></span>

* <span data-ttu-id="d6d14-3647">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3647">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d6d14-3648">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="d6d14-3648">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d6d14-3649">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="d6d14-3649">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d6d14-3650">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="d6d14-3650">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d6d14-3651">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-3651">Data Lake Analytics</span></span>

* <span data-ttu-id="d6d14-3652">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="d6d14-3652">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d6d14-3653">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3653">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d6d14-3654">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3654">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d6d14-3655">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="d6d14-3655">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d6d14-3656">Tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-3656">Table</span></span>
  * <span data-ttu-id="d6d14-3657">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-3657">Table valued function</span></span>
  * <span data-ttu-id="d6d14-3658">Visualizar</span><span class="sxs-lookup"><span data-stu-id="d6d14-3658">View</span></span>
  * <span data-ttu-id="d6d14-3659">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3659">Table Statistics.</span></span> <span data-ttu-id="d6d14-3660">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="d6d14-3660">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d6d14-3661">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3661">Data Lake Store</span></span>

* <span data-ttu-id="d6d14-3662">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="d6d14-3662">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d6d14-3663">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3663">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d6d14-3664">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3664">missed help for access show.</span></span> <span data-ttu-id="d6d14-3665">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3665">adding it.</span></span> <span data-ttu-id="d6d14-3666">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3666">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d6d14-3667">Localizar</span><span class="sxs-lookup"><span data-stu-id="d6d14-3667">Find</span></span>

* <span data-ttu-id="d6d14-3668">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="d6d14-3668">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d6d14-3669">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d6d14-3669">KeyVault</span></span>

* <span data-ttu-id="d6d14-3670">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="d6d14-3670">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d6d14-3671">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois estes parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="d6d14-3671">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d6d14-3672">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="d6d14-3672">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d6d14-3673">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3673">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d6d14-3674">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3674">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d6d14-3675">Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3675">Lab</span></span>

* <span data-ttu-id="d6d14-3676">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3676">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d6d14-3677">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3677">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d6d14-3678">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3678">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d6d14-3679">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3679">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d6d14-3680">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="d6d14-3680">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d6d14-3681">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3681">Monitor</span></span>

* <span data-ttu-id="d6d14-3682">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3682">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d6d14-3683">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3683">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d6d14-3684">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3684">Network</span></span>

* <span data-ttu-id="d6d14-3685">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3685">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d6d14-3686">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3686">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d6d14-3687">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3687">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d6d14-3688">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3688">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d6d14-3689">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d6d14-3689">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d6d14-3690">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="d6d14-3690">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d6d14-3691">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3691">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d6d14-3692">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="d6d14-3692">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d6d14-3693">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3693">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d6d14-3694">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="d6d14-3694">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d6d14-3695">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3695">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d6d14-3696">BC: corrigido um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3696">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d6d14-3697">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3697">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d6d14-3698">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="d6d14-3698">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d6d14-3699">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="d6d14-3699">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d6d14-3700">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3700">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d6d14-3701">Perfil</span><span class="sxs-lookup"><span data-stu-id="d6d14-3701">Profile</span></span>

* <span data-ttu-id="d6d14-3702">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3702">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d6d14-3703">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3703">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d6d14-3704">Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-3704">Redis</span></span>

* <span data-ttu-id="d6d14-3705">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="d6d14-3705">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d6d14-3706">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="d6d14-3706">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d6d14-3707">Recurso</span><span class="sxs-lookup"><span data-stu-id="d6d14-3707">Resource</span></span>

* <span data-ttu-id="d6d14-3708">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3708">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d6d14-3709">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3709">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d6d14-3710">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3710">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d6d14-3711">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3711">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d6d14-3712">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3712">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d6d14-3713">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3713">Add docs for az lock update.</span></span> <span data-ttu-id="d6d14-3714">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3714">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d6d14-3715">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3715">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d6d14-3716">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3716">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d6d14-3717">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3717">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d6d14-3718">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3718">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d6d14-3719">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3719">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d6d14-3720">Função</span><span class="sxs-lookup"><span data-stu-id="d6d14-3720">Role</span></span>

* <span data-ttu-id="d6d14-3721">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3721">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d6d14-3722">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3722">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d6d14-3723">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3723">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d6d14-3724">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="d6d14-3724">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d6d14-3725">SQL</span><span class="sxs-lookup"><span data-stu-id="d6d14-3725">SQL</span></span>

* <span data-ttu-id="d6d14-3726">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="d6d14-3726">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d6d14-3727">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3727">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d6d14-3728">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3728">Storage</span></span>

* <span data-ttu-id="d6d14-3729">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3729">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d6d14-3730">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="d6d14-3730">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d6d14-3731">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="d6d14-3731">Add support for large block blob upload</span></span>
* <span data-ttu-id="d6d14-3732">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3732">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3733">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3733">VM</span></span>

* <span data-ttu-id="d6d14-3734">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="d6d14-3734">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d6d14-3735">observação: em comandos da VM em nuvens soberanas, evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3735">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d6d14-3736">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d6d14-3736">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d6d14-3737">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d6d14-3737">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d6d14-3738">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="d6d14-3738">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d6d14-3739">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="d6d14-3739">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d6d14-3740">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3740">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d6d14-3741">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3741">April 3, 2017</span></span>

<span data-ttu-id="d6d14-3742">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d6d14-3742">Version 2.0.2</span></span>

<span data-ttu-id="d6d14-3743">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3743">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d6d14-3744">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d6d14-3744">Core</span></span>

* <span data-ttu-id="d6d14-3745">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3745">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d6d14-3746">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3746">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d6d14-3747">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3747">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d6d14-3748">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3748">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d6d14-3749">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3749">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d6d14-3750">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3750">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d6d14-3751">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3751">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d6d14-3752">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="d6d14-3752">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d6d14-3753">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="d6d14-3753">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d6d14-3754">ACS</span><span class="sxs-lookup"><span data-stu-id="d6d14-3754">ACS</span></span>

* <span data-ttu-id="d6d14-3755">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3755">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d6d14-3756">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3756">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d6d14-3757">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3757">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d6d14-3758">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3758">Add support for windows clusters.</span></span> <span data-ttu-id="d6d14-3759">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3759">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d6d14-3760">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3760">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d6d14-3761">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3761">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d6d14-3762">AppService</span><span class="sxs-lookup"><span data-stu-id="d6d14-3762">AppService</span></span>

* <span data-ttu-id="d6d14-3763">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3763">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d6d14-3764">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3764">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d6d14-3765">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3765">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d6d14-3766">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3766">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d6d14-3767">DataLake</span><span class="sxs-lookup"><span data-stu-id="d6d14-3767">DataLake</span></span>

* <span data-ttu-id="d6d14-3768">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d6d14-3768">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d6d14-3769">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d6d14-3769">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d6d14-3770">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="d6d14-3770">DocuemntDB</span></span>

* <span data-ttu-id="d6d14-3771">DocumentDB: adicionado suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3771">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d6d14-3772">VM</span><span class="sxs-lookup"><span data-stu-id="d6d14-3772">VM</span></span>

* <span data-ttu-id="d6d14-3773">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3773">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d6d14-3774">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3774">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d6d14-3775">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3775">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d6d14-3776">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3776">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d6d14-3777">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3777">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d6d14-3778">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3778">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="d6d14-3779">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d6d14-3779">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d6d14-3780">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="d6d14-3780">February 27, 2017</span></span>

<span data-ttu-id="d6d14-3781">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d6d14-3781">Version 2.0.0</span></span>

<span data-ttu-id="d6d14-3782">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3782">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d6d14-3783">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3783">Container Service (acs)</span></span>
- <span data-ttu-id="d6d14-3784">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3784">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d6d14-3785">Rede</span><span class="sxs-lookup"><span data-stu-id="d6d14-3785">Networking</span></span>
- <span data-ttu-id="d6d14-3786">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d6d14-3786">Storage</span></span>

<span data-ttu-id="d6d14-3787">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3787">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d6d14-3788">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-3788">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d6d14-3789">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="d6d14-3789">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d6d14-3790">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="d6d14-3790">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d6d14-3791">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3791">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d6d14-3792">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="d6d14-3792">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d6d14-3793">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3793">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d6d14-3794">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d6d14-3794">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d6d14-3795">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d6d14-3795">Provide feedback from the command line with the `az feedback` command</span></span>

# <a name="beta-release-notes"></a>[<span data-ttu-id="d6d14-3796">Notas sobre a versão beta</span><span class="sxs-lookup"><span data-stu-id="d6d14-3796">Beta release notes</span></span>](#tab/azure-cli-beta)

<span data-ttu-id="d6d14-3797">A versão beta da CLI do Azure é uma migração do método de autenticação da plataforma AAD (v 1.0) para a [plataforma de Identidade da Microsoft (v 2.0)](/azure/active-directory/develop/v2-overview).</span><span class="sxs-lookup"><span data-stu-id="d6d14-3797">The Azure CLI beta release is a migration from the authentican method of AAD platform (v1.0) to [Microsoft Identity platform (v2.0)](/azure/active-directory/develop/v2-overview).</span></span>

## <a name="june-23-2020"></a><span data-ttu-id="d6d14-3798">23 de junho de 2020</span><span class="sxs-lookup"><span data-stu-id="d6d14-3798">June 23, 2020</span></span>

### <a name="things-to-know-about-the-new-azure-cli-beta-release"></a><span data-ttu-id="d6d14-3799">O que você precisa saber sobre a nova versão beta da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="d6d14-3799">Things to know about the new Azure CLI beta release</span></span>

-   <span data-ttu-id="d6d14-3800">A versão beta da CLI do Azure dá suporte a todos os comandos da CLI que você encontrará na versão lançada atual.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3800">The beta version of the Azure CLI supports all CLI commands that you will find in the current released version.</span></span>
-   <span data-ttu-id="d6d14-3801">Fazer logon novamente é necessário após a instalação da versão beta.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3801">Relogin is required after install the beta version.</span></span>
-   <span data-ttu-id="d6d14-3802">A versão beta dá suporte apenas à plataforma Windows.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3802">The beta release only supports the Windows platform.</span></span>
-   <span data-ttu-id="d6d14-3803">Não há suporte para o Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3803">The Azure Stack is not supported.</span></span>
-   <span data-ttu-id="d6d14-3804">Não há suporte para o parâmetro `--use-cert-sn-issuer` ao usar a chave de entidade de serviço para autenticar.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3804">`--use-cert-sn-issuer` parameter is not supported when using service principle key to authenticate.</span></span>
-   <span data-ttu-id="d6d14-3805">Não há suporte para ignorar a verificação SSL por meio do ambiente `ADAL_PYTHON_SSL_NO_VERIFY`.</span><span class="sxs-lookup"><span data-stu-id="d6d14-3805">Skip SSL verification via environment `ADAL_PYTHON_SSL_NO_VERIFY` is not supported.</span></span>

<span data-ttu-id="d6d14-3806">Se você encontrar problemas com a versão beta, a equipe de engenharia da CLI do Azure ficará feliz por receber seus comentários no [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span><span class="sxs-lookup"><span data-stu-id="d6d14-3806">If you find any issues in the beta release, the Azure CLI engineering team welcomes your comments on [GitHub](https://github.com/Azure/azure-cli/issues/new/choose).</span></span>

---