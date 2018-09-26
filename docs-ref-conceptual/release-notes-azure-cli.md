---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/21/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: f6dd04e088651527b1ac13e719b7fc3c5522b310
ms.sourcegitcommit: d93b0a2bcfb0d164ef90d6d4618f0552609a8ea6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/20/2018
ms.locfileid: "46470058"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="15cea-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="15cea-103">Azure CLI 2.0 release notes</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="15cea-104">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-104">September 21, 2018</span></span>

<span data-ttu-id="15cea-105">Versão 20.46</span><span class="sxs-lookup"><span data-stu-id="15cea-105">Version 20.46</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-106">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-106">ACR</span></span>
* <span data-ttu-id="15cea-107">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-107">Added ACR Task commands</span></span>
* <span data-ttu-id="15cea-108">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="15cea-108">Added quick run command</span></span>
* <span data-ttu-id="15cea-109">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-109">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="15cea-110">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-110">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="15cea-111">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="15cea-111">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="15cea-112">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="15cea-112">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-113">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-113">ACS</span></span>
* <span data-ttu-id="15cea-114">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-114">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="15cea-115">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="15cea-115">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-116">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-116">AppService</span></span>

* <span data-ttu-id="15cea-117">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="15cea-117">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="15cea-118">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="15cea-118">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="15cea-119">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="15cea-119">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="15cea-120">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="15cea-120">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-121">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-121">Batch</span></span>
* <span data-ttu-id="15cea-122">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="15cea-122">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="15cea-123">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="15cea-123">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="15cea-124">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="15cea-124">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="15cea-125">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="15cea-125">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15cea-126">Lote AI</span><span class="sxs-lookup"><span data-stu-id="15cea-126">Batch AI</span></span> 
* <span data-ttu-id="15cea-127">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="15cea-127">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15cea-128">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-128">Cognitive Services</span></span>
* <span data-ttu-id="15cea-129">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="15cea-129">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="15cea-130">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="15cea-130">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="15cea-131">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="15cea-131">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="15cea-132">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="15cea-132">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="15cea-133">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="15cea-133">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="15cea-134">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="15cea-134">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="15cea-135">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-135">Container</span></span>
* <span data-ttu-id="15cea-136">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="15cea-136">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="15cea-137">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="15cea-137">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="15cea-138">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="15cea-138">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="15cea-139">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="15cea-139">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="15cea-140">DataLake</span><span class="sxs-lookup"><span data-stu-id="15cea-140">Datalake</span></span>
* <span data-ttu-id="15cea-141">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="15cea-141">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="15cea-142">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-142">Interactive Shell</span></span>
* <span data-ttu-id="15cea-143">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-143">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="15cea-144">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-144">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-145">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-145">IoT</span></span>
* <span data-ttu-id="15cea-146">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-146">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="15cea-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="15cea-147">Key Vault</span></span>
* <span data-ttu-id="15cea-148">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="15cea-148">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="15cea-149">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-149">Network</span></span>
* <span data-ttu-id="15cea-150">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="15cea-150">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="15cea-151">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="15cea-151">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="15cea-152">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="15cea-152">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="15cea-153">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="15cea-153">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="15cea-154">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="15cea-154">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="15cea-155">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="15cea-155">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="15cea-156">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="15cea-156">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="15cea-157">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="15cea-157">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="15cea-158">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="15cea-158">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="15cea-159">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="15cea-159">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="15cea-160">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="15cea-160">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="15cea-161">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="15cea-161">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="15cea-162">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="15cea-162">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="15cea-163">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="15cea-163">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="15cea-164">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="15cea-164">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="15cea-165">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="15cea-165">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="15cea-166">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="15cea-166">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="15cea-167">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="15cea-167">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-168">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15cea-168">RDBMS</span></span>
* <span data-ttu-id="15cea-169">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="15cea-169">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="15cea-170">Reserva</span><span class="sxs-lookup"><span data-stu-id="15cea-170">Reservation</span></span>
* <span data-ttu-id="15cea-171">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="15cea-171">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="15cea-172">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="15cea-172">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="15cea-173">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cea-173">Manage App</span></span>
* <span data-ttu-id="15cea-174">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="15cea-174">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="15cea-175">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="15cea-175">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="15cea-176">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-176">Role</span></span>
* <span data-ttu-id="15cea-177">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="15cea-177">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="15cea-178">SignalR</span><span class="sxs-lookup"><span data-stu-id="15cea-178">SignalR</span></span>
* <span data-ttu-id="15cea-179">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="15cea-179">First release</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-180">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-180">Storage</span></span>
* <span data-ttu-id="15cea-181">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="15cea-181">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="15cea-182">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="15cea-182">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-183">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-183">VM</span></span>
* <span data-ttu-id="15cea-184">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="15cea-184">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="15cea-185">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="15cea-185">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="15cea-186">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-186">August 28, 2018</span></span>

<span data-ttu-id="15cea-187">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="15cea-187">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="15cea-188">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-188">Core</span></span>

* <span data-ttu-id="15cea-189">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="15cea-189">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="15cea-190">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="15cea-190">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-191">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-191">ACR</span></span>

* <span data-ttu-id="15cea-192">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="15cea-192">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="15cea-193">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="15cea-193">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-194">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-194">ACS</span></span>

* <span data-ttu-id="15cea-195">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="15cea-195">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="15cea-196">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="15cea-196">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-197">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-197">AppService</span></span>

* <span data-ttu-id="15cea-198">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="15cea-198">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="15cea-199">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-199">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="15cea-200">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-200">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="15cea-201">Backup</span><span class="sxs-lookup"><span data-stu-id="15cea-201">Backup</span></span>

* <span data-ttu-id="15cea-202">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-202">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="15cea-203">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="15cea-203">Bot Service</span></span>

* <span data-ttu-id="15cea-204">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-204">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15cea-205">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-205">Cognitive Services</span></span>

* <span data-ttu-id="15cea-206">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="15cea-206">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-207">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-207">IoT</span></span>

* <span data-ttu-id="15cea-208">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="15cea-208">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-209">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-209">Monitor</span></span>

* <span data-ttu-id="15cea-210">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="15cea-210">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="15cea-211">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-211">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="15cea-212">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-212">Network</span></span>

* <span data-ttu-id="15cea-213">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-213">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-214">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-214">Resource</span></span>

* <span data-ttu-id="15cea-215">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-215">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-216">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-216">Storage</span></span>

* <span data-ttu-id="15cea-217">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-217">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-218">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-218">VM</span></span>

* <span data-ttu-id="15cea-219">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-219">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="15cea-220">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-220">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="15cea-221">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-221">Auguest 14, 2018</span></span>

<span data-ttu-id="15cea-222">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="15cea-222">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="15cea-223">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-223">Core</span></span>

* <span data-ttu-id="15cea-224">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="15cea-224">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="15cea-225">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="15cea-225">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="15cea-226">Telemetria</span><span class="sxs-lookup"><span data-stu-id="15cea-226">Telemetry</span></span>

* <span data-ttu-id="15cea-227">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="15cea-227">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-228">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-228">ACR</span></span>

* <span data-ttu-id="15cea-229">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="15cea-229">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="15cea-230">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="15cea-230">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-231">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-231">ACS</span></span>

* <span data-ttu-id="15cea-232">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="15cea-232">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="15cea-233">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="15cea-233">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="15cea-234">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="15cea-234">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="15cea-235">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="15cea-235">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="15cea-236">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="15cea-236">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="15cea-237">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-237">AppService</span></span>

* <span data-ttu-id="15cea-238">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="15cea-238">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="15cea-239">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="15cea-239">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="15cea-240">BatchAI</span><span class="sxs-lookup"><span data-stu-id="15cea-240">BatchAI</span></span>

* <span data-ttu-id="15cea-241">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="15cea-241">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="15cea-242">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-242">Container</span></span>

* <span data-ttu-id="15cea-243">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-243">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="15cea-244">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-244">IoT</span></span>

* <span data-ttu-id="15cea-245">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="15cea-245">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="15cea-246">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="15cea-246">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="15cea-247">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-247">Iot Central</span></span>

* <span data-ttu-id="15cea-248">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="15cea-248">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-249">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15cea-249">KeyVault</span></span>


* <span data-ttu-id="15cea-250">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="15cea-250">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="15cea-251">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="15cea-251">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="15cea-252">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="15cea-252">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="15cea-253">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="15cea-253">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="15cea-254">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="15cea-254">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="15cea-255">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="15cea-255">Relay</span></span>

* <span data-ttu-id="15cea-256">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-256">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-257">Sql</span><span class="sxs-lookup"><span data-stu-id="15cea-257">Sql</span></span>

* <span data-ttu-id="15cea-258">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="15cea-258">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-259">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-259">Storage</span></span>

* <span data-ttu-id="15cea-260">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="15cea-260">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="15cea-261">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="15cea-261">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="15cea-262">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="15cea-262">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="15cea-263">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="15cea-263">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="15cea-264">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-264">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-265">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-265">VM</span></span>

* <span data-ttu-id="15cea-266">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="15cea-266">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="15cea-267">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-267">July 31, 2018</span></span>

<span data-ttu-id="15cea-268">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="15cea-268">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-269">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-269">ACR</span></span>

* <span data-ttu-id="15cea-270">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="15cea-270">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="15cea-271">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="15cea-271">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-272">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-272">ACS</span></span>

* <span data-ttu-id="15cea-273">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="15cea-273">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-274">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-274">Batch</span></span>

* <span data-ttu-id="15cea-275">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="15cea-275">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="15cea-276">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-276">Container</span></span>

* <span data-ttu-id="15cea-277">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-277">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="15cea-278">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-278">Network</span></span>

* <span data-ttu-id="15cea-279">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="15cea-279">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="15cea-280">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-280">Resource</span></span>

* <span data-ttu-id="15cea-281">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="15cea-281">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="15cea-282">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="15cea-282">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="15cea-283">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-283">Role</span></span>

* <span data-ttu-id="15cea-284">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="15cea-284">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="15cea-285">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-285">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="15cea-286">Search</span><span class="sxs-lookup"><span data-stu-id="15cea-286">Search</span></span>

* <span data-ttu-id="15cea-287">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="15cea-287">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="15cea-288">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="15cea-288">Service Bus</span></span>

* <span data-ttu-id="15cea-289">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="15cea-289">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="15cea-290">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-290">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="15cea-291">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="15cea-291">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="15cea-292">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="15cea-292">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-293">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-293">Storage</span></span>

* <span data-ttu-id="15cea-294">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="15cea-294">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="15cea-295">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-295">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-296">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-296">VM</span></span>

* <span data-ttu-id="15cea-297">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-297">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="15cea-298">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="15cea-298">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="15cea-299">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="15cea-299">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="15cea-300">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="15cea-300">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="15cea-301">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-301">July 18, 2018</span></span>

<span data-ttu-id="15cea-302">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="15cea-302">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="15cea-303">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-303">Core</span></span>

* <span data-ttu-id="15cea-304">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="15cea-304">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="15cea-305">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="15cea-305">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="15cea-306">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="15cea-306">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-307">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-307">ACR</span></span>

* <span data-ttu-id="15cea-308">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="15cea-308">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="15cea-309">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="15cea-309">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="15cea-310">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="15cea-310">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="15cea-311">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="15cea-311">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-312">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-312">ACS</span></span>

* <span data-ttu-id="15cea-313">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="15cea-313">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-314">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-314">AppService</span></span>

* <span data-ttu-id="15cea-315">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="15cea-315">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-316">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-316">Batch</span></span>

* <span data-ttu-id="15cea-317">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="15cea-317">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="15cea-318">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="15cea-318">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15cea-319">Lote AI</span><span class="sxs-lookup"><span data-stu-id="15cea-319">Batch AI</span></span>

* <span data-ttu-id="15cea-320">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="15cea-320">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="15cea-321">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-321">Container</span></span>

* <span data-ttu-id="15cea-322">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="15cea-322">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="15cea-323">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="15cea-323">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="15cea-324">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-324">Network</span></span>

* <span data-ttu-id="15cea-325">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="15cea-325">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="15cea-326">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="15cea-326">Added `network nic wait`</span></span>
* <span data-ttu-id="15cea-327">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="15cea-327">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="15cea-328">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="15cea-328">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="15cea-329">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-329">Resource</span></span>

* <span data-ttu-id="15cea-330">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="15cea-330">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="15cea-331">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="15cea-331">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="15cea-332">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="15cea-332">Added `deployment wait` command</span></span>
* <span data-ttu-id="15cea-333">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="15cea-333">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-334">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-334">SQL</span></span>

* <span data-ttu-id="15cea-335">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="15cea-335">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="15cea-336">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="15cea-336">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="15cea-337">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="15cea-337">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-338">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-338">Storage</span></span>

* <span data-ttu-id="15cea-339">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="15cea-339">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-340">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-340">VM</span></span>

* <span data-ttu-id="15cea-341">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-341">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="15cea-342">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="15cea-342">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="15cea-343">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="15cea-343">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="15cea-344">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-344">July 3, 2018</span></span>

<span data-ttu-id="15cea-345">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="15cea-345">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="15cea-346">AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-346">AKS</span></span>

* <span data-ttu-id="15cea-347">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-347">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="15cea-348">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-348">July 3, 2018</span></span>

<span data-ttu-id="15cea-349">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="15cea-349">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="15cea-350">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-350">Core</span></span>

* <span data-ttu-id="15cea-351">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-351">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-352">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-352">ACR</span></span>

* <span data-ttu-id="15cea-353">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="15cea-353">Added polling build status</span></span>
* <span data-ttu-id="15cea-354">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="15cea-354">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="15cea-355">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="15cea-355">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-356">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-356">ACS</span></span>

* <span data-ttu-id="15cea-357">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-357">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="15cea-358">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="15cea-358">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="15cea-359">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="15cea-359">Updated options for `aks browse` command.</span></span> <span data-ttu-id="15cea-360">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="15cea-360">Added `--listen-port` support</span></span>
* <span data-ttu-id="15cea-361">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="15cea-361">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="15cea-362">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="15cea-362">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="15cea-363">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="15cea-363">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-364">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-364">AppService</span></span>

* <span data-ttu-id="15cea-365">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="15cea-365">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="15cea-366">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="15cea-366">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="15cea-367">Backup</span><span class="sxs-lookup"><span data-stu-id="15cea-367">Backup</span></span>

* <span data-ttu-id="15cea-368">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="15cea-368">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="15cea-369">BatchAI</span><span class="sxs-lookup"><span data-stu-id="15cea-369">BatchAI</span></span>

* <span data-ttu-id="15cea-370">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="15cea-370">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="15cea-371">Nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-371">Cloud</span></span>

* <span data-ttu-id="15cea-372">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-372">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="15cea-373">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-373">Container</span></span>

* <span data-ttu-id="15cea-374">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="15cea-374">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="15cea-375">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="15cea-375">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="15cea-376">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="15cea-376">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-377">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-377">Extension</span></span>

* <span data-ttu-id="15cea-378">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="15cea-378">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="15cea-379">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-379">Network</span></span>

* <span data-ttu-id="15cea-380">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="15cea-380">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-381">Rdbms</span><span class="sxs-lookup"><span data-stu-id="15cea-381">Rdbms</span></span>

* <span data-ttu-id="15cea-382">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="15cea-382">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-383">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-383">Resource</span></span>

* <span data-ttu-id="15cea-384">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="15cea-384">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-385">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-385">VM</span></span>

* <span data-ttu-id="15cea-386">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="15cea-386">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="15cea-387">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-387">June 25, 2018</span></span>

<span data-ttu-id="15cea-388">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="15cea-388">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="15cea-389">CLI</span><span class="sxs-lookup"><span data-stu-id="15cea-389">CLI</span></span>

* <span data-ttu-id="15cea-390">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-390">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="15cea-391">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-391">June 19, 2018</span></span>

<span data-ttu-id="15cea-392">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="15cea-392">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="15cea-393">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-393">Core</span></span>

* <span data-ttu-id="15cea-394">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-394">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-395">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-395">ACR</span></span>

* <span data-ttu-id="15cea-396">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="15cea-396">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="15cea-397">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="15cea-397">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-398">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-398">ACS</span></span>

* <span data-ttu-id="15cea-399">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="15cea-399">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="15cea-400">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="15cea-400">Added `--update` support</span></span>
* <span data-ttu-id="15cea-401">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="15cea-401">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="15cea-402">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="15cea-402">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="15cea-403">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="15cea-403">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="15cea-404">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="15cea-404">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="15cea-405">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="15cea-405">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="15cea-406">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="15cea-406">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-407">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-407">AppService</span></span>

* <span data-ttu-id="15cea-408">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="15cea-408">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="15cea-409">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="15cea-409">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-410">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-410">Batch</span></span>

* <span data-ttu-id="15cea-411">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="15cea-411">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15cea-412">Lote AI</span><span class="sxs-lookup"><span data-stu-id="15cea-412">Batch AI</span></span>

* <span data-ttu-id="15cea-413">Foi adicionado suporte aos espaços de trabalho.</span><span class="sxs-lookup"><span data-stu-id="15cea-413">Added support for workspaces.</span></span> <span data-ttu-id="15cea-414">Os espaços de trabalho permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="15cea-414">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="15cea-415">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="15cea-415">Added support for experiments.</span></span> <span data-ttu-id="15cea-416">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="15cea-416">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="15cea-417">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="15cea-417">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="15cea-418">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="15cea-418">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="15cea-419">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="15cea-419">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="15cea-420">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="15cea-420">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="15cea-421">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-421">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="15cea-422">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="15cea-422">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="15cea-423">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="15cea-423">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="15cea-424">Para montar um NFS pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="15cea-424">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="15cea-425">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="15cea-425">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="15cea-426">Para enviar um trabalho em um cluster pertencente a outro espaço de trabalho/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="15cea-426">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="15cea-427">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="15cea-427">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="15cea-428">Agora, o local é um atributo de um espaço de trabalho.</span><span class="sxs-lookup"><span data-stu-id="15cea-428">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="15cea-429">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="15cea-429">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="15cea-430">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="15cea-430">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="15cea-431">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="15cea-431">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="15cea-432">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="15cea-432">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="15cea-433">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="15cea-433">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="15cea-434">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="15cea-434">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="15cea-435">Mapas</span><span class="sxs-lookup"><span data-stu-id="15cea-435">Maps</span></span>

* <span data-ttu-id="15cea-436">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="15cea-436">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="15cea-437">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-437">Network</span></span>

* <span data-ttu-id="15cea-438">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="15cea-438">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="15cea-439">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="15cea-439">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="15cea-440">#6502</span><span class="sxs-lookup"><span data-stu-id="15cea-440">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="15cea-441">Reservas</span><span class="sxs-lookup"><span data-stu-id="15cea-441">Reservations</span></span>

* <span data-ttu-id="15cea-442">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="15cea-442">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="15cea-443">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="15cea-443">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="15cea-444">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="15cea-444">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="15cea-445">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="15cea-445">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="15cea-446">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="15cea-446">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="15cea-447">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="15cea-447">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="15cea-448">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-448">Role</span></span>

* <span data-ttu-id="15cea-449">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="15cea-449">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-450">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-450">SQL</span></span>

* <span data-ttu-id="15cea-451">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-451">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-452">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-452">Storage</span></span>

* <span data-ttu-id="15cea-453">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="15cea-453">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-454">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-454">VM</span></span>

* <span data-ttu-id="15cea-455">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-455">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="15cea-456">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="15cea-456">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="15cea-457">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="15cea-457">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="15cea-458">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-458">June 13, 2018</span></span>

<span data-ttu-id="15cea-459">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="15cea-459">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="15cea-460">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-460">Core</span></span>

* <span data-ttu-id="15cea-461">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="15cea-461">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="15cea-462">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-462">June 13, 2018</span></span>

<span data-ttu-id="15cea-463">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="15cea-463">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="15cea-464">AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-464">AKS</span></span>

* <span data-ttu-id="15cea-465">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="15cea-465">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="15cea-466">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="15cea-466">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="15cea-467">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="15cea-467">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="15cea-468">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="15cea-468">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="15cea-469">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="15cea-469">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-470">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-470">AppService</span></span>

* <span data-ttu-id="15cea-471">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="15cea-471">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="15cea-472">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-472">June 5, 2018</span></span>

<span data-ttu-id="15cea-473">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="15cea-473">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-474">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-474">Interactive</span></span>

* <span data-ttu-id="15cea-475">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-475">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="15cea-476">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-476">June 5, 2018</span></span>

<span data-ttu-id="15cea-477">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="15cea-477">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="15cea-478">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-478">Core</span></span>

* <span data-ttu-id="15cea-479">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="15cea-479">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="15cea-480">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="15cea-480">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-481">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-481">ACR</span></span>

* <span data-ttu-id="15cea-482">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="15cea-482">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="15cea-483">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="15cea-483">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="15cea-484">AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-484">AKS</span></span>

* <span data-ttu-id="15cea-485">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="15cea-485">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-486">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-486">Batch</span></span>

* <span data-ttu-id="15cea-487">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="15cea-487">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-488">IOT</span><span class="sxs-lookup"><span data-stu-id="15cea-488">IOT</span></span>

* <span data-ttu-id="15cea-489">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="15cea-489">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="15cea-490">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-490">Network</span></span>

* <span data-ttu-id="15cea-491">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="15cea-491">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="15cea-492">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="15cea-492">Policy Insights</span></span>

* <span data-ttu-id="15cea-493">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-493">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="15cea-494">ARM</span><span class="sxs-lookup"><span data-stu-id="15cea-494">ARM</span></span>

* <span data-ttu-id="15cea-495">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="15cea-495">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-496">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-496">SQL</span></span>

* <span data-ttu-id="15cea-497">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="15cea-497">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="15cea-498">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="15cea-498">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="15cea-499">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-499">Storage</span></span>

* <span data-ttu-id="15cea-500">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="15cea-500">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-501">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-501">VM</span></span>

* <span data-ttu-id="15cea-502">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="15cea-502">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="15cea-503">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-503">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="15cea-504">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="15cea-504">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="15cea-505">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-505">May 22, 2018</span></span>

<span data-ttu-id="15cea-506">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="15cea-506">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="15cea-507">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-507">Core</span></span>

* <span data-ttu-id="15cea-508">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="15cea-508">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-509">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-509">ACS</span></span>

* <span data-ttu-id="15cea-510">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-510">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="15cea-511">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="15cea-511">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-512">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-512">AppService</span></span>

* <span data-ttu-id="15cea-513">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="15cea-513">Improved generic update commands</span></span>
* <span data-ttu-id="15cea-514">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="15cea-514">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="15cea-515">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-515">Container</span></span>

* <span data-ttu-id="15cea-516">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="15cea-516">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="15cea-517">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-517">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-518">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-518">Extension</span></span>

* <span data-ttu-id="15cea-519">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="15cea-519">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-520">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-520">Interactive</span></span>

* <span data-ttu-id="15cea-521">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="15cea-521">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="15cea-522">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="15cea-522">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-523">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15cea-523">KeyVault</span></span>

* <span data-ttu-id="15cea-524">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="15cea-524">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="15cea-525">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-525">Network</span></span>

* <span data-ttu-id="15cea-526">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="15cea-526">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="15cea-527">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="15cea-527">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-528">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-528">SQL</span></span>

* <span data-ttu-id="15cea-529">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="15cea-529">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="15cea-530">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="15cea-530">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="15cea-531">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="15cea-531">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="15cea-532">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cea-532">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="15cea-533">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="15cea-533">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="15cea-534">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="15cea-534">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="15cea-535">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="15cea-535">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="15cea-536">`edition`.</span><span class="sxs-lookup"><span data-stu-id="15cea-536">`edition`.</span></span> <span data-ttu-id="15cea-537">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="15cea-537">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="15cea-538">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="15cea-538">`elasticPoolName`.</span></span> <span data-ttu-id="15cea-539">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="15cea-539">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="15cea-540">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="15cea-540">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="15cea-541">`edition`.</span><span class="sxs-lookup"><span data-stu-id="15cea-541">`edition`.</span></span> <span data-ttu-id="15cea-542">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="15cea-542">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="15cea-543">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="15cea-543">`dtu`.</span></span> <span data-ttu-id="15cea-544">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="15cea-544">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="15cea-545">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="15cea-545">`databaseDtuMin`.</span></span> <span data-ttu-id="15cea-546">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="15cea-546">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="15cea-547">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="15cea-547">`databaseDtuMax`.</span></span> <span data-ttu-id="15cea-548">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="15cea-548">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="15cea-549">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="15cea-549">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="15cea-550">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="15cea-550">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-551">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-551">Storage</span></span>

* <span data-ttu-id="15cea-552">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="15cea-552">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="15cea-553">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="15cea-553">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-554">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-554">VM</span></span>

* <span data-ttu-id="15cea-555">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="15cea-555">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="15cea-556">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="15cea-556">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="15cea-557">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="15cea-557">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="15cea-558">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="15cea-558">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="15cea-559">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="15cea-559">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="15cea-560">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-560">May 7, 2018</span></span>

<span data-ttu-id="15cea-561">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="15cea-561">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="15cea-562">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-562">Core</span></span>

* <span data-ttu-id="15cea-563">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="15cea-563">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="15cea-564">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="15cea-564">Added limited support for positional arguments</span></span>
* <span data-ttu-id="15cea-565">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="15cea-565">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="15cea-566">#5591</span><span class="sxs-lookup"><span data-stu-id="15cea-566">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="15cea-567">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="15cea-567">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="15cea-568">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="15cea-568">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="15cea-569">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-569">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="15cea-570">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="15cea-570">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="15cea-571">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="15cea-571">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-572">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-572">ACR</span></span>

* <span data-ttu-id="15cea-573">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-573">Added ACR Build commands</span></span>
* <span data-ttu-id="15cea-574">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="15cea-574">Improved resource not found error messages</span></span>
* <span data-ttu-id="15cea-575">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="15cea-575">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="15cea-576">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="15cea-576">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="15cea-577">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="15cea-577">Improved repository commands error messages</span></span>
* <span data-ttu-id="15cea-578">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="15cea-578">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-579">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-579">ACS</span></span>

* <span data-ttu-id="15cea-580">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="15cea-580">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="15cea-581">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="15cea-581">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="15cea-582">MAS</span><span class="sxs-lookup"><span data-stu-id="15cea-582">AMS</span></span>

* <span data-ttu-id="15cea-583">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="15cea-583">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-584">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-584">Appservice</span></span>

* <span data-ttu-id="15cea-585">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="15cea-585">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="15cea-586">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="15cea-586">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="15cea-587">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="15cea-587">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="15cea-588">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="15cea-588">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="15cea-589">Lote AI</span><span class="sxs-lookup"><span data-stu-id="15cea-589">Batch AI</span></span>

* <span data-ttu-id="15cea-590">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="15cea-590">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15cea-591">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-591">Cognitive Services</span></span>

* <span data-ttu-id="15cea-592">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="15cea-592">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="15cea-593">Consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-593">Consumption</span></span>

* <span data-ttu-id="15cea-594">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="15cea-594">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="15cea-595">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-595">Container</span></span>

* <span data-ttu-id="15cea-596">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="15cea-596">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="15cea-597">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15cea-597">Cosmos DB</span></span>

* <span data-ttu-id="15cea-598">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="15cea-598">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="15cea-599">DMS</span><span class="sxs-lookup"><span data-stu-id="15cea-599">DMS</span></span>

* <span data-ttu-id="15cea-600">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="15cea-600">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-601">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-601">Extension</span></span>

* <span data-ttu-id="15cea-602">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="15cea-602">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-603">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-603">Interactive</span></span>

* <span data-ttu-id="15cea-604">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="15cea-604">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="15cea-605">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="15cea-605">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="15cea-606">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="15cea-606">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="15cea-607">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="15cea-607">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="15cea-608">Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-608">Lab</span></span>

* <span data-ttu-id="15cea-609">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="15cea-609">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="15cea-610">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-610">Network</span></span>

* <span data-ttu-id="15cea-611">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="15cea-611">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="15cea-612">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-612">Profile</span></span>

* <span data-ttu-id="15cea-613">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="15cea-613">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="15cea-614">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="15cea-614">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="15cea-615">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="15cea-615">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="15cea-616">Redis</span><span class="sxs-lookup"><span data-stu-id="15cea-616">Redis</span></span>

* <span data-ttu-id="15cea-617">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="15cea-617">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="15cea-618">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="15cea-618">Deprecated `redis list-all`.</span></span> <span data-ttu-id="15cea-619">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="15cea-619">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="15cea-620">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="15cea-620">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="15cea-621">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-621">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="15cea-622">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-622">Role</span></span>

* <span data-ttu-id="15cea-623">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="15cea-623">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-624">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-624">Storage</span></span>

* <span data-ttu-id="15cea-625">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="15cea-625">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="15cea-626">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="15cea-626">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="15cea-627">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="15cea-627">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="15cea-628">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="15cea-628">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="15cea-629">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="15cea-629">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-630">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-630">VM</span></span>

* <span data-ttu-id="15cea-631">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="15cea-631">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="15cea-632">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="15cea-632">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="15cea-633">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="15cea-633">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="15cea-634">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="15cea-634">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="15cea-635">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="15cea-635">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="15cea-636">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="15cea-636">Added write accelerator support</span></span>
* <span data-ttu-id="15cea-637">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="15cea-637">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="15cea-638">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="15cea-638">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="15cea-639">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="15cea-639">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="15cea-640">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-640">April 10, 2018</span></span>

<span data-ttu-id="15cea-641">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="15cea-641">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-642">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-642">ACR</span></span>

* <span data-ttu-id="15cea-643">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="15cea-643">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-644">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-644">ACS</span></span>

* <span data-ttu-id="15cea-645">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="15cea-645">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-646">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-646">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="15cea-648">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="15cea-648">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="15cea-649">BatchAI</span><span class="sxs-lookup"><span data-stu-id="15cea-649">BatchAI</span></span>

* <span data-ttu-id="15cea-650">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="15cea-650">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="15cea-651">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-651">Job level mounting</span></span>
 - <span data-ttu-id="15cea-652">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="15cea-652">Environment variables with secret values</span></span>
 - <span data-ttu-id="15cea-653">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="15cea-653">Performance counters settings</span></span>
 - <span data-ttu-id="15cea-654">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-654">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="15cea-655">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="15cea-655">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="15cea-656">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="15cea-656">Usage and limits reporting</span></span>
 - <span data-ttu-id="15cea-657">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="15cea-657">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="15cea-658">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="15cea-658">Support for custom images</span></span>
 - <span data-ttu-id="15cea-659">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="15cea-659">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="15cea-660">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-660">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="15cea-661">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="15cea-661">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="15cea-662">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="15cea-662">National clouds are supported</span></span>
* <span data-ttu-id="15cea-663">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="15cea-663">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="15cea-664">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="15cea-664">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="15cea-665">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-665">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="15cea-666">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="15cea-666">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="15cea-667">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="15cea-667">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="15cea-668">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="15cea-668">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="15cea-669">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="15cea-669">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="15cea-670">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="15cea-670">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="15cea-671">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="15cea-671">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="15cea-672">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="15cea-672">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="15cea-673">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="15cea-673">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="15cea-674">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="15cea-674">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="15cea-675">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="15cea-675">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="15cea-676">Cobrança</span><span class="sxs-lookup"><span data-stu-id="15cea-676">Billing</span></span>

* <span data-ttu-id="15cea-677">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="15cea-677">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="15cea-678">Consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-678">Consumption</span></span>

* <span data-ttu-id="15cea-679">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="15cea-679">Added `marketplace` commands</span></span>
* <span data-ttu-id="15cea-680">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="15cea-680">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="15cea-681">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="15cea-681">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="15cea-682">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="15cea-682">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="15cea-683">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="15cea-683">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="15cea-684">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="15cea-684">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="15cea-685">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-685">Container</span></span>

* <span data-ttu-id="15cea-686">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="15cea-686">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="15cea-687">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="15cea-687">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-688">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-688">Extension</span></span>

* <span data-ttu-id="15cea-689">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="15cea-689">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-690">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-690">Interactive</span></span>

* <span data-ttu-id="15cea-691">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="15cea-691">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="15cea-692">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="15cea-692">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="15cea-693">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="15cea-693">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="15cea-694">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-694">Network</span></span>

* <span data-ttu-id="15cea-695">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="15cea-695">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="15cea-696">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="15cea-696">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="15cea-697">#4910</span><span class="sxs-lookup"><span data-stu-id="15cea-697">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="15cea-698">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="15cea-698">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="15cea-699">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="15cea-699">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="15cea-700">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-700">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="15cea-701">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-701">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="15cea-702">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="15cea-702">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-703">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-703">Profile</span></span>

* <span data-ttu-id="15cea-704">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="15cea-704">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="15cea-705">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="15cea-705">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-706">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15cea-706">RDBMS</span></span>

* <span data-ttu-id="15cea-707">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="15cea-707">Added `georestore` command</span></span>
* <span data-ttu-id="15cea-708">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="15cea-708">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-709">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-709">Resource</span></span>

* <span data-ttu-id="15cea-710">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="15cea-710">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="15cea-711">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="15cea-711">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-712">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-712">SQL</span></span>

* <span data-ttu-id="15cea-713">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="15cea-713">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-714">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-714">Storage</span></span>

* <span data-ttu-id="15cea-715">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="15cea-715">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-716">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-716">VM</span></span>

* <span data-ttu-id="15cea-717">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="15cea-717">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="15cea-718">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="15cea-718">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="15cea-720">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-720">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="15cea-721">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="15cea-721">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="15cea-722">#5718</span><span class="sxs-lookup"><span data-stu-id="15cea-722">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="15cea-723">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="15cea-723">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="15cea-724">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-724">March 27, 2018</span></span>

<span data-ttu-id="15cea-725">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="15cea-725">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="15cea-726">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-726">Core</span></span>

* <span data-ttu-id="15cea-727">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="15cea-727">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-728">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-728">ACS</span></span>

* <span data-ttu-id="15cea-729">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="15cea-729">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-730">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-730">Appservice</span></span>

* <span data-ttu-id="15cea-731">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="15cea-731">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="15cea-732">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="15cea-732">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15cea-733">Backup</span><span class="sxs-lookup"><span data-stu-id="15cea-733">Backup</span></span>

* <span data-ttu-id="15cea-734">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="15cea-734">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="15cea-735">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-735">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="15cea-736">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="15cea-736">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="15cea-737">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="15cea-737">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="15cea-738">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-738">Container</span></span>

* <span data-ttu-id="15cea-739">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="15cea-739">Added `container exec` command.</span></span> <span data-ttu-id="15cea-740">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="15cea-740">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="15cea-741">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-741">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-742">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-742">Extension</span></span>

* <span data-ttu-id="15cea-743">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="15cea-743">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="15cea-744">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="15cea-744">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="15cea-745">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-745">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-746">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-746">Interactive</span></span>

* <span data-ttu-id="15cea-747">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-747">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="15cea-748">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="15cea-748">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="15cea-749">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-749">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="15cea-750">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="15cea-750">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="15cea-751">Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-751">Lab</span></span>

* <span data-ttu-id="15cea-752">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="15cea-752">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-753">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-753">Monitor</span></span>

* <span data-ttu-id="15cea-754">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="15cea-754">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="15cea-755">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="15cea-755">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="15cea-756">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="15cea-756">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="15cea-757">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-757">Network</span></span>

* <span data-ttu-id="15cea-758">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="15cea-758">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-759">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-759">Profile</span></span>

* <span data-ttu-id="15cea-760">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="15cea-760">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-761">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15cea-761">RDBMS</span></span>

* <span data-ttu-id="15cea-762">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="15cea-762">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-763">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-763">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="15cea-765">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-765">Role</span></span>

* <span data-ttu-id="15cea-766">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="15cea-766">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="15cea-767">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="15cea-767">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="15cea-768">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="15cea-768">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="15cea-769">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="15cea-769">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="15cea-770">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="15cea-770">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-771">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-771">Storage</span></span>

* <span data-ttu-id="15cea-772">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="15cea-772">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="15cea-773">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="15cea-773">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-774">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-774">VM</span></span>

* <span data-ttu-id="15cea-775">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="15cea-775">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="15cea-776">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="15cea-776">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="15cea-777">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="15cea-777">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="15cea-778">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="15cea-778">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="15cea-779">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-779">March 13, 2018</span></span>

<span data-ttu-id="15cea-780">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="15cea-780">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-781">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-781">ACR</span></span>

* <span data-ttu-id="15cea-782">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="15cea-782">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="15cea-783">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="15cea-783">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="15cea-784">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="15cea-784">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-785">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-785">ACS</span></span>

* <span data-ttu-id="15cea-786">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="15cea-786">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="15cea-787">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="15cea-787">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="15cea-788">Supervisor</span><span class="sxs-lookup"><span data-stu-id="15cea-788">Advisor</span></span>

* <span data-ttu-id="15cea-789">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="15cea-789">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="15cea-790">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="15cea-790">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="15cea-791">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="15cea-791">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="15cea-792">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="15cea-792">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="15cea-793">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="15cea-793">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-794">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-794">Appservice</span></span>

* <span data-ttu-id="15cea-795">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="15cea-795">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="15cea-796">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-796">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="15cea-797">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="15cea-797">Eventhubs</span></span>

* <span data-ttu-id="15cea-798">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-798">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-799">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-799">Extension</span></span>

* <span data-ttu-id="15cea-800">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="15cea-800">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-801">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-801">Interactive</span></span>

* <span data-ttu-id="15cea-802">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="15cea-802">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="15cea-803">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="15cea-803">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="15cea-804">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="15cea-804">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="15cea-805">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="15cea-805">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-806">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-806">Monitor</span></span>

* <span data-ttu-id="15cea-807">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-807">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="15cea-808">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="15cea-808">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="15cea-809">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="15cea-809">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="15cea-810">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="15cea-810">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="15cea-811">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-811">Network</span></span>

* <span data-ttu-id="15cea-812">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="15cea-812">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="15cea-813">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="15cea-813">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="15cea-814">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-814">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="15cea-815">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="15cea-815">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-816">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-816">Profile</span></span>

* <span data-ttu-id="15cea-817">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="15cea-817">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="15cea-818">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="15cea-818">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-819">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15cea-819">RDBMS</span></span>

* <span data-ttu-id="15cea-820">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="15cea-820">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="15cea-821">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="15cea-821">Service Bus</span></span>

* <span data-ttu-id="15cea-822">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-822">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-823">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-823">Storage</span></span>

* <span data-ttu-id="15cea-824">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="15cea-824">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="15cea-825">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="15cea-825">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-826">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-826">VM</span></span>

* <span data-ttu-id="15cea-827">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="15cea-827">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="15cea-828">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-828">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="15cea-829">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="15cea-829">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="15cea-830">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="15cea-830">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="15cea-831">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-831">February 27, 2018</span></span>

<span data-ttu-id="15cea-832">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="15cea-832">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="15cea-833">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-833">Core</span></span>

* <span data-ttu-id="15cea-834">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="15cea-834">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="15cea-835">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="15cea-835">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="15cea-836">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="15cea-836">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-837">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-837">ACS</span></span>

* <span data-ttu-id="15cea-838">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-838">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="15cea-839">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="15cea-839">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="15cea-840">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="15cea-840">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="15cea-841">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="15cea-841">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-842">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-842">Appservice</span></span>

* <span data-ttu-id="15cea-843">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="15cea-843">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="15cea-844">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="15cea-844">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="15cea-845">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-845">Cognitive Services</span></span>

* <span data-ttu-id="15cea-846">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-846">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="15cea-847">Consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-847">Consumption</span></span>

* <span data-ttu-id="15cea-848">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="15cea-848">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="15cea-849">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="15cea-849">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="15cea-850">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-850">Container</span></span>

* <span data-ttu-id="15cea-851">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="15cea-851">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="15cea-852">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-852">Network</span></span>

* <span data-ttu-id="15cea-853">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="15cea-853">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-854">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-854">Resource</span></span>

* <span data-ttu-id="15cea-855">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="15cea-855">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="15cea-856">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-856">Role</span></span>

* <span data-ttu-id="15cea-857">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="15cea-857">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-858">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-858">SQL</span></span>

* <span data-ttu-id="15cea-859">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="15cea-859">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-860">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-860">Storage</span></span>

* <span data-ttu-id="15cea-861">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="15cea-861">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-862">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-862">VM</span></span>

* <span data-ttu-id="15cea-863">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="15cea-863">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="15cea-864">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-864">February 13, 2018</span></span>

<span data-ttu-id="15cea-865">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="15cea-865">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="15cea-866">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-866">Core</span></span>

* <span data-ttu-id="15cea-867">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="15cea-867">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-868">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-868">ACS</span></span>

* <span data-ttu-id="15cea-869">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="15cea-869">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="15cea-870">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="15cea-870">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="15cea-871">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="15cea-871">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="15cea-872">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-872">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="15cea-873">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="15cea-873">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="15cea-874">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="15cea-874">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="15cea-875">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="15cea-875">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="15cea-876">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="15cea-876">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-877">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-877">Appservice</span></span>

* <span data-ttu-id="15cea-878">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="15cea-878">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="15cea-879">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="15cea-879">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="15cea-880">CDN</span><span class="sxs-lookup"><span data-stu-id="15cea-880">CDN</span></span>

* <span data-ttu-id="15cea-881">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="15cea-881">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="15cea-882">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-882">Container</span></span>

* <span data-ttu-id="15cea-883">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="15cea-883">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="15cea-884">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-884">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15cea-885">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-885">CosmosDB</span></span>

* <span data-ttu-id="15cea-886">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="15cea-886">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-887">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-887">Extension</span></span>

* <span data-ttu-id="15cea-888">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-888">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="15cea-889">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-889">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="15cea-890">Comentários</span><span class="sxs-lookup"><span data-stu-id="15cea-890">Feedback</span></span>

* <span data-ttu-id="15cea-891">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="15cea-891">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-892">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-892">Interactive</span></span>

* <span data-ttu-id="15cea-893">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="15cea-893">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="15cea-894">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="15cea-894">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-895">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-895">IoT</span></span>

* <span data-ttu-id="15cea-896">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="15cea-896">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15cea-897">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="15cea-897">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="15cea-898">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-898">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="15cea-899">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="15cea-899">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-900">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-900">Monitor</span></span>

* <span data-ttu-id="15cea-901">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="15cea-901">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="15cea-902">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-902">Network</span></span>

* <span data-ttu-id="15cea-903">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="15cea-903">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="15cea-904">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-904">Profile</span></span>

* <span data-ttu-id="15cea-905">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-905">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-906">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-906">Resource</span></span>

* <span data-ttu-id="15cea-907">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="15cea-907">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="15cea-908">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-908">Role</span></span>

* <span data-ttu-id="15cea-909">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="15cea-909">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-910">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-910">SQL</span></span>

* <span data-ttu-id="15cea-911">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="15cea-911">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="15cea-912">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="15cea-912">Added `sql db rename`</span></span>
* <span data-ttu-id="15cea-913">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="15cea-913">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-914">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-914">Storage</span></span>

* <span data-ttu-id="15cea-915">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="15cea-915">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-916">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-916">VM</span></span>

* <span data-ttu-id="15cea-917">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="15cea-917">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="15cea-918">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="15cea-918">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="15cea-919">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="15cea-919">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="15cea-920">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-920">January 31, 2018</span></span>

<span data-ttu-id="15cea-921">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="15cea-921">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="15cea-922">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-922">Core</span></span>

* <span data-ttu-id="15cea-923">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="15cea-923">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="15cea-924">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="15cea-924">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="15cea-925">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="15cea-925">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="15cea-926">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="15cea-926">Use `--verbose` to see</span></span>
* <span data-ttu-id="15cea-927">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="15cea-927">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-928">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-928">ACS</span></span>

* <span data-ttu-id="15cea-929">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="15cea-929">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="15cea-930">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="15cea-930">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-931">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-931">Appservice</span></span>

* <span data-ttu-id="15cea-932">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="15cea-932">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="15cea-933">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="15cea-933">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="15cea-934">CDN</span><span class="sxs-lookup"><span data-stu-id="15cea-934">CDN</span></span>

* <span data-ttu-id="15cea-935">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="15cea-935">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15cea-936">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-936">CosmosDB</span></span>

* <span data-ttu-id="15cea-937">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="15cea-937">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-938">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-938">Interactive</span></span>

* <span data-ttu-id="15cea-939">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="15cea-939">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="15cea-940">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-940">Network</span></span>

* <span data-ttu-id="15cea-941">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="15cea-941">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="15cea-942">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="15cea-942">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="15cea-943">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="15cea-943">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="15cea-944">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="15cea-944">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="15cea-945">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="15cea-945">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="15cea-946">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="15cea-946">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="15cea-947">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-947">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="15cea-948">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="15cea-948">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="15cea-949">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="15cea-949">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="15cea-950">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="15cea-950">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-951">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-951">Profile</span></span>

* <span data-ttu-id="15cea-952">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="15cea-952">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-953">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-953">Resource</span></span>

* <span data-ttu-id="15cea-954">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="15cea-954">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-955">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-955">Storage</span></span>

* <span data-ttu-id="15cea-956">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="15cea-956">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="15cea-957">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="15cea-957">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="15cea-958">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="15cea-958">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="15cea-959">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="15cea-959">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="15cea-960">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="15cea-960">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-961">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-961">VM</span></span>

* <span data-ttu-id="15cea-962">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="15cea-962">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="15cea-963">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="15cea-963">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="15cea-964">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="15cea-964">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="15cea-965">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-965">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="15cea-966">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="15cea-966">January 17, 2018</span></span>

<span data-ttu-id="15cea-967">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="15cea-967">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-968">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-968">ACR</span></span>

* <span data-ttu-id="15cea-969">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="15cea-969">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="15cea-970">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="15cea-970">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-971">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-971">ACS</span></span>

* <span data-ttu-id="15cea-972">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="15cea-972">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="15cea-973">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="15cea-973">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-974">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-974">Appservice</span></span>

* <span data-ttu-id="15cea-975">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="15cea-975">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="15cea-976">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="15cea-976">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="15cea-977">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="15cea-977">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="15cea-978">Backup</span><span class="sxs-lookup"><span data-stu-id="15cea-978">Backup</span></span>

* <span data-ttu-id="15cea-979">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="15cea-979">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="15cea-980">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="15cea-980">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="15cea-981">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="15cea-981">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="15cea-982">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="15cea-982">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="15cea-983">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-983">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-984">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-984">Batch</span></span>

* <span data-ttu-id="15cea-985">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="15cea-985">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="15cea-986">Nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-986">Cloud</span></span>

* <span data-ttu-id="15cea-987">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-987">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="15cea-988">Consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-988">Consumption</span></span>

* <span data-ttu-id="15cea-989">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="15cea-989">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="15cea-990">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="15cea-990">Event Grid</span></span>

* <span data-ttu-id="15cea-991">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="15cea-991">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15cea-992">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="15cea-992">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="15cea-993">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="15cea-993">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="15cea-994">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="15cea-994">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="15cea-995">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="15cea-995">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="15cea-996">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="15cea-996">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="15cea-997">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="15cea-997">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="15cea-998">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="15cea-998">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-999">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-999">Interactive</span></span>

* <span data-ttu-id="15cea-1000">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="15cea-1000">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="15cea-1001">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="15cea-1001">Fixed errors on startup</span></span>
* <span data-ttu-id="15cea-1002">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1002">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-1003">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-1003">IoT</span></span>

* <span data-ttu-id="15cea-1004">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="15cea-1004">Added support for device provisioning service</span></span>
* <span data-ttu-id="15cea-1005">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="15cea-1005">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="15cea-1006">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-1006">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1007">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1007">Monitor</span></span>

* <span data-ttu-id="15cea-1008">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="15cea-1008">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="15cea-1009">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1009">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="15cea-1010">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="15cea-1010">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1011">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1011">Network</span></span>

* <span data-ttu-id="15cea-1012">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1012">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="15cea-1013">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1013">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-1014">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-1014">Profile</span></span>

* <span data-ttu-id="15cea-1015">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="15cea-1015">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="15cea-1016">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-1016">Role</span></span>

* <span data-ttu-id="15cea-1017">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="15cea-1017">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15cea-1018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15cea-1018">Service Fabric</span></span>

* <span data-ttu-id="15cea-1019">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="15cea-1019">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="15cea-1020">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="15cea-1020">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1021">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1021">VM</span></span>

* <span data-ttu-id="15cea-1022">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="15cea-1022">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="15cea-1023">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="15cea-1023">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="15cea-1024">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="15cea-1024">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="15cea-1025">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="15cea-1025">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="15cea-1026">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="15cea-1026">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="15cea-1027">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1027">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="15cea-1028">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1028">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="15cea-1029">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="15cea-1029">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="15cea-1030">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1030">December 19, 2017</span></span>

<span data-ttu-id="15cea-1031">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="15cea-1031">Version 2.0.23</span></span>

* <span data-ttu-id="15cea-1032">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="15cea-1032">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="15cea-1033">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1033">Container</span></span>

* <span data-ttu-id="15cea-1034">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1034">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1035">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1035">Network</span></span>

* <span data-ttu-id="15cea-1036">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1036">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="15cea-1037">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1037">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1038">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1038">Storage</span></span>

* <span data-ttu-id="15cea-1039">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="15cea-1039">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1040">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1040">VM</span></span>

* <span data-ttu-id="15cea-1041">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="15cea-1041">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="15cea-1042">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1042">December 5, 2017</span></span>

<span data-ttu-id="15cea-1043">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="15cea-1043">Version 2.0.22</span></span>

* <span data-ttu-id="15cea-1044">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="15cea-1044">Removed `az component` commands.</span></span> <span data-ttu-id="15cea-1045">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="15cea-1045">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="15cea-1046">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1046">Core</span></span>
* <span data-ttu-id="15cea-1047">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="15cea-1047">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="15cea-1048">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="15cea-1048">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1049">ACS</span></span>

* <span data-ttu-id="15cea-1050">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-1050">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="15cea-1051">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1051">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="15cea-1052">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="15cea-1052">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="15cea-1053">Supervisor</span><span class="sxs-lookup"><span data-stu-id="15cea-1053">Advisor</span></span>

* <span data-ttu-id="15cea-1054">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-1054">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1055">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1055">Appservice</span></span>

* <span data-ttu-id="15cea-1056">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="15cea-1056">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="15cea-1057">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="15cea-1057">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="15cea-1058">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="15cea-1058">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="15cea-1059">Consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-1059">Consumption</span></span>

* <span data-ttu-id="15cea-1060">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1060">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="15cea-1061">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1061">Container</span></span>

* <span data-ttu-id="15cea-1062">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-1062">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1063">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1063">Monitor</span></span>

* <span data-ttu-id="15cea-1064">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="15cea-1064">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1065">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1065">Resource</span></span>

* <span data-ttu-id="15cea-1066">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1066">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="15cea-1067">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-1067">Role</span></span>

* <span data-ttu-id="15cea-1068">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="15cea-1068">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="15cea-1069">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="15cea-1069">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="15cea-1070">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="15cea-1070">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1071">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1071">SQL</span></span>

* <span data-ttu-id="15cea-1072">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-1072">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="15cea-1073">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-1073">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1074">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1074">VM</span></span>

* <span data-ttu-id="15cea-1075">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="15cea-1075">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="15cea-1076">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1076">November 14, 2017</span></span>

<span data-ttu-id="15cea-1077">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="15cea-1077">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1078">ACR</span></span>

* <span data-ttu-id="15cea-1079">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="15cea-1079">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="15cea-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1080">ACS</span></span>

* <span data-ttu-id="15cea-1081">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="15cea-1081">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="15cea-1082">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1082">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="15cea-1083">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="15cea-1083">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="15cea-1084">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="15cea-1084">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="15cea-1085">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="15cea-1085">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1086">Appservice</span></span>

* <span data-ttu-id="15cea-1087">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="15cea-1087">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="15cea-1088">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="15cea-1088">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="15cea-1089">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="15cea-1089">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="15cea-1090">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="15cea-1090">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="15cea-1091">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="15cea-1091">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="15cea-1092">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="15cea-1092">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-1093">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1093">Batch</span></span>

* <span data-ttu-id="15cea-1094">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="15cea-1094">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="15cea-1095">Batchai</span><span class="sxs-lookup"><span data-stu-id="15cea-1095">Batchai</span></span>

* <span data-ttu-id="15cea-1096">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1096">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="15cea-1097">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1097">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="15cea-1098">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="15cea-1098">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="15cea-1099">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1099">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="15cea-1100">Nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-1100">Cloud</span></span>

* <span data-ttu-id="15cea-1101">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="15cea-1101">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="15cea-1102">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1102">Container</span></span>

* <span data-ttu-id="15cea-1103">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="15cea-1103">Added support to open multiple ports</span></span>
* <span data-ttu-id="15cea-1104">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="15cea-1104">Added container group restart policy</span></span>
* <span data-ttu-id="15cea-1105">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="15cea-1105">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="15cea-1106">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="15cea-1106">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15cea-1107">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15cea-1107">Data Lake Analytics</span></span>

* <span data-ttu-id="15cea-1108">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="15cea-1108">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15cea-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1109">Data Lake Store</span></span>

* <span data-ttu-id="15cea-1110">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="15cea-1110">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-1111">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-1111">Extension</span></span>

* <span data-ttu-id="15cea-1112">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="15cea-1112">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="15cea-1113">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="15cea-1113">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-1114">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-1114">IoT</span></span>

* <span data-ttu-id="15cea-1115">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="15cea-1115">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1116">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1116">Monitor</span></span>

* <span data-ttu-id="15cea-1117">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="15cea-1117">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1118">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1118">Network</span></span>

* <span data-ttu-id="15cea-1119">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="15cea-1119">Added support for CAA DNS records</span></span>
* <span data-ttu-id="15cea-1120">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1120">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="15cea-1121">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="15cea-1121">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="15cea-1122">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="15cea-1122">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="15cea-1123">Reservas</span><span class="sxs-lookup"><span data-stu-id="15cea-1123">Reservations</span></span>

* <span data-ttu-id="15cea-1124">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-1124">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1125">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1125">Resource</span></span>

* <span data-ttu-id="15cea-1126">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1126">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1127">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1127">SQL</span></span>

* <span data-ttu-id="15cea-1128">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1128">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1129">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1129">Storage</span></span>

* <span data-ttu-id="15cea-1130">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-1130">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="15cea-1131">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="15cea-1131">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="15cea-1132">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="15cea-1132">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="15cea-1133">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="15cea-1133">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="15cea-1134">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1134">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="15cea-1135">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="15cea-1135">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="15cea-1136">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1136">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1137">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1137">VM</span></span>

* <span data-ttu-id="15cea-1138">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="15cea-1138">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="15cea-1139">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="15cea-1139">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="15cea-1140">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-1140">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="15cea-1141">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="15cea-1141">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="15cea-1142">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="15cea-1142">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="15cea-1143">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1143">October 24, 2017</span></span>

<span data-ttu-id="15cea-1144">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="15cea-1144">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="15cea-1145">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1145">Core</span></span>

* <span data-ttu-id="15cea-1146">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="15cea-1146">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-1147">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1147">ACR</span></span>

* <span data-ttu-id="15cea-1148">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="15cea-1148">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="15cea-1149">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="15cea-1149">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="15cea-1150">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="15cea-1150">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1151">ACS</span></span>

* <span data-ttu-id="15cea-1152">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="15cea-1152">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="15cea-1153">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="15cea-1153">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1154">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1154">Appservice</span></span>

* <span data-ttu-id="15cea-1155">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="15cea-1155">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="15cea-1156">Componente</span><span class="sxs-lookup"><span data-stu-id="15cea-1156">Component</span></span>

* <span data-ttu-id="15cea-1157">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="15cea-1157">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1158">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1158">Monitor</span></span>

* <span data-ttu-id="15cea-1159">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="15cea-1159">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1160">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1160">Resource</span></span>

* <span data-ttu-id="15cea-1161">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="15cea-1161">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="15cea-1162">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="15cea-1162">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1163">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1163">VM</span></span>

* <span data-ttu-id="15cea-1164">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1164">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="15cea-1165">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1165">October 9, 2017</span></span>

<span data-ttu-id="15cea-1166">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="15cea-1166">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="15cea-1167">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1167">Core</span></span>

* <span data-ttu-id="15cea-1168">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="15cea-1168">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1169">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1169">Appservice</span></span>

* <span data-ttu-id="15cea-1170">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1170">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-1171">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1171">Batch</span></span>

* <span data-ttu-id="15cea-1172">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="15cea-1172">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="15cea-1173">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="15cea-1173">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="15cea-1174">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1174">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="15cea-1175">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="15cea-1175">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="15cea-1176">Batchai</span><span class="sxs-lookup"><span data-stu-id="15cea-1176">Batchai</span></span>

* <span data-ttu-id="15cea-1177">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1177">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-1178">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15cea-1178">Keyvault</span></span>

* <span data-ttu-id="15cea-1179">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="15cea-1179">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="15cea-1180">(#4448)</span><span class="sxs-lookup"><span data-stu-id="15cea-1180">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="15cea-1181">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1181">Network</span></span>

* <span data-ttu-id="15cea-1182">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="15cea-1182">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="15cea-1183">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="15cea-1183">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1184">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1184">Resource</span></span>

* <span data-ttu-id="15cea-1185">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="15cea-1185">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="15cea-1186">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-1186">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="15cea-1187">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="15cea-1187">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="15cea-1188">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1188">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1189">Sql</span><span class="sxs-lookup"><span data-stu-id="15cea-1189">Sql</span></span>

* <span data-ttu-id="15cea-1190">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="15cea-1190">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="15cea-1191">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="15cea-1191">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="15cea-1192">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="15cea-1192">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1193">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1193">Storage</span></span>

* <span data-ttu-id="15cea-1194">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="15cea-1194">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1195">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1195">Vm</span></span>

* <span data-ttu-id="15cea-1196">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="15cea-1196">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="15cea-1197">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1197">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="15cea-1198">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="15cea-1198">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="15cea-1199">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1199">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="15cea-1200">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1200">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="15cea-1201">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1201">September 22, 2017</span></span>

<span data-ttu-id="15cea-1202">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="15cea-1202">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1203">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1203">Resource</span></span>

* <span data-ttu-id="15cea-1204">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="15cea-1204">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="15cea-1205">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="15cea-1205">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="15cea-1206">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1206">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="15cea-1207">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="15cea-1207">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1208">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1208">Network</span></span>

* <span data-ttu-id="15cea-1209">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="15cea-1209">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="15cea-1210">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="15cea-1210">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="15cea-1211">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1211">Added `asg` application security group commands</span></span>
* <span data-ttu-id="15cea-1212">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1212">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="15cea-1213">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1213">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15cea-1214">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1214">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="15cea-1215">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1215">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1216">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1216">Storage</span></span>

* <span data-ttu-id="15cea-1217">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="15cea-1217">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="15cea-1218">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="15cea-1218">Eventgrid</span></span>

* <span data-ttu-id="15cea-1219">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="15cea-1219">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1220">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1220">SQL</span></span>

* <span data-ttu-id="15cea-1221">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="15cea-1221">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="15cea-1222">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="15cea-1222">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="15cea-1223">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1223">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-1224">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15cea-1224">Keyvault</span></span>

* <span data-ttu-id="15cea-1225">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="15cea-1225">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1226">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1226">VM</span></span>

* <span data-ttu-id="15cea-1227">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1227">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="15cea-1228">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="15cea-1228">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="15cea-1229">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1229">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="15cea-1230">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="15cea-1230">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="15cea-1231">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="15cea-1231">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="15cea-1232">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="15cea-1232">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1233">ACS</span></span>

* <span data-ttu-id="15cea-1234">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1234">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1235">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1235">Appservice</span></span>

* <span data-ttu-id="15cea-1236">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1236">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="15cea-1237">Backup</span><span class="sxs-lookup"><span data-stu-id="15cea-1237">Backup</span></span>

* <span data-ttu-id="15cea-1238">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="15cea-1238">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="15cea-1239">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1239">September 11, 2017</span></span>

<span data-ttu-id="15cea-1240">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="15cea-1240">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="15cea-1241">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1241">Core</span></span>

* <span data-ttu-id="15cea-1242">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="15cea-1242">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="15cea-1243">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="15cea-1243">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1244">Acs</span><span class="sxs-lookup"><span data-stu-id="15cea-1244">Acs</span></span>

* <span data-ttu-id="15cea-1245">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="15cea-1245">Added `acs list-locations` command</span></span>
* <span data-ttu-id="15cea-1246">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="15cea-1246">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1247">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1247">Appservice</span></span>

* <span data-ttu-id="15cea-1248">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1248">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="15cea-1249">CDN</span><span class="sxs-lookup"><span data-stu-id="15cea-1249">CDN</span></span>

* <span data-ttu-id="15cea-1250">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1250">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="15cea-1251">Extensão</span><span class="sxs-lookup"><span data-stu-id="15cea-1251">Extension</span></span>

* <span data-ttu-id="15cea-1252">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-1252">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-1253">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15cea-1253">Keyvault</span></span>

* <span data-ttu-id="15cea-1254">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="15cea-1254">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1255">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1255">Network</span></span>

* <span data-ttu-id="15cea-1256">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="15cea-1256">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15cea-1257">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1257">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="15cea-1258">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1258">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="15cea-1259">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1259">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15cea-1260">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1260">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1261">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1261">Resource</span></span>

* <span data-ttu-id="15cea-1262">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1262">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="15cea-1263">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1263">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="15cea-1264">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="15cea-1264">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="15cea-1265">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="15cea-1265">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1266">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1266">SQL</span></span>

* <span data-ttu-id="15cea-1267">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="15cea-1267">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1268">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1268">VM</span></span>

* <span data-ttu-id="15cea-1269">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="15cea-1269">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="15cea-1270">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="15cea-1270">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="15cea-1271">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1271">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="15cea-1272">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="15cea-1272">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="15cea-1273">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="15cea-1273">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="15cea-1274">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1274">August 31, 2017</span></span>

<span data-ttu-id="15cea-1275">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="15cea-1275">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-1276">Keyvault</span><span class="sxs-lookup"><span data-stu-id="15cea-1276">Keyvault</span></span>

* <span data-ttu-id="15cea-1277">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="15cea-1277">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="15cea-1278">Sf</span><span class="sxs-lookup"><span data-stu-id="15cea-1278">Sf</span></span>

* <span data-ttu-id="15cea-1279">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="15cea-1279">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1280">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1280">Storage</span></span>

* <span data-ttu-id="15cea-1281">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="15cea-1281">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="15cea-1282">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="15cea-1282">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="15cea-1283">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1283">August 28, 2017</span></span>

<span data-ttu-id="15cea-1284">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="15cea-1284">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="15cea-1285">CLI</span><span class="sxs-lookup"><span data-stu-id="15cea-1285">CLI</span></span>

* <span data-ttu-id="15cea-1286">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="15cea-1286">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1287">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1287">ACS</span></span>

* <span data-ttu-id="15cea-1288">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="15cea-1288">Corrected preview regions</span></span>
* <span data-ttu-id="15cea-1289">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="15cea-1289">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="15cea-1290">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="15cea-1290">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1291">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1291">Appservice</span></span>

* <span data-ttu-id="15cea-1292">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1292">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="15cea-1293">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="15cea-1293">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="15cea-1294">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1294">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="15cea-1295">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1295">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="15cea-1296">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-1296">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-1297">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-1297">IoT</span></span>

* <span data-ttu-id="15cea-1298">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="15cea-1298">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1299">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1299">Network</span></span>

* <span data-ttu-id="15cea-1300">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="15cea-1300">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="15cea-1301">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1301">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="15cea-1302">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="15cea-1302">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="15cea-1303">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1303">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="15cea-1304">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1304">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-1305">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-1305">Profile</span></span>

* <span data-ttu-id="15cea-1306">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="15cea-1306">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15cea-1307">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15cea-1307">Service Fabric</span></span>

* <span data-ttu-id="15cea-1308">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="15cea-1308">Preview release</span></span>
* <span data-ttu-id="15cea-1309">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="15cea-1309">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="15cea-1310">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="15cea-1310">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="15cea-1311">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="15cea-1311">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1312">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1312">Storage</span></span>

* <span data-ttu-id="15cea-1313">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="15cea-1313">Enabled setting blob tier</span></span>
* <span data-ttu-id="15cea-1314">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="15cea-1314">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="15cea-1315">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="15cea-1315">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="15cea-1316">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="15cea-1316">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="15cea-1317">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1317">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="15cea-1318">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="15cea-1318">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1319">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1319">VM</span></span>

* <span data-ttu-id="15cea-1320">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="15cea-1320">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="15cea-1321">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="15cea-1321">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="15cea-1322">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1322">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="15cea-1323">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="15cea-1323">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="15cea-1324">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="15cea-1324">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="15cea-1325">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1325">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="15cea-1326">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1326">August 15, 2017</span></span>

<span data-ttu-id="15cea-1327">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="15cea-1327">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1328">ACS</span></span>

* <span data-ttu-id="15cea-1329">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="15cea-1329">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1330">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1330">Appservice</span></span>

* <span data-ttu-id="15cea-1331">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="15cea-1331">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="15cea-1332">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="15cea-1332">Event Grid</span></span>

* <span data-ttu-id="15cea-1333">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="15cea-1333">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="15cea-1334">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1334">August 11, 2017</span></span>

<span data-ttu-id="15cea-1335">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="15cea-1335">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1336">ACS</span></span>

* <span data-ttu-id="15cea-1337">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="15cea-1337">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-1338">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1338">Batch</span></span>

* <span data-ttu-id="15cea-1339">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="15cea-1339">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="15cea-1340">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-1340">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="15cea-1341">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1341">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="15cea-1342">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="15cea-1342">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="15cea-1343">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="15cea-1343">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="15cea-1344">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="15cea-1344">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="15cea-1345">Componente</span><span class="sxs-lookup"><span data-stu-id="15cea-1345">Component</span></span>

* <span data-ttu-id="15cea-1346">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="15cea-1346">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="15cea-1347">Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1347">Container</span></span>

* <span data-ttu-id="15cea-1348">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="15cea-1348">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="15cea-1349">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1349">Data Lake Store</span></span>

* <span data-ttu-id="15cea-1350">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1350">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="15cea-1351">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="15cea-1351">Event Grid</span></span>

* <span data-ttu-id="15cea-1352">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="15cea-1352">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1353">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1353">Network</span></span>

* <span data-ttu-id="15cea-1354">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="15cea-1354">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="15cea-1355">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="15cea-1355">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="15cea-1356">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="15cea-1356">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="15cea-1357">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="15cea-1357">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-1358">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-1358">Profile</span></span>

* <span data-ttu-id="15cea-1359">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="15cea-1359">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1360">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1360">Storage</span></span>

* <span data-ttu-id="15cea-1361">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="15cea-1361">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1362">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1362">VM</span></span>

* <span data-ttu-id="15cea-1363">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="15cea-1363">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="15cea-1364">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="15cea-1364">Exposed `list-skus` command</span></span>
* <span data-ttu-id="15cea-1365">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="15cea-1365">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="15cea-1366">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="15cea-1366">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="15cea-1367">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="15cea-1367">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="15cea-1368">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1368">July 28, 2017</span></span>

<span data-ttu-id="15cea-1369">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="15cea-1369">Version 2.0.12</span></span>

* <span data-ttu-id="15cea-1370">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1370">Added container commands</span></span>
* <span data-ttu-id="15cea-1371">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="15cea-1371">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="15cea-1372">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1372">Core</span></span>

* <span data-ttu-id="15cea-1373">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="15cea-1373">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="15cea-1374">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="15cea-1374">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="15cea-1375">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="15cea-1375">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="15cea-1376">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="15cea-1376">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="15cea-1377">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="15cea-1377">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="15cea-1378">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="15cea-1378">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="15cea-1379">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="15cea-1379">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15cea-1380">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="15cea-1380">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="15cea-1381">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="15cea-1381">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="15cea-1382">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="15cea-1382">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="15cea-1383">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="15cea-1383">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="15cea-1384">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="15cea-1384">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="15cea-1385">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="15cea-1385">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="15cea-1386">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="15cea-1386">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="15cea-1387">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="15cea-1387">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="15cea-1388">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="15cea-1388">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="15cea-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1389">ACR</span></span>

* <span data-ttu-id="15cea-1390">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="15cea-1390">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="15cea-1391">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="15cea-1391">Support SKU update for managed registries</span></span>
* <span data-ttu-id="15cea-1392">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="15cea-1392">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="15cea-1393">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1393">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="15cea-1394">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1394">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="15cea-1395">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="15cea-1395">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1396">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1396">ACS</span></span>

* <span data-ttu-id="15cea-1397">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="15cea-1397">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1398">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1398">Appservice</span></span>

* <span data-ttu-id="15cea-1399">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="15cea-1399">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="15cea-1400">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="15cea-1400">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="15cea-1401">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="15cea-1401">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="15cea-1402">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="15cea-1402">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="15cea-1403">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="15cea-1403">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="15cea-1404">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="15cea-1404">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="15cea-1405">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="15cea-1405">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="15cea-1406">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="15cea-1406">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="15cea-1407">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="15cea-1407">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="15cea-1408">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="15cea-1408">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="15cea-1409">Lote</span><span class="sxs-lookup"><span data-stu-id="15cea-1409">Batch</span></span>

* <span data-ttu-id="15cea-1410">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="15cea-1410">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="15cea-1411">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="15cea-1411">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="15cea-1412">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="15cea-1412">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="15cea-1413">CDN</span><span class="sxs-lookup"><span data-stu-id="15cea-1413">CDN</span></span>

* <span data-ttu-id="15cea-1414">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="15cea-1414">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="15cea-1415">Nuvem</span><span class="sxs-lookup"><span data-stu-id="15cea-1415">Cloud</span></span>

* <span data-ttu-id="15cea-1416">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="15cea-1416">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="15cea-1417">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="15cea-1417">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="15cea-1418">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="15cea-1418">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="15cea-1419">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="15cea-1419">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="15cea-1420">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="15cea-1420">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15cea-1421">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-1421">CosmosDB</span></span>

* <span data-ttu-id="15cea-1422">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="15cea-1422">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="15cea-1423">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="15cea-1423">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15cea-1424">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15cea-1424">Data Lake Analytics</span></span>

* <span data-ttu-id="15cea-1425">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="15cea-1425">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="15cea-1426">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1426">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="15cea-1427">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="15cea-1427">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15cea-1428">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1428">Data Lake Store</span></span>

* <span data-ttu-id="15cea-1429">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1429">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="15cea-1430">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="15cea-1430">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="15cea-1431">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="15cea-1431">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="15cea-1432">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1432">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="15cea-1433">Interativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1433">Interactive</span></span>

* <span data-ttu-id="15cea-1434">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="15cea-1434">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="15cea-1435">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="15cea-1435">Increased test coverage</span></span>
* <span data-ttu-id="15cea-1436">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="15cea-1436">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="15cea-1437">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="15cea-1437">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="15cea-1438">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="15cea-1438">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="15cea-1439">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="15cea-1439">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="15cea-1440">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="15cea-1440">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="15cea-1441">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="15cea-1441">Added `--progress` flag</span></span>
* <span data-ttu-id="15cea-1442">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="15cea-1442">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="15cea-1443">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="15cea-1443">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="15cea-1444">IoT</span><span class="sxs-lookup"><span data-stu-id="15cea-1444">IoT</span></span>

* <span data-ttu-id="15cea-1445">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="15cea-1445">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="15cea-1446">(#3934)</span><span class="sxs-lookup"><span data-stu-id="15cea-1446">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="15cea-1447">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="15cea-1447">Key vault</span></span>

* <span data-ttu-id="15cea-1448">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="15cea-1448">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="15cea-1449">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="15cea-1449">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="15cea-1450">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="15cea-1450">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15cea-1451">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="15cea-1451">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="15cea-1452">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="15cea-1452">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="15cea-1453">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="15cea-1453">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="15cea-1454">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="15cea-1454">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="15cea-1455">(#3307)</span><span class="sxs-lookup"><span data-stu-id="15cea-1455">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="15cea-1456">Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1456">Lab</span></span>

* <span data-ttu-id="15cea-1457">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="15cea-1457">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="15cea-1458">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1458">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1459">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1459">Monitor</span></span>

* <span data-ttu-id="15cea-1460">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="15cea-1460">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="15cea-1461">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="15cea-1461">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="15cea-1462">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="15cea-1462">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="15cea-1463">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="15cea-1463">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="15cea-1464">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="15cea-1464">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="15cea-1465">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="15cea-1465">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="15cea-1466">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="15cea-1466">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="15cea-1467">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="15cea-1467">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="15cea-1468">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="15cea-1468">`location` no longer required</span></span>
  * <span data-ttu-id="15cea-1469">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="15cea-1469">Add name and ID support for target</span></span>
  * <span data-ttu-id="15cea-1470">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="15cea-1470">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="15cea-1471">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="15cea-1471">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="15cea-1472">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="15cea-1472">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="15cea-1473">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="15cea-1473">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="15cea-1474">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="15cea-1474">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="15cea-1475">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1475">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1476">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1476">Network</span></span>

* <span data-ttu-id="15cea-1477">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="15cea-1477">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="15cea-1478">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1478">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="15cea-1479">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="15cea-1479">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="15cea-1480">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="15cea-1480">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="15cea-1481">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1481">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="15cea-1482">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15cea-1482">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="15cea-1483">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1483">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="15cea-1484">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="15cea-1484">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="15cea-1485">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="15cea-1485">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="15cea-1486">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="15cea-1486">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="15cea-1487">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1487">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="15cea-1488">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="15cea-1488">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="15cea-1489">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="15cea-1489">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="15cea-1490">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1490">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="15cea-1491">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1491">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="15cea-1492">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1492">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="15cea-1493">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="15cea-1493">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="15cea-1494">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="15cea-1494">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="15cea-1495">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1495">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="15cea-1496">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1496">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="15cea-1497">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1497">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="15cea-1498">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="15cea-1498">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="15cea-1499">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="15cea-1499">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="15cea-1500">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="15cea-1500">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="15cea-1501">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="15cea-1501">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="15cea-1502">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="15cea-1502">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="15cea-1503">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="15cea-1503">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-1504">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-1504">Profile</span></span>

* <span data-ttu-id="15cea-1505">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="15cea-1505">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="15cea-1506">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="15cea-1506">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="15cea-1507">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="15cea-1507">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="15cea-1508">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="15cea-1508">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="15cea-1509">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="15cea-1509">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="15cea-1510">RDBMS</span><span class="sxs-lookup"><span data-stu-id="15cea-1510">RDBMS</span></span>

* <span data-ttu-id="15cea-1511">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="15cea-1511">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="15cea-1512">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="15cea-1512">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="15cea-1513">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="15cea-1513">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="15cea-1514">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="15cea-1514">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1515">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1515">Resource</span></span>

* <span data-ttu-id="15cea-1516">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1516">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="15cea-1517">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="15cea-1517">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="15cea-1518">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="15cea-1518">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="15cea-1519">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="15cea-1519">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="15cea-1520">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="15cea-1520">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="15cea-1521">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="15cea-1521">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="15cea-1522">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="15cea-1522">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="15cea-1523">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="15cea-1523">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="15cea-1524">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-1524">Role</span></span>

* <span data-ttu-id="15cea-1525">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="15cea-1525">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="15cea-1526">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="15cea-1526">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="15cea-1527">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="15cea-1527">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="15cea-1528">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="15cea-1528">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="15cea-1529">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="15cea-1529">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="15cea-1530">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15cea-1530">Service Fabric</span></span>
* <span data-ttu-id="15cea-1531">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="15cea-1531">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="15cea-1532">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="15cea-1532">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="15cea-1533">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="15cea-1533">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1534">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1534">SQL</span></span>

* <span data-ttu-id="15cea-1535">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="15cea-1535">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="15cea-1536">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="15cea-1536">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="15cea-1537">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="15cea-1537">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1538">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1538">Storage</span></span>

* <span data-ttu-id="15cea-1539">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="15cea-1539">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="15cea-1540">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="15cea-1540">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="15cea-1541">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="15cea-1541">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="15cea-1542">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="15cea-1542">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="15cea-1543">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="15cea-1543">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="15cea-1544">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="15cea-1544">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1545">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1545">VM</span></span>

* <span data-ttu-id="15cea-1546">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="15cea-1546">Support configuring nsg</span></span>
* <span data-ttu-id="15cea-1547">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-1547">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="15cea-1548">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="15cea-1548">Support managed service identities</span></span>
* <span data-ttu-id="15cea-1549">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="15cea-1549">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="15cea-1550">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="15cea-1550">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="15cea-1551">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1551">May 10, 2017</span></span>

<span data-ttu-id="15cea-1552">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="15cea-1552">Version 2.0.6</span></span>

* <span data-ttu-id="15cea-1553">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-1553">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="15cea-1554">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="15cea-1554">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="15cea-1555">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1555">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="15cea-1556">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="15cea-1556">Include Cognitive Services module</span></span>
* <span data-ttu-id="15cea-1557">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="15cea-1557">Include Service Fabric module</span></span>
* <span data-ttu-id="15cea-1558">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="15cea-1558">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="15cea-1559">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="15cea-1559">Add support for CDN commands</span></span>
* <span data-ttu-id="15cea-1560">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="15cea-1560">Remove Container module</span></span>
* <span data-ttu-id="15cea-1561">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="15cea-1561">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="15cea-1562">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15cea-1562">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="15cea-1563">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1563">Core</span></span>

* <span data-ttu-id="15cea-1564">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="15cea-1564">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="15cea-1565">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="15cea-1565">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="15cea-1566">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="15cea-1566">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="15cea-1567">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="15cea-1567">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="15cea-1568">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="15cea-1568">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="15cea-1569">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="15cea-1569">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="15cea-1570">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="15cea-1570">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="15cea-1571">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="15cea-1571">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="15cea-1572">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="15cea-1572">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="15cea-1573">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="15cea-1573">core: Improved performance</span></span>
* <span data-ttu-id="15cea-1574">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="15cea-1574">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="15cea-1575">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="15cea-1575">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1576">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1576">ACS</span></span>

* <span data-ttu-id="15cea-1577">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cea-1577">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="15cea-1578">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="15cea-1578">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="15cea-1579">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="15cea-1579">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="15cea-1580">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="15cea-1580">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1581">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1581">AppService</span></span>

* <span data-ttu-id="15cea-1582">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="15cea-1582">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="15cea-1583">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="15cea-1583">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="15cea-1584">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="15cea-1584">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="15cea-1585">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="15cea-1585">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="15cea-1586">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="15cea-1586">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="15cea-1587">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="15cea-1587">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="15cea-1588">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="15cea-1588">support slot swap with preview</span></span>
* <span data-ttu-id="15cea-1589">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="15cea-1589">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="15cea-1590">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="15cea-1590">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="15cea-1591">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-1591">CosmosDB</span></span>

* <span data-ttu-id="15cea-1592">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="15cea-1592">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="15cea-1593">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="15cea-1593">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="15cea-1594">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="15cea-1594">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="15cea-1595">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="15cea-1595">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="15cea-1596">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15cea-1596">Data Lake Analytics</span></span>

* <span data-ttu-id="15cea-1597">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="15cea-1597">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="15cea-1598">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="15cea-1598">Add support for new catalog item type: package.</span></span> <span data-ttu-id="15cea-1599">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="15cea-1599">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="15cea-1600">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="15cea-1600">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="15cea-1601">Tabela</span><span class="sxs-lookup"><span data-stu-id="15cea-1601">Table</span></span>
  * <span data-ttu-id="15cea-1602">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="15cea-1602">Table valued function</span></span>
  * <span data-ttu-id="15cea-1603">Visualizar</span><span class="sxs-lookup"><span data-stu-id="15cea-1603">View</span></span>
  * <span data-ttu-id="15cea-1604">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="15cea-1604">Table Statistics.</span></span> <span data-ttu-id="15cea-1605">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="15cea-1605">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="15cea-1606">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1606">Data Lake Store</span></span>

* <span data-ttu-id="15cea-1607">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="15cea-1607">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="15cea-1608">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="15cea-1608">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="15cea-1609">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="15cea-1609">missed help for access show.</span></span> <span data-ttu-id="15cea-1610">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="15cea-1610">adding it.</span></span> <span data-ttu-id="15cea-1611">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="15cea-1611">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="15cea-1612">Localizar</span><span class="sxs-lookup"><span data-stu-id="15cea-1612">Find</span></span>

* <span data-ttu-id="15cea-1613">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="15cea-1613">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="15cea-1614">KeyVault</span><span class="sxs-lookup"><span data-stu-id="15cea-1614">KeyVault</span></span>

* <span data-ttu-id="15cea-1615">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="15cea-1615">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="15cea-1616">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="15cea-1616">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="15cea-1617">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="15cea-1617">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="15cea-1618">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="15cea-1618">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="15cea-1619">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="15cea-1619">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="15cea-1620">Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1620">Lab</span></span>

* <span data-ttu-id="15cea-1621">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1621">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="15cea-1622">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1622">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="15cea-1623">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1623">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="15cea-1624">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1624">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="15cea-1625">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="15cea-1625">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="15cea-1626">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="15cea-1626">Monitor</span></span>

* <span data-ttu-id="15cea-1627">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="15cea-1627">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="15cea-1628">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="15cea-1628">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="15cea-1629">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1629">Network</span></span>

* <span data-ttu-id="15cea-1630">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="15cea-1630">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="15cea-1631">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1631">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="15cea-1632">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1632">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="15cea-1633">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="15cea-1633">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="15cea-1634">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="15cea-1634">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="15cea-1635">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="15cea-1635">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="15cea-1636">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="15cea-1636">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="15cea-1637">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="15cea-1637">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="15cea-1638">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="15cea-1638">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="15cea-1639">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="15cea-1639">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="15cea-1640">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="15cea-1640">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="15cea-1641">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1641">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="15cea-1642">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-1642">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="15cea-1643">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="15cea-1643">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="15cea-1644">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="15cea-1644">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="15cea-1645">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="15cea-1645">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="15cea-1646">Perfil</span><span class="sxs-lookup"><span data-stu-id="15cea-1646">Profile</span></span>

* <span data-ttu-id="15cea-1647">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="15cea-1647">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="15cea-1648">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="15cea-1648">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="15cea-1649">Redis</span><span class="sxs-lookup"><span data-stu-id="15cea-1649">Redis</span></span>

* <span data-ttu-id="15cea-1650">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="15cea-1650">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="15cea-1651">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="15cea-1651">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="15cea-1652">Recurso</span><span class="sxs-lookup"><span data-stu-id="15cea-1652">Resource</span></span>

* <span data-ttu-id="15cea-1653">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="15cea-1653">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="15cea-1654">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="15cea-1654">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="15cea-1655">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="15cea-1655">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="15cea-1656">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="15cea-1656">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="15cea-1657">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="15cea-1657">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="15cea-1658">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="15cea-1658">Add docs for az lock update.</span></span> <span data-ttu-id="15cea-1659">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="15cea-1659">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="15cea-1660">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="15cea-1660">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="15cea-1661">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="15cea-1661">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="15cea-1662">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="15cea-1662">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="15cea-1663">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="15cea-1663">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="15cea-1664">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="15cea-1664">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="15cea-1665">Função</span><span class="sxs-lookup"><span data-stu-id="15cea-1665">Role</span></span>

* <span data-ttu-id="15cea-1666">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="15cea-1666">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="15cea-1667">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="15cea-1667">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="15cea-1668">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="15cea-1668">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="15cea-1669">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="15cea-1669">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="15cea-1670">SQL</span><span class="sxs-lookup"><span data-stu-id="15cea-1670">SQL</span></span>

* <span data-ttu-id="15cea-1671">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="15cea-1671">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="15cea-1672">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="15cea-1672">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="15cea-1673">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1673">Storage</span></span>

* <span data-ttu-id="15cea-1674">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="15cea-1674">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="15cea-1675">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="15cea-1675">Add support for incremental blob copy</span></span>
* <span data-ttu-id="15cea-1676">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="15cea-1676">Add support for large block blob upload</span></span>
* <span data-ttu-id="15cea-1677">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="15cea-1677">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1678">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1678">VM</span></span>

* <span data-ttu-id="15cea-1679">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="15cea-1679">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="15cea-1680">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="15cea-1680">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="15cea-1681">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="15cea-1681">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="15cea-1682">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="15cea-1682">az vm/vmss disk</span></span>
  3. <span data-ttu-id="15cea-1683">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="15cea-1683">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="15cea-1684">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="15cea-1684">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="15cea-1685">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="15cea-1685">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="15cea-1686">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1686">April 3, 2017</span></span>

<span data-ttu-id="15cea-1687">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="15cea-1687">Version 2.0.2</span></span>

<span data-ttu-id="15cea-1688">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="15cea-1688">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="15cea-1689">Núcleo</span><span class="sxs-lookup"><span data-stu-id="15cea-1689">Core</span></span>

* <span data-ttu-id="15cea-1690">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-1690">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="15cea-1691">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="15cea-1691">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="15cea-1692">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="15cea-1692">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="15cea-1693">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15cea-1693">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15cea-1694">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="15cea-1694">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="15cea-1695">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="15cea-1695">Add prompting for missing template parameters.</span></span> <span data-ttu-id="15cea-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="15cea-1696">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="15cea-1697">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="15cea-1697">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="15cea-1698">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="15cea-1698">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="15cea-1699">ACS</span><span class="sxs-lookup"><span data-stu-id="15cea-1699">ACS</span></span>

* <span data-ttu-id="15cea-1700">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="15cea-1700">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="15cea-1701">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="15cea-1701">Add support for ssh key password prompting.</span></span> <span data-ttu-id="15cea-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="15cea-1702">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="15cea-1703">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="15cea-1703">Add support for windows clusters.</span></span> <span data-ttu-id="15cea-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="15cea-1704">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="15cea-1705">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="15cea-1705">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="15cea-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="15cea-1706">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="15cea-1707">AppService</span><span class="sxs-lookup"><span data-stu-id="15cea-1707">AppService</span></span>

* <span data-ttu-id="15cea-1708">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="15cea-1708">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="15cea-1709">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="15cea-1709">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="15cea-1710">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="15cea-1710">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="15cea-1711">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="15cea-1711">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="15cea-1712">DataLake</span><span class="sxs-lookup"><span data-stu-id="15cea-1712">DataLake</span></span>

* <span data-ttu-id="15cea-1713">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="15cea-1713">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="15cea-1714">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="15cea-1714">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="15cea-1715">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="15cea-1715">DocuemntDB</span></span>

* <span data-ttu-id="15cea-1716">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="15cea-1716">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="15cea-1717">VM</span><span class="sxs-lookup"><span data-stu-id="15cea-1717">VM</span></span>

* <span data-ttu-id="15cea-1718">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="15cea-1718">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="15cea-1719">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="15cea-1719">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="15cea-1720">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="15cea-1720">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="15cea-1721">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="15cea-1721">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="15cea-1722">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="15cea-1722">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="15cea-1723">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="15cea-1723">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="15cea-1724">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="15cea-1724">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="15cea-1725">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="15cea-1725">February 27, 2017</span></span>

<span data-ttu-id="15cea-1726">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="15cea-1726">Version 2.0.0</span></span>

<span data-ttu-id="15cea-1727">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="15cea-1727">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="15cea-1728">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="15cea-1728">Container Service (acs)</span></span>
- <span data-ttu-id="15cea-1729">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="15cea-1729">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="15cea-1730">Rede</span><span class="sxs-lookup"><span data-stu-id="15cea-1730">Networking</span></span>
- <span data-ttu-id="15cea-1731">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="15cea-1731">Storage</span></span>

<span data-ttu-id="15cea-1732">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="15cea-1732">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="15cea-1733">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="15cea-1733">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="15cea-1734">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="15cea-1734">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="15cea-1735">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="15cea-1735">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="15cea-1736">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="15cea-1736">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="15cea-1737">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="15cea-1737">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="15cea-1738">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="15cea-1738">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="15cea-1739">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="15cea-1739">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="15cea-1740">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="15cea-1740">Provide feedback from the command line with the `az feedback` command</span></span>

