---
title: Notas de versão da CLI do Azure
description: Saiba mais sobre as últimas atualizações da CLI do Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/09/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0aec9dce0eda007c71df3693b39c7ec8cc9856cd
ms.sourcegitcommit: 0fc354c24454f5c9c5ff4b7296ad7b18ffdf31b1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2018
ms.locfileid: "48904779"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="8eafc-103">Notas de versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="8eafc-103">Azure CLI release notes</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="8eafc-104">9 de outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-104">October 9, 2018</span></span>

<span data-ttu-id="8eafc-105">Versão 2.0.47</span><span class="sxs-lookup"><span data-stu-id="8eafc-105">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-106">Core</span></span>
* <span data-ttu-id="8eafc-107">Melhoria do tratamento de erro para os erros de "Solicitação Incorreta"</span><span class="sxs-lookup"><span data-stu-id="8eafc-107">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-108">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-108">ACR</span></span>
* <span data-ttu-id="8eafc-109">Suporte adicionado para o formato de tabela semelhante como cliente do helm</span><span class="sxs-lookup"><span data-stu-id="8eafc-109">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-110">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-110">ACS</span></span>
* <span data-ttu-id="8eafc-111">`aks [create|scale] --nodepool-name` adicionado para configurar o nome nodepool, truncado com 12 caracteres, padrão – nodepool1</span><span class="sxs-lookup"><span data-stu-id="8eafc-111">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="8eafc-112">Corrigido para voltar para “scp” quando Parimiko falha</span><span class="sxs-lookup"><span data-stu-id="8eafc-112">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="8eafc-113">`aks create` alterado para não precisar mais de `--aad-tenant-id`</span><span class="sxs-lookup"><span data-stu-id="8eafc-113">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="8eafc-114">Melhoria da mesclagem das credenciais do Kubernetes quando houver entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-114">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-115">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-115">Container</span></span>
* <span data-ttu-id="8eafc-116">`functionapp create` alterado para dar suporte à criação de um tipo de plano de consumo do Linux com um tempo de execução específico</span><span class="sxs-lookup"><span data-stu-id="8eafc-116">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="8eafc-117">[VERSÃO PRÉVIA] Suporte adicionado para hospedar aplicativos Web nos contêineres do Windows</span><span class="sxs-lookup"><span data-stu-id="8eafc-117">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="8eafc-118">Hub de evento</span><span class="sxs-lookup"><span data-stu-id="8eafc-118">Event Hub</span></span>
* <span data-ttu-id="8eafc-119">Corrigido o comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-119">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="8eafc-120">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="8eafc-120">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="8eafc-121">Extensões</span><span class="sxs-lookup"><span data-stu-id="8eafc-121">Extensions</span></span>
* <span data-ttu-id="8eafc-122">Corrigido o problema ao tentar adicionar uma extensão já instalada</span><span class="sxs-lookup"><span data-stu-id="8eafc-122">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8eafc-123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8eafc-123">HDInsight</span></span>
* <span data-ttu-id="8eafc-124">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-124">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-125">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-125">IoT</span></span>
* <span data-ttu-id="8eafc-126">Comando de instalação da extensão adicionado à faixa inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-126">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-127">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8eafc-127">KeyVault</span></span>
* <span data-ttu-id="8eafc-128">Alterado para restringir os comandos de armazenamento do keyvault ao perfil da API mais recente</span><span class="sxs-lookup"><span data-stu-id="8eafc-128">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-129">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-129">Network</span></span>
* <span data-ttu-id="8eafc-130">`network dns zone create` corrigido: o comando terá êxito mesmo se o usuário tiver configurado um local padrão.</span><span class="sxs-lookup"><span data-stu-id="8eafc-130">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="8eafc-131">Veja o n° 6052</span><span class="sxs-lookup"><span data-stu-id="8eafc-131">See #6052</span></span>
* <span data-ttu-id="8eafc-132">Preterido `--remote-vnet-id` para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-132">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="8eafc-133">`--remote-vnet` a `network vnet peering create` adicionados, que aceita um nome ou uma ID</span><span class="sxs-lookup"><span data-stu-id="8eafc-133">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="8eafc-134">Suporte adicionado para vários prefixos de sub-rede a `network vnet create` com `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8eafc-134">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="8eafc-135">Suporte adicionado para vários prefixos de sub-rede a `network vnet subnet [create|update]` com `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8eafc-135">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="8eafc-136">Corrigido o problema com `network application-gateway create` que impedia a criação de gateways com a SKU `WAF_v2` ou `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="8eafc-136">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="8eafc-137">Argumento de conveniência `--service-endpoint-policy` adicionado a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-137">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-138">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-138">Role</span></span>
* <span data-ttu-id="8eafc-139">Suporte adicionado para listar os proprietários de aplicativo do Azure AD para `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="8eafc-139">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="8eafc-140">Suporte adicionado para listar os proprietários da entidade de serviço do Azure AD para `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="8eafc-140">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="8eafc-141">Alterado para garantir que os comandos para criar e atualizar a definição da função aceitem várias configurações de permissão</span><span class="sxs-lookup"><span data-stu-id="8eafc-141">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="8eafc-142">`ad sp create-for-rbac` alterado para garantir que a URI da home page sempre seja "https"</span><span class="sxs-lookup"><span data-stu-id="8eafc-142">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="8eafc-143">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-143">Service Bus</span></span>
* <span data-ttu-id="8eafc-144">[ALTERAÇÃO SIGNIFICATIVA] `list` comandos alterados para lidar com os erros de recurso(s) NotFound(404) do modo típico, em vez de mostrar uma lista vazia</span><span class="sxs-lookup"><span data-stu-id="8eafc-144">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-145">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-145">VM</span></span>
* <span data-ttu-id="8eafc-146">Corrigido o campo `accessSas` vazio em `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="8eafc-146">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="8eafc-147">`vmss create` alterado para reservar um intervalo de portas de front-end grande o suficiente para lidar com excesso de provisionamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-147">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="8eafc-148">Corrigidos os comandos de atualização para `sig`</span><span class="sxs-lookup"><span data-stu-id="8eafc-148">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="8eafc-149">Suporte `--no-wait` adicionado para gerenciar as versões da imagem em `sig`</span><span class="sxs-lookup"><span data-stu-id="8eafc-149">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="8eafc-150">`vm list-ip-addresses` alterado para mostrar a zona de disponibilidade dos endereços IP públicos</span><span class="sxs-lookup"><span data-stu-id="8eafc-150">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="8eafc-151">`[vm|vmss] disk attach` alterado para definir o LUN padrão do disco para o primeiro ponto disponível</span><span class="sxs-lookup"><span data-stu-id="8eafc-151">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="8eafc-152">21 de setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-152">September 21, 2018</span></span>

<span data-ttu-id="8eafc-153">Versão 2.0.46</span><span class="sxs-lookup"><span data-stu-id="8eafc-153">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-154">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-154">ACR</span></span>
* <span data-ttu-id="8eafc-155">Adicionados comandos de tarefa de ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-155">Added ACR Task commands</span></span>
* <span data-ttu-id="8eafc-156">Adicionado o comando de execução rápido</span><span class="sxs-lookup"><span data-stu-id="8eafc-156">Added quick run command</span></span>
* <span data-ttu-id="8eafc-157">Grupo de comandos `build-task` preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-157">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="8eafc-158">Adicionado o grupo de comando `helm` para dar suporte ao gerenciamento de gráficos Helm com o ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-158">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="8eafc-159">Suporte adicionado para criação idempotente para registro gerenciado</span><span class="sxs-lookup"><span data-stu-id="8eafc-159">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="8eafc-160">Adicionado um sinalizador de formato no para exibir logs de build</span><span class="sxs-lookup"><span data-stu-id="8eafc-160">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-161">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-161">ACS</span></span>
* <span data-ttu-id="8eafc-162">Alterado o comando `install-connector` para definir o FQDN mestre do AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-162">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="8eafc-163">Corrigida a criação de atribuição de função para vnet-subnet-id ao não especificar a entidade de serviço e skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="8eafc-163">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-164">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-164">AppService</span></span>

* <span data-ttu-id="8eafc-165">Adicionado suporte para o gerenciamento de operações de WebJobs (contínuos e disparados)</span><span class="sxs-lookup"><span data-stu-id="8eafc-165">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="8eafc-166">Suporte de az webapp config set para a propriedade --fts-state property. Adicionado suporte também para az functionapp config set & show</span><span class="sxs-lookup"><span data-stu-id="8eafc-166">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="8eafc-167">Adicionado suporte para trazer seu próprio armazenamento para aplicativos Web</span><span class="sxs-lookup"><span data-stu-id="8eafc-167">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="8eafc-168">Adicionado suporte para a listar e restaurar aplicativos Web excluídos</span><span class="sxs-lookup"><span data-stu-id="8eafc-168">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-169">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-169">Batch</span></span>
* <span data-ttu-id="8eafc-170">Alterada a inclusão de tarefas por meio de `--json-file` para dar suporte à sintaxe AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="8eafc-170">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="8eafc-171">Atualizada a documentação de formatos `--json-file` aceitos</span><span class="sxs-lookup"><span data-stu-id="8eafc-171">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="8eafc-172">`--max-tasks-per-node-option` foi adicionado a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-172">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="8eafc-173">Alterado o comportamento de `batch account` para mostrar as contas atualmente conectadas se nenhuma opção foi especificada</span><span class="sxs-lookup"><span data-stu-id="8eafc-173">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8eafc-174">Lote AI</span><span class="sxs-lookup"><span data-stu-id="8eafc-174">Batch AI</span></span> 
* <span data-ttu-id="8eafc-175">Corrigida a falha na criação de conta de armazenamento automática no comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-175">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8eafc-176">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-176">Cognitive Services</span></span>
* <span data-ttu-id="8eafc-177">Adicionado o complemento para os argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="8eafc-177">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="8eafc-178">Adicionado o comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="8eafc-178">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="8eafc-179">Adicionado o comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="8eafc-179">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="8eafc-180">Adicionado o comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-180">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="8eafc-181">Preterido `cognitiveservices list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-181">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="8eafc-182">Alterado `--name` para que seja opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="8eafc-182">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-183">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-183">Container</span></span>
* <span data-ttu-id="8eafc-184">Adicionada a capacidade de reiniciar e parar um grupo de contêineres em execução</span><span class="sxs-lookup"><span data-stu-id="8eafc-184">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="8eafc-185">Adicionado `--network-profile` para passar em um perfil de rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-185">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="8eafc-186">Adicionado `--subnet`, `--vnet_name`, para permitir a criação de grupos de contêineres em uma rede virtual</span><span class="sxs-lookup"><span data-stu-id="8eafc-186">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="8eafc-187">Alterada a saída da tabela para mostrar o status do grupo de contêineres</span><span class="sxs-lookup"><span data-stu-id="8eafc-187">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="8eafc-188">DataLake</span><span class="sxs-lookup"><span data-stu-id="8eafc-188">Datalake</span></span>
* <span data-ttu-id="8eafc-189">Comandos adicionados para regras de rede virtual</span><span class="sxs-lookup"><span data-stu-id="8eafc-189">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="8eafc-190">Shell interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-190">Interactive Shell</span></span>
* <span data-ttu-id="8eafc-191">Corrigido o erro no Windows em que comandos não são executados corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-191">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="8eafc-192">Corrigido o problema para carregar o comando no modo interativo que era causado por objetos preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-192">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-193">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-193">IoT</span></span>
* <span data-ttu-id="8eafc-194">Adicionado suporte para roteamento de Hubs de IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-194">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="8eafc-195">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8eafc-195">Key Vault</span></span>
* <span data-ttu-id="8eafc-196">Corrigida a importação de chave do Key Vault para chaves RSA</span><span class="sxs-lookup"><span data-stu-id="8eafc-196">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-197">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-197">Network</span></span>
* <span data-ttu-id="8eafc-198">Adicionados os comandos `network public-ip prefix` para dar suporte a recursos de prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="8eafc-198">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="8eafc-199">Adicionados os comandos `network service-endpoint` para dar suporte a recursos de política de ponto de extremidade de serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-199">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="8eafc-200">Adicionados os comandos `network lb outbound-rule` para dar suporte à criação de regras de saída do Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="8eafc-200">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="8eafc-201">Adicionado `--public-ip-prefix` a `network lb frontend-ip create/update` para dar suporte a configurações de IP de front-end usando prefixos de IP público</span><span class="sxs-lookup"><span data-stu-id="8eafc-201">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="8eafc-202">Adicionado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-202">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="8eafc-203">Adicionado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-203">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="8eafc-204">Permitido o uso de `network watcher flow-log show/configure` com NSGs clássicos</span><span class="sxs-lookup"><span data-stu-id="8eafc-204">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="8eafc-205">Adição do comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="8eafc-205">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="8eafc-206">Corrigido o comando `network watcher test-connectivity` e adicionadas as propriedades `--method`, `--valid-status-codes` e `--headers`</span><span class="sxs-lookup"><span data-stu-id="8eafc-206">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="8eafc-207">`network express-route create/update`: Adicionado o sinalizador `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="8eafc-207">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="8eafc-208">`network vnet subnet create/update`: Adicionado suporte para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="8eafc-208">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="8eafc-209">Adicionado o comando `network vnet subnet list-available-delegations`</span><span class="sxs-lookup"><span data-stu-id="8eafc-209">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="8eafc-210">`network traffic-manager profile create/update`: Adicionado suporte para `--interval`, `--timeout` e `--max-failures` para as opções preteridas de configuração do monitor `--monitor-path`, `--monitor-port` e `--monitor-protocol`, que foram substituídas por `--path`, `--port` e `--protocol`</span><span class="sxs-lookup"><span data-stu-id="8eafc-210">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="8eafc-211">`network lb frontend-ip create/update`: Corrigida a lógica para configurar o método de alocação de IP privado. Se um endereço IP privado for fornecido, a alocação será estática. Se nenhum endereço IP privado for fornecido ou uma cadeia de caracteres vazia for fornecida para o endereço IP privado, a alocação será dinâmica.</span><span class="sxs-lookup"><span data-stu-id="8eafc-211">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="8eafc-212">`dns record-set * create/update`: Adicionado suporte para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="8eafc-212">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="8eafc-213">Adicionados comandos `network interface-endpoint` para consultar objetos do ponto de extremidade da interface</span><span class="sxs-lookup"><span data-stu-id="8eafc-213">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="8eafc-214">Adicionado `network profile show/list/delete` para gerenciamento parcial dos perfis de rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-214">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="8eafc-215">Adicionados comandos `network express-route peering connection` para gerenciar conexões de emparelhamento entre as ExpressRoutes</span><span class="sxs-lookup"><span data-stu-id="8eafc-215">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-216">RDBMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-216">RDBMS</span></span>
* <span data-ttu-id="8eafc-217">Adicionado suporte para o serviço MariaDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-217">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="8eafc-218">Reserva</span><span class="sxs-lookup"><span data-stu-id="8eafc-218">Reservation</span></span>
* <span data-ttu-id="8eafc-219">Adicionado CosmosDB no tipo enumerado de recurso reservado</span><span class="sxs-lookup"><span data-stu-id="8eafc-219">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="8eafc-220">Adicionada a propriedade nome no modelo do Patch</span><span class="sxs-lookup"><span data-stu-id="8eafc-220">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="8eafc-221">Gerenciar aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-221">Manage App</span></span>
* <span data-ttu-id="8eafc-222">Corrigido o bug em `managedapp create --kind MarketPlace` que resultava em falha durante a criação da instância de um aplicativo gerenciado do Marketplace</span><span class="sxs-lookup"><span data-stu-id="8eafc-222">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="8eafc-223">Alterados os comandos `feature` para serem restritos somente aos perfis com suporte</span><span class="sxs-lookup"><span data-stu-id="8eafc-223">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-224">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-224">Role</span></span>
* <span data-ttu-id="8eafc-225">Adicionado suporte para listar membros de grupo de usuários</span><span class="sxs-lookup"><span data-stu-id="8eafc-225">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="8eafc-226">SignalR</span><span class="sxs-lookup"><span data-stu-id="8eafc-226">SignalR</span></span>
* <span data-ttu-id="8eafc-227">Primeira versão</span><span class="sxs-lookup"><span data-stu-id="8eafc-227">First release</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-228">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-228">Storage</span></span>
* <span data-ttu-id="8eafc-229">Adicionado o parâmetro `--auth-mode login` para usar as credenciais de login do usuário para autorização de filas e blobs</span><span class="sxs-lookup"><span data-stu-id="8eafc-229">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="8eafc-230">Adicionado `storage container immutability-policy/legal-hold` para gerenciar o armazenamento imutável</span><span class="sxs-lookup"><span data-stu-id="8eafc-230">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-231">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-231">VM</span></span>
* <span data-ttu-id="8eafc-232">Corrigido o problema em que `vm create --generate-ssh-keys` sobrescreve o arquivo de chave privada se o arquivo de chave pública estiver ausente (#4725, #6780)</span><span class="sxs-lookup"><span data-stu-id="8eafc-232">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="8eafc-233">Adicionado suporte para galeria de imagem compartilhada através de `az sig`</span><span class="sxs-lookup"><span data-stu-id="8eafc-233">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="8eafc-234">28 de Agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-234">August 28, 2018</span></span>

<span data-ttu-id="8eafc-235">Versão 2.0.45</span><span class="sxs-lookup"><span data-stu-id="8eafc-235">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-236">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-236">Core</span></span>

* <span data-ttu-id="8eafc-237">Corrigido o problema de carregamento de arquivo de configuração vazio</span><span class="sxs-lookup"><span data-stu-id="8eafc-237">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="8eafc-238">Adicionado suporte para o perfil `2018-03-01-hybrid` para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8eafc-238">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-239">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-239">ACR</span></span>

* <span data-ttu-id="8eafc-240">Adicionada uma solução alternativa para operações de tempo de execução sem solicitações ARM</span><span class="sxs-lookup"><span data-stu-id="8eafc-240">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="8eafc-241">Alterado para excluir arquivos de controle de versão (por exemplo, .git, .gitignore) de tar carregados por padrão no comando `build`</span><span class="sxs-lookup"><span data-stu-id="8eafc-241">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-242">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-242">ACS</span></span>

* <span data-ttu-id="8eafc-243">Alterado `aks create` para os padrões para VMs `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="8eafc-243">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="8eafc-244">Alterado `aks get-credentials` para agora chamar novas APIs para obter credenciais de cluster</span><span class="sxs-lookup"><span data-stu-id="8eafc-244">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-245">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-245">AppService</span></span>

* <span data-ttu-id="8eafc-246">Adicionado suporte para CORS no functionapp e webapp</span><span class="sxs-lookup"><span data-stu-id="8eafc-246">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="8eafc-247">Adicionado suporte a marcas ARM ao criar comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-247">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="8eafc-248">Alterado `[webapp|functionapp] identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-248">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="8eafc-249">Backup</span><span class="sxs-lookup"><span data-stu-id="8eafc-249">Backup</span></span>

* <span data-ttu-id="8eafc-250">Alterado `backup vault backup-properties show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-250">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="8eafc-251">Serviço de Bot</span><span class="sxs-lookup"><span data-stu-id="8eafc-251">Bot Service</span></span>

* <span data-ttu-id="8eafc-252">Versão da CLI do serviço de Bot inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-252">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8eafc-253">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-253">Cognitive Services</span></span>

* <span data-ttu-id="8eafc-254">Adicionado novo parâmetro `--api-properties,` que é necessário para a criação de alguns dos serviços</span><span class="sxs-lookup"><span data-stu-id="8eafc-254">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-255">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-255">IoT</span></span>

* <span data-ttu-id="8eafc-256">Corrigido o problema com a associação de hubs vinculados</span><span class="sxs-lookup"><span data-stu-id="8eafc-256">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-257">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-257">Monitor</span></span>

* <span data-ttu-id="8eafc-258">Adicionados comandos `monitor metrics alert` para alertas de métrica quase em tempo real</span><span class="sxs-lookup"><span data-stu-id="8eafc-258">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="8eafc-259">Comandos `monitor alert` preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-259">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-260">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-260">Network</span></span>

* <span data-ttu-id="8eafc-261">Alterado `network application-gateway ssl-policy predefined show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-261">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-262">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-262">Resource</span></span>

* <span data-ttu-id="8eafc-263">Alterado `provider operation show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-263">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-264">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-264">Storage</span></span>

* <span data-ttu-id="8eafc-265">Alterado `storage share policy show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-265">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-266">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-266">VM</span></span>

* <span data-ttu-id="8eafc-267">Alterado `vm/vmss identity show` para sair com o código 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-267">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="8eafc-268">Preterido `--storage-caching` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-268">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="8eafc-269">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-269">Auguest 14, 2018</span></span>

<span data-ttu-id="8eafc-270">Versão 2.0.44</span><span class="sxs-lookup"><span data-stu-id="8eafc-270">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-271">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-271">Core</span></span>

* <span data-ttu-id="8eafc-272">Corrigida a exibição numérica na saída `table`</span><span class="sxs-lookup"><span data-stu-id="8eafc-272">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="8eafc-273">Adicionado o formato de saída YAML</span><span class="sxs-lookup"><span data-stu-id="8eafc-273">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="8eafc-274">Telemetria</span><span class="sxs-lookup"><span data-stu-id="8eafc-274">Telemetry</span></span>

* <span data-ttu-id="8eafc-275">Melhorias nos relatórios de telemetria</span><span class="sxs-lookup"><span data-stu-id="8eafc-275">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-276">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-276">ACR</span></span>

* <span data-ttu-id="8eafc-277">Adicionados os comandos `content-trust policy`</span><span class="sxs-lookup"><span data-stu-id="8eafc-277">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="8eafc-278">Corrigido o problema onde `.dockerignore` não foi tratado adequadamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-278">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-279">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-279">ACS</span></span>

* <span data-ttu-id="8eafc-280">Alterado `az acs/aks install-cli` para instalar em `%USERPROFILE%\.azure-kubectl` no Windows</span><span class="sxs-lookup"><span data-stu-id="8eafc-280">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="8eafc-281">Alterado `az aks install-connector` para detectar se o cluster tem RBAC e configurar o conector ACI adequadamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-281">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="8eafc-282">Alterado para atribuição de função à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="8eafc-282">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="8eafc-283">Adicionada uma nova opção para “ignorar a atribuição de função” à sub-rede quando ela é fornecida</span><span class="sxs-lookup"><span data-stu-id="8eafc-283">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="8eafc-284">Alterado para ignorar a atribuição de função à sub-rede quando a atribuição já existe</span><span class="sxs-lookup"><span data-stu-id="8eafc-284">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="8eafc-285">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-285">AppService</span></span>

* <span data-ttu-id="8eafc-286">Corrigido um bug que impede a criação de um aplicativo de funções usando contas de armazenamento em grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="8eafc-286">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="8eafc-287">Corrigida uma falha na implantação de zip</span><span class="sxs-lookup"><span data-stu-id="8eafc-287">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="8eafc-288">BatchAI</span><span class="sxs-lookup"><span data-stu-id="8eafc-288">BatchAI</span></span>

* <span data-ttu-id="8eafc-289">Alterada a saída do agente para criação de conta de armazenamento automática para especificar “*grupo* de recurso”.</span><span class="sxs-lookup"><span data-stu-id="8eafc-289">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="8eafc-290">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-290">Container</span></span>

* <span data-ttu-id="8eafc-291">Adicionado `--secure-environment-variables` para passar as variáveis de ambiente seguras para um contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-291">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="8eafc-292">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-292">IoT</span></span>

* <span data-ttu-id="8eafc-293">[ALTERAÇÃO SIGNIFICATIVA] Removidos os comandos preteridos que foram movidos para a extensão iot</span><span class="sxs-lookup"><span data-stu-id="8eafc-293">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="8eafc-294">Atualizados os elementos para não presumirem o domínio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="8eafc-294">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="8eafc-295">Central de IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-295">Iot Central</span></span>

* <span data-ttu-id="8eafc-296">Versão inicial do módulo do IoT Central</span><span class="sxs-lookup"><span data-stu-id="8eafc-296">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-297">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8eafc-297">KeyVault</span></span>


* <span data-ttu-id="8eafc-298">Comandos adicionados para gerenciar contas de armazenamento e as definições de sas</span><span class="sxs-lookup"><span data-stu-id="8eafc-298">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="8eafc-299">Comandos adicionados para regras de rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-299">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="8eafc-300">Adicionado o parâmetro `--id` para operações de certificado, chave e segredo</span><span class="sxs-lookup"><span data-stu-id="8eafc-300">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="8eafc-301">Adicionado suporte para a versão de várias APIs de gerenciamento KV</span><span class="sxs-lookup"><span data-stu-id="8eafc-301">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="8eafc-302">Adicionado suporte para a versão de várias APIs do plano de dados KV</span><span class="sxs-lookup"><span data-stu-id="8eafc-302">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="8eafc-303">Retransmissão</span><span class="sxs-lookup"><span data-stu-id="8eafc-303">Relay</span></span>

* <span data-ttu-id="8eafc-304">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-304">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-305">Sql</span><span class="sxs-lookup"><span data-stu-id="8eafc-305">Sql</span></span>

* <span data-ttu-id="8eafc-306">Adicionados os comandos `sql failover-group`</span><span class="sxs-lookup"><span data-stu-id="8eafc-306">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-307">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-307">Storage</span></span>

* <span data-ttu-id="8eafc-308">[ALTERAÇÃO SIGNIFICATIVA] Alterado `storage account show-usage` para exigir o parâmetro `--location` e listará por região</span><span class="sxs-lookup"><span data-stu-id="8eafc-308">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="8eafc-309">Alterado o parâmetro `--resource-group` para ser opcional para comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="8eafc-309">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="8eafc-310">Removidos os avisos de “Falha na pré-condição” para as falhas individuais em comandos em lote para uma única mensagem agregada</span><span class="sxs-lookup"><span data-stu-id="8eafc-310">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="8eafc-311">Alterados os comandos `[blob|file] delete-batch` para não exibir mais matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="8eafc-311">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="8eafc-312">Alterados os comandos `blob [download|upload|delete-batch]` para ler o token de sas da url do contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-312">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-313">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-313">VM</span></span>

* <span data-ttu-id="8eafc-314">Adicionado filtros comuns à `vm list-skus` para facilidade de uso</span><span class="sxs-lookup"><span data-stu-id="8eafc-314">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="8eafc-315">31 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-315">July 31, 2018</span></span>

<span data-ttu-id="8eafc-316">Versão 2.0.43</span><span class="sxs-lookup"><span data-stu-id="8eafc-316">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-317">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-317">ACR</span></span>

* <span data-ttu-id="8eafc-318">Sinalizador `--with-secure-properties` adicionado ao comando `acr build-task show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-318">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="8eafc-319">Adicionado o comando `acr build-task update-build`</span><span class="sxs-lookup"><span data-stu-id="8eafc-319">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-320">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-320">ACS</span></span>

* <span data-ttu-id="8eafc-321">Alterado para retornar 0 (êxito) ao terminar `az aks browse` pressionando [Ctrl+C]</span><span class="sxs-lookup"><span data-stu-id="8eafc-321">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-322">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-322">Batch</span></span>

* <span data-ttu-id="8eafc-323">Bug corrigido ao mostrar o token AAD no cloudshell</span><span class="sxs-lookup"><span data-stu-id="8eafc-323">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-324">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-324">Container</span></span>

* <span data-ttu-id="8eafc-325">Requisito removido de `--log-analytics-workspace-key` para o nome ou a ID ao definir assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-325">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-326">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-326">Network</span></span>

* <span data-ttu-id="8eafc-327">Suporte a DNS adicionado a 2017-03-09-profile para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8eafc-327">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="8eafc-328">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-328">Resource</span></span>

* <span data-ttu-id="8eafc-329">`--rollback-on-error` a `group deployment create` adicionado para executar uma implantação válida no erro</span><span class="sxs-lookup"><span data-stu-id="8eafc-329">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="8eafc-330">Problema corrigido onde `--parameters {}` com `group deployment create` resultou em um erro</span><span class="sxs-lookup"><span data-stu-id="8eafc-330">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-331">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-331">Role</span></span>

* <span data-ttu-id="8eafc-332">Suporte adicionado para o perfil da pilha 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="8eafc-332">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="8eafc-333">Problema corrigido onde os parâmetros de atualização genéricos para `app update` não funcionariam corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-333">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="8eafc-334">Search</span><span class="sxs-lookup"><span data-stu-id="8eafc-334">Search</span></span>

* <span data-ttu-id="8eafc-335">Comandos adicionados para o serviço Azure Search</span><span class="sxs-lookup"><span data-stu-id="8eafc-335">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="8eafc-336">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-336">Service Bus</span></span>

* <span data-ttu-id="8eafc-337">Grupo de comandos de migração adicionados para migrar um namespace do Barramento de Serviço Standard para Premium</span><span class="sxs-lookup"><span data-stu-id="8eafc-337">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="8eafc-338">Novas propriedades opcionais adicionadas à fila do Barramento de Serviço e à Assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-338">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="8eafc-339">`--enable-batched-operations` e `--enable-dead-lettering-on-message-expiration` em `queue`</span><span class="sxs-lookup"><span data-stu-id="8eafc-339">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="8eafc-340">`--dead-letter-on-filter-exceptions` em `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="8eafc-340">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-341">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-341">Storage</span></span>

* <span data-ttu-id="8eafc-342">Suporte adicionado para o download de arquivos grandes usando uma única conexão</span><span class="sxs-lookup"><span data-stu-id="8eafc-342">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="8eafc-343">Comandos `show` convertidos que foram perdidos na falha com código de saída 3 mediante um recurso ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-343">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-344">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-344">VM</span></span>

* <span data-ttu-id="8eafc-345">Suporte adicionado para listar conjuntos de disponibilidade por assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-345">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="8eafc-346">Adicionado o suporte para `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="8eafc-346">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="8eafc-347">Suporte adicionado para o grupo de segurança do aplicativo ao criar um conjunto de dimensionamento da VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-347">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="8eafc-348">[ALTERAÇÃO SIGNIFICATIVA] `[vm|vmss] create`, `[vm|vmss] identity assign` e `[vm|vmss] identity remove` alterados para produzir identidades de usuário atribuídas no formato de dicionário</span><span class="sxs-lookup"><span data-stu-id="8eafc-348">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="8eafc-349">18 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-349">July 18, 2018</span></span>

<span data-ttu-id="8eafc-350">Versão 2.0.42</span><span class="sxs-lookup"><span data-stu-id="8eafc-350">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-351">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-351">Core</span></span>

* <span data-ttu-id="8eafc-352">Adicionado suporte para logon baseado em navegador, na janela de bash WSL</span><span class="sxs-lookup"><span data-stu-id="8eafc-352">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="8eafc-353">O sinalizador `--force-string` foi adicionado a todos os comandos de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="8eafc-353">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="8eafc-354">[ALTERAÇÃO SIGNIFICATIVA] Os comandos 'show' foram alterados para registrar mensagens de erro e falha com código de saída 3 quando um recurso está ausente</span><span class="sxs-lookup"><span data-stu-id="8eafc-354">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-355">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-355">ACR</span></span>

* <span data-ttu-id="8eafc-356">[ALTERAÇÃO SIGNIFICATIVA] '--no-push' foi atualizado para um sinalizador puro no comando 'acr build'</span><span class="sxs-lookup"><span data-stu-id="8eafc-356">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="8eafc-357">Foram adicionados os comandos `show` e `update` no grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="8eafc-357">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="8eafc-358">Foi adicionado o sinalizador `--detail` a `show-manifests` e `show-tags` para mostrar informações mais detalhadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-358">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="8eafc-359">Foi adicionado o parâmetro `--image` para dar suporte aos detalhes do build get ou aos logs por meio de uma imagem</span><span class="sxs-lookup"><span data-stu-id="8eafc-359">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-360">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-360">ACS</span></span>

* <span data-ttu-id="8eafc-361">`az aks create` foi alterado para excluir o erro se `--max-pods` for menor que 5</span><span class="sxs-lookup"><span data-stu-id="8eafc-361">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-362">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-362">AppService</span></span>

* <span data-ttu-id="8eafc-363">Suporte adicionado para skus PremiumV2</span><span class="sxs-lookup"><span data-stu-id="8eafc-363">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-364">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-364">Batch</span></span>

* <span data-ttu-id="8eafc-365">Corrigido o bug sobre como usar a credencial de token no modo do Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8eafc-365">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="8eafc-366">Alterada a entrada JSON para diferenciar maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="8eafc-366">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8eafc-367">Lote AI</span><span class="sxs-lookup"><span data-stu-id="8eafc-367">Batch AI</span></span>

* <span data-ttu-id="8eafc-368">Corrigido o comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="8eafc-368">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-369">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-369">Container</span></span>

* <span data-ttu-id="8eafc-370">Removido o requisito de nome de usuário e senha para os registros não dockerhub</span><span class="sxs-lookup"><span data-stu-id="8eafc-370">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="8eafc-371">Correção de erro durante a criação de grupos de contêineres de arquivo yaml</span><span class="sxs-lookup"><span data-stu-id="8eafc-371">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-372">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-372">Network</span></span>

* <span data-ttu-id="8eafc-373">Adicionado o suporte `--no-wait` para `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-373">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="8eafc-374">Adicionado `network nic wait`</span><span class="sxs-lookup"><span data-stu-id="8eafc-374">Added `network nic wait`</span></span>
* <span data-ttu-id="8eafc-375">Preterido o argumento `--ids` para `network vnet [subnet|peering] list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-375">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="8eafc-376">Adicionado o sinalizador `--include-default` para incluir regras de segurança padrão na saída do `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-376">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="8eafc-377">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-377">Resource</span></span>

* <span data-ttu-id="8eafc-378">Adicionado o suporte `--no-wait` para `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="8eafc-378">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="8eafc-379">Adicionado o suporte `--no-wait` para `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="8eafc-379">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="8eafc-380">Adicionado o comando `deployment wait`</span><span class="sxs-lookup"><span data-stu-id="8eafc-380">Added `deployment wait` command</span></span>
* <span data-ttu-id="8eafc-381">Correção do problema em que os comandos de nível de assinatura `az deployment` erroneamente apareceram no perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="8eafc-381">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-382">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-382">SQL</span></span>

* <span data-ttu-id="8eafc-383">O erro “O nome de grupo de recursos fornecido ... não correspondeu ao nome na Url” foi fixado ao especificar o nome do pool elástico para os comandos `sql db copy` e `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-383">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="8eafc-384">Permitir a configuração do padrão do SQL Server, executando `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="8eafc-384">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="8eafc-385">Os formatadores de tabela foram implementados aos comandos `sql server`, `sql server firewall-rule`, `sql list-usages` e `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="8eafc-385">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-386">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-386">Storage</span></span>

* <span data-ttu-id="8eafc-387">Adicionada a propriedade `pageRanges` à saída `storage blob show` que será preenchida para blobs de página</span><span class="sxs-lookup"><span data-stu-id="8eafc-387">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-388">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-388">VM</span></span>

* <span data-ttu-id="8eafc-389">[ALTERAÇÃO SIGNIFICATIVA] Alterado `vmss create` para usar o `Standard_DS1_v2` como o tamanho de instância padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-389">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="8eafc-390">Adicionado o suporte `--no-wait` para `vm extension [set|delete]` e `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-390">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="8eafc-391">Adicionado `vm extension wait`</span><span class="sxs-lookup"><span data-stu-id="8eafc-391">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8eafc-392">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-392">July 3, 2018</span></span>

<span data-ttu-id="8eafc-393">Versão 2.0.41</span><span class="sxs-lookup"><span data-stu-id="8eafc-393">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="8eafc-394">AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-394">AKS</span></span>

* <span data-ttu-id="8eafc-395">Monitoramento alterado para usar a ID de assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-395">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8eafc-396">3 de julho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-396">July 3, 2018</span></span>

<span data-ttu-id="8eafc-397">Versão 2.0.40</span><span class="sxs-lookup"><span data-stu-id="8eafc-397">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-398">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-398">Core</span></span>

* <span data-ttu-id="8eafc-399">Adicionado um novo fluxo de código de autorização para o logon interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-399">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-400">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-400">ACR</span></span>

* <span data-ttu-id="8eafc-401">Status da compilação de sondagem adicionado</span><span class="sxs-lookup"><span data-stu-id="8eafc-401">Added polling build status</span></span>
* <span data-ttu-id="8eafc-402">Suporte adicionado para valores de enumeração que não diferenciam maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="8eafc-402">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="8eafc-403">Parâmetros `--top` e `--orderby` adicionados para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="8eafc-403">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-404">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-404">ACS</span></span>

* <span data-ttu-id="8eafc-405">[ALTERAÇÃO SIGNIFICATIVA] Habilitar controle de acesso baseado em funções do Kubernetes por padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-405">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="8eafc-406">Argumento `--disable-rbac` e preterido `--enable-rbac` adicionados, pois é o padrão agora</span><span class="sxs-lookup"><span data-stu-id="8eafc-406">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="8eafc-407">Opções atualizadas do comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-407">Updated options for `aks browse` command.</span></span> <span data-ttu-id="8eafc-408">Suporte `--listen-port` adicionado</span><span class="sxs-lookup"><span data-stu-id="8eafc-408">Added `--listen-port` support</span></span>
* <span data-ttu-id="8eafc-409">Atualizado o pacote de gráficos do helm padrão para o comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-409">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="8eafc-410">Usar virtual-kubelet-para-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="8eafc-410">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="8eafc-411">Comandos `aks enable-addons` e `aks disable-addons` adicionados para atualizar um cluster existente</span><span class="sxs-lookup"><span data-stu-id="8eafc-411">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-412">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-412">AppService</span></span>

* <span data-ttu-id="8eafc-413">Suporte adicionado para desabilitar a identidade via `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="8eafc-413">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="8eafc-414">Marca `preview` removida para o recurso de Identidade</span><span class="sxs-lookup"><span data-stu-id="8eafc-414">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="8eafc-415">Backup</span><span class="sxs-lookup"><span data-stu-id="8eafc-415">Backup</span></span>

* <span data-ttu-id="8eafc-416">Definição do módulo atualizada</span><span class="sxs-lookup"><span data-stu-id="8eafc-416">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="8eafc-417">BatchAI</span><span class="sxs-lookup"><span data-stu-id="8eafc-417">BatchAI</span></span>

* <span data-ttu-id="8eafc-418">Saída da tabela corrigida para comandos `batchai cluster node list` e `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-418">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="8eafc-419">Nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-419">Cloud</span></span>

* <span data-ttu-id="8eafc-420">Sufixo do servidor `acr login` adicionado à configuração de nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-420">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-421">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-421">Container</span></span>

* <span data-ttu-id="8eafc-422">`container create` alterado para padrão para a operação de longa execução</span><span class="sxs-lookup"><span data-stu-id="8eafc-422">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="8eafc-423">Parâmetros `--log-analytics-workspace` e `--log-analytics-workspace-key` adicionados do Log Analytics</span><span class="sxs-lookup"><span data-stu-id="8eafc-423">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="8eafc-424">Parâmetro `--protocol` adicionado para especificar qual protocolo de rede usar</span><span class="sxs-lookup"><span data-stu-id="8eafc-424">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-425">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-425">Extension</span></span>

* <span data-ttu-id="8eafc-426">`extension list-available` alterado para mostrar apenas as extensões compatíveis com a versão da CLI</span><span class="sxs-lookup"><span data-stu-id="8eafc-426">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-427">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-427">Network</span></span>

* <span data-ttu-id="8eafc-428">Corrigido o problema onde os tipos de registro diferenciam maiúsculas de minúsculas ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="8eafc-428">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-429">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8eafc-429">Rdbms</span></span>

* <span data-ttu-id="8eafc-430">Adicionados os comandos `[postgres|myql] server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="8eafc-430">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-431">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-431">Resource</span></span>

* <span data-ttu-id="8eafc-432">Novo grupo de operação `deployment` adicionado</span><span class="sxs-lookup"><span data-stu-id="8eafc-432">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-433">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-433">VM</span></span>

* <span data-ttu-id="8eafc-434">Suporte adicionado para remover a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="8eafc-434">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="8eafc-435">25 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-435">June 25, 2018</span></span>

<span data-ttu-id="8eafc-436">Versão 2.0.39</span><span class="sxs-lookup"><span data-stu-id="8eafc-436">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="8eafc-437">CLI</span><span class="sxs-lookup"><span data-stu-id="8eafc-437">CLI</span></span>

* <span data-ttu-id="8eafc-438">Corte de arquivo atualizado no instalador MSI para corrigir o problema de instalação da extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-438">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="8eafc-439">19 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-439">June 19, 2018</span></span>

<span data-ttu-id="8eafc-440">Versão 2.0.38</span><span class="sxs-lookup"><span data-stu-id="8eafc-440">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-441">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-441">Core</span></span>

* <span data-ttu-id="8eafc-442">Suporte global adicionado para `--subscription` a maioria dos comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-442">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-443">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-443">ACR</span></span>

* <span data-ttu-id="8eafc-444">`azure-storage-blob` foi adicionado como dependência</span><span class="sxs-lookup"><span data-stu-id="8eafc-444">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="8eafc-445">A configuração de CPU padrão foi alterada com `acr build-task create` para usar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="8eafc-445">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-446">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-446">ACS</span></span>

* <span data-ttu-id="8eafc-447">As opções do comando `aks use-dev-spaces` foram atualizadas.</span><span class="sxs-lookup"><span data-stu-id="8eafc-447">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="8eafc-448">Suporte `--update` adicionado</span><span class="sxs-lookup"><span data-stu-id="8eafc-448">Added `--update` support</span></span>
* <span data-ttu-id="8eafc-449">`aks get-credentials --admin` foi alterado para substituir o contexto do usuário em `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="8eafc-449">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="8eafc-450">A propriedade `nodeResourceGroup` somente leitura foi exposta em clusters gerenciados</span><span class="sxs-lookup"><span data-stu-id="8eafc-450">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="8eafc-451">O erro de comando `acs browse` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="8eafc-451">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="8eafc-452">Foram feitas `--connector-name` opcional para `aks install-connector`, `aks upgrade-connector` e `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="8eafc-452">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="8eafc-453">Novas regiões de Instância de Contêiner do Azure foram adicionadas para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8eafc-453">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="8eafc-454">O local normalizado foi adicionado no nome de versão do comando e no nome do nó para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8eafc-454">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-455">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-455">AppService</span></span>

* <span data-ttu-id="8eafc-456">Foi adicionado suporte para versões mais recentes do urllib</span><span class="sxs-lookup"><span data-stu-id="8eafc-456">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="8eafc-457">Foi adicionado suporte para `functionapp create` para usar o plano de serviço de aplicativo de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="8eafc-457">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-458">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-458">Batch</span></span>

* <span data-ttu-id="8eafc-459">A dependência `azure-batch-extensions` foi removida</span><span class="sxs-lookup"><span data-stu-id="8eafc-459">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8eafc-460">Lote AI</span><span class="sxs-lookup"><span data-stu-id="8eafc-460">Batch AI</span></span>

* <span data-ttu-id="8eafc-461">Foi adicionado suporte aos workspaces.</span><span class="sxs-lookup"><span data-stu-id="8eafc-461">Added support for workspaces.</span></span> <span data-ttu-id="8eafc-462">Os workspaces permitem agrupar clusters, servidores de arquivos e experimentos, removendo a limitação no número de recursos que podem ser criados</span><span class="sxs-lookup"><span data-stu-id="8eafc-462">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="8eafc-463">Foi adicionado suporte para os experimentos.</span><span class="sxs-lookup"><span data-stu-id="8eafc-463">Added support for experiments.</span></span> <span data-ttu-id="8eafc-464">Os experimentos permitem agrupar trabalhos em coleções removendo a limitação no número de trabalhos criados</span><span class="sxs-lookup"><span data-stu-id="8eafc-464">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="8eafc-465">Foi adicionado suporte para configurar `/dev/shm` para trabalhos em execução em um contêiner de docker</span><span class="sxs-lookup"><span data-stu-id="8eafc-465">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="8eafc-466">Foram adicionados os comandos `batchai cluster node exec` e `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-466">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="8eafc-467">Esses comandos permitem executar qualquer comando diretamente nos nós e fornece a funcionalidade de encaminhamento de porta.</span><span class="sxs-lookup"><span data-stu-id="8eafc-467">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="8eafc-468">Foi adicionado suporte a `--ids` para os comandos `batchai`</span><span class="sxs-lookup"><span data-stu-id="8eafc-468">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="8eafc-469">[ALTERAÇÃO SIGNIFICATIVA] Todos os clusters e servidores de arquivos devem ser criados nos espaços de trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-469">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="8eafc-470">[ALTERAÇÃO SIGNIFICATIVA] Os trabalhos devem ser criados nas experiências</span><span class="sxs-lookup"><span data-stu-id="8eafc-470">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="8eafc-471">[ALTERAÇÃO SIGNIFICATIVA] `--nfs-resource-group` foi removido dos comandos `cluster create` e `job create`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-471">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="8eafc-472">Para montar um NFS pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do servidor de arquivos através da opção `--nfs`</span><span class="sxs-lookup"><span data-stu-id="8eafc-472">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="8eafc-473">[ALTERAÇÃO SIGNIFICATIVA] `--cluster-resource-group` foi removido do comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-473">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="8eafc-474">Para enviar um trabalho em um cluster pertencente a outro workspace/grupo de recursos, forneça a ID de ARM do cluster através da opção `--cluster`</span><span class="sxs-lookup"><span data-stu-id="8eafc-474">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="8eafc-475">[ALTERAÇÃO SIGNIFICATIVA] O atributo `location` foi removido de trabalhos, cluster e servidores de arquivos.</span><span class="sxs-lookup"><span data-stu-id="8eafc-475">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="8eafc-476">Agora, o local é um atributo de um workspace.</span><span class="sxs-lookup"><span data-stu-id="8eafc-476">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="8eafc-477">[ALTERAÇÃO SIGNIFICATIVA] `--location` foi removido dos comandos `job create` e `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-477">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="8eafc-478">[ALTERAÇÃO SIGNIFICATIVA] Os nomes das opções curtas foi alterado para tornar a interface mais consistente:</span><span class="sxs-lookup"><span data-stu-id="8eafc-478">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="8eafc-479">[`--config`, `-c`] foi renomeado para [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="8eafc-479">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="8eafc-480">[`--cluster`, `-r`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="8eafc-480">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="8eafc-481">[`--cluster`, `-n`] foi renomeado para [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="8eafc-481">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="8eafc-482">[`--job`, `-n`] foi renomeado para [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="8eafc-482">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="8eafc-483">Mapas</span><span class="sxs-lookup"><span data-stu-id="8eafc-483">Maps</span></span>

* <span data-ttu-id="8eafc-484">[ALTERAÇÃO SIGNIFICATIVA] `maps account create` foi alterado para exigir a aceitação dos Termos de Serviço pelo prompt interativo ou sinalizador `--accept-tos`</span><span class="sxs-lookup"><span data-stu-id="8eafc-484">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-485">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-485">Network</span></span>

* <span data-ttu-id="8eafc-486">Foi adicionado suporte a `https` para `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="8eafc-486">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="8eafc-487">Foi corrigido o problema em que `--endpoint-status` diferenciava maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8eafc-487">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="8eafc-488">#6502</span><span class="sxs-lookup"><span data-stu-id="8eafc-488">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="8eafc-489">Reservas</span><span class="sxs-lookup"><span data-stu-id="8eafc-489">Reservations</span></span>

* <span data-ttu-id="8eafc-490">[ALTERAÇÃO SIGNIFICATIVA] Foi adicionado o parâmetro `ReservedResourceType` necessário a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-490">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="8eafc-491">Parâmetro `Location` adicionado a `reservations catalog show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-491">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="8eafc-492">[ALTERAÇÃO SIGNIFICATIVA] `kind` foi removido de `ReservationProperties`</span><span class="sxs-lookup"><span data-stu-id="8eafc-492">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="8eafc-493">[ALTERAÇÃO SIGNIFICATIVA] `capabilities` foi renomeado para `sku_properties` em `Catalog`</span><span class="sxs-lookup"><span data-stu-id="8eafc-493">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="8eafc-494">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `size` e `tier` foram removidas de `Catalog`</span><span class="sxs-lookup"><span data-stu-id="8eafc-494">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="8eafc-495">Parâmetro `InstanceFlexibility` adicionado a `reservations reservation update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-495">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-496">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-496">Role</span></span>

* <span data-ttu-id="8eafc-497">Tratamento de erro melhorado</span><span class="sxs-lookup"><span data-stu-id="8eafc-497">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-498">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-498">SQL</span></span>

* <span data-ttu-id="8eafc-499">Foi corrigido um erro confuso ao executar `az sql db list-editions` para um local que não está disponível para sua assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-499">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-500">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-500">Storage</span></span>

* <span data-ttu-id="8eafc-501">A saída da tabela foi alterada para `storage blob download` para ser mais legível</span><span class="sxs-lookup"><span data-stu-id="8eafc-501">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-502">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-502">VM</span></span>

* <span data-ttu-id="8eafc-503">A verificação da refinação do tamanho da VM foi aprimorada para o suporte de rede acelerada em `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-503">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="8eafc-504">Foi adicionado um aviso para `vmss create` informando que o tamanho padrão da VM será alternado de `Standard_D1_v2` para `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="8eafc-504">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="8eafc-505">Foi adicionado `--force-update` a `[vm|vmss] extension set` para atualizar a extensão mesmo quando a configuração não foi alterada</span><span class="sxs-lookup"><span data-stu-id="8eafc-505">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8eafc-506">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-506">June 13, 2018</span></span>

<span data-ttu-id="8eafc-507">Versão 2.0.37</span><span class="sxs-lookup"><span data-stu-id="8eafc-507">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-508">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-508">Core</span></span>

* <span data-ttu-id="8eafc-509">A telemetria interativa foi melhorada</span><span class="sxs-lookup"><span data-stu-id="8eafc-509">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8eafc-510">13 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-510">June 13, 2018</span></span>

<span data-ttu-id="8eafc-511">Versão 2.0.36</span><span class="sxs-lookup"><span data-stu-id="8eafc-511">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="8eafc-512">AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-512">AKS</span></span>

* <span data-ttu-id="8eafc-513">Foram adicionadas opções avançadas de rede para `aks create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-513">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="8eafc-514">Foram adicionados argumentos para `aks create` para habilitar o monitoramento e roteamento de HTTP</span><span class="sxs-lookup"><span data-stu-id="8eafc-514">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="8eafc-515">Adicionado o argumento `--no-ssh-key` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-515">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="8eafc-516">Adicionado o argumento `--enable-rbac` para `aks create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-516">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="8eafc-517">[VERSÃO PRÉVIA] Suporte adicionado para a autenticação do Azure Active Directory no `aks create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-517">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-518">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-518">AppService</span></span>

* <span data-ttu-id="8eafc-519">Foi corrigido um problema com as versões urllib incompatíveis</span><span class="sxs-lookup"><span data-stu-id="8eafc-519">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8eafc-520">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-520">June 5, 2018</span></span>

<span data-ttu-id="8eafc-521">Versão 2.0.35</span><span class="sxs-lookup"><span data-stu-id="8eafc-521">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-522">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-522">Interactive</span></span>

* <span data-ttu-id="8eafc-523">Foram adicionados limites para as dependências do modo interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-523">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8eafc-524">5 de junho de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-524">June 5, 2018</span></span>

<span data-ttu-id="8eafc-525">Versão 2.0.34</span><span class="sxs-lookup"><span data-stu-id="8eafc-525">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-526">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-526">Core</span></span>

* <span data-ttu-id="8eafc-527">Suporte adicionado para referência de recursos de locatário cruzado</span><span class="sxs-lookup"><span data-stu-id="8eafc-527">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="8eafc-528">Melhor confiabilidade de carregamento de telemetria</span><span class="sxs-lookup"><span data-stu-id="8eafc-528">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-529">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-529">ACR</span></span>

* <span data-ttu-id="8eafc-530">Suporte adicionado para VSTS como um local de origem remota</span><span class="sxs-lookup"><span data-stu-id="8eafc-530">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="8eafc-531">Adicionado o comando `acr import`</span><span class="sxs-lookup"><span data-stu-id="8eafc-531">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="8eafc-532">AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-532">AKS</span></span>

* <span data-ttu-id="8eafc-533">`aks get-credentials` foi alterado para criar o arquivo de configuração kube com permissões de sistema de arquivos mais seguras</span><span class="sxs-lookup"><span data-stu-id="8eafc-533">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-534">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-534">Batch</span></span>

* <span data-ttu-id="8eafc-535">Correção do bug na formatação de tabela da lista de Pool [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="8eafc-535">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-536">IOT</span><span class="sxs-lookup"><span data-stu-id="8eafc-536">IOT</span></span>

* <span data-ttu-id="8eafc-537">Suporte adicionado para a criação de Hubs IoT de Camada Básica</span><span class="sxs-lookup"><span data-stu-id="8eafc-537">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-538">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-538">Network</span></span>

* <span data-ttu-id="8eafc-539">`network vnet peering` melhorado</span><span class="sxs-lookup"><span data-stu-id="8eafc-539">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="8eafc-540">Informações sobre a Política</span><span class="sxs-lookup"><span data-stu-id="8eafc-540">Policy Insights</span></span>

* <span data-ttu-id="8eafc-541">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-541">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="8eafc-542">ARM</span><span class="sxs-lookup"><span data-stu-id="8eafc-542">ARM</span></span>

* <span data-ttu-id="8eafc-543">Comandos `account management-group` adicionados.</span><span class="sxs-lookup"><span data-stu-id="8eafc-543">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-544">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-544">SQL</span></span>

* <span data-ttu-id="8eafc-545">Novos comandos de instância gerenciada adicionados:</span><span class="sxs-lookup"><span data-stu-id="8eafc-545">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="8eafc-546">Novos comandos de banco de dados gerenciado adicionados:</span><span class="sxs-lookup"><span data-stu-id="8eafc-546">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="8eafc-547">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-547">Storage</span></span>

* <span data-ttu-id="8eafc-548">Mimetypes extra adicionados para json e javascript para ser deduzido de extensões de arquivo</span><span class="sxs-lookup"><span data-stu-id="8eafc-548">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-549">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-549">VM</span></span>

* <span data-ttu-id="8eafc-550">`vm list-skus` foi alterado para usar colunas fixas e adicionar o aviso de que `Tier` e `Size` serão removidos</span><span class="sxs-lookup"><span data-stu-id="8eafc-550">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="8eafc-551">Opção `--accelerated-networking` adicionada a `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-551">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="8eafc-552">`--tags` foi adicionado a `identity create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-552">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="8eafc-553">22 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-553">May 22, 2018</span></span>

<span data-ttu-id="8eafc-554">Versão 2.0.33</span><span class="sxs-lookup"><span data-stu-id="8eafc-554">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-555">Core</span></span>

* <span data-ttu-id="8eafc-556">Suporte adicionado para expandir `@` em nomes de arquivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-556">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-557">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-557">ACS</span></span>

* <span data-ttu-id="8eafc-558">Novos comandos de espaços de desenvolvimento `aks use-dev-spaces` e `aks remove-dev-spaces` foram adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-558">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="8eafc-559">Erro de digitação corrigido na mensagem de ajuda</span><span class="sxs-lookup"><span data-stu-id="8eafc-559">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-560">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-560">AppService</span></span>

* <span data-ttu-id="8eafc-561">Comandos melhorados de atualização genérica</span><span class="sxs-lookup"><span data-stu-id="8eafc-561">Improved generic update commands</span></span>
* <span data-ttu-id="8eafc-562">Suporte assíncrono adicionado para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="8eafc-562">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-563">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-563">Container</span></span>

* <span data-ttu-id="8eafc-564">Suporte adicionado para a exportação de um grupo de contêiner no formato yaml</span><span class="sxs-lookup"><span data-stu-id="8eafc-564">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="8eafc-565">Suporte adicionado para usar um arquivo yaml para criar/atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-565">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-566">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-566">Extension</span></span>

* <span data-ttu-id="8eafc-567">Remoção de extensões melhorada</span><span class="sxs-lookup"><span data-stu-id="8eafc-567">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-568">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-568">Interactive</span></span>

* <span data-ttu-id="8eafc-569">Log de alterações alterado para silenciar o analisador para conclusões</span><span class="sxs-lookup"><span data-stu-id="8eafc-569">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="8eafc-570">Manipulação aprimorada de caches de ajuda inválida</span><span class="sxs-lookup"><span data-stu-id="8eafc-570">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-571">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8eafc-571">KeyVault</span></span>

* <span data-ttu-id="8eafc-572">Comandos de keyvault corrigidos para trabalhar no cloud shell ou VMs com identidade</span><span class="sxs-lookup"><span data-stu-id="8eafc-572">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-573">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-573">Network</span></span>

* <span data-ttu-id="8eafc-574">Corrija o problema em que `network watcher show-topology` não funcionará com o nome de rede virtual e/ou sub-rede [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="8eafc-574">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="8eafc-575">Corrija o problema onde alguns comandos `network watcher` iriam declarar que o Observador de Rede não está habilitado para regiões quando na verdade é [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="8eafc-575">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-576">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-576">SQL</span></span>

* <span data-ttu-id="8eafc-577">[ALTERAÇÃO SIGNIFICATIVA] Objetos de resposta alterados retornados dos comandos `db` e `dw`:</span><span class="sxs-lookup"><span data-stu-id="8eafc-577">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="8eafc-578">A propriedade `serviceLevelObjective` foi renomeada para `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="8eafc-578">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="8eafc-579">As propriedades `currentServiceObjectiveId` e `requestedServiceObjectiveId` foram removidas</span><span class="sxs-lookup"><span data-stu-id="8eafc-579">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="8eafc-580">A propriedade `maxSizeBytes` foi alterada para ser um valor inteiro em vez de uma cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eafc-580">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="8eafc-581">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `db` e `dw` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="8eafc-581">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="8eafc-582">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-582">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="8eafc-583">Para atualizar, use o parâmetro `--service-objective` ou defina a propriedade `sku.name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-583">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="8eafc-584">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-584">`edition`.</span></span> <span data-ttu-id="8eafc-585">Para atualizar, use o parâmetro `--edition` ou defina a propriedade `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="8eafc-585">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="8eafc-586">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-586">`elasticPoolName`.</span></span> <span data-ttu-id="8eafc-587">Para atualizar, use o parâmetro `--elastic-pool` ou defina a propriedade `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="8eafc-587">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="8eafc-588">[ALTERAÇÃO SIGNIFICATIVA] As propriedades `elastic-pool` a seguir foram alteradas para somente leitura:</span><span class="sxs-lookup"><span data-stu-id="8eafc-588">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="8eafc-589">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-589">`edition`.</span></span> <span data-ttu-id="8eafc-590">Para atualizar, use o parâmetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="8eafc-590">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="8eafc-591">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-591">`dtu`.</span></span> <span data-ttu-id="8eafc-592">Para atualizar, use o parâmetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-592">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="8eafc-593">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-593">`databaseDtuMin`.</span></span> <span data-ttu-id="8eafc-594">Para atualizar, use o parâmetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-594">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="8eafc-595">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-595">`databaseDtuMax`.</span></span> <span data-ttu-id="8eafc-596">Para atualizar, use o parâmetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-596">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="8eafc-597">Os parâmetros `--family` e `--capacity` foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-597">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="8eafc-598">Os formatadores de tabela foram adicionados aos comandos `db`, `dw` e `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-598">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-599">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-599">Storage</span></span>

* <span data-ttu-id="8eafc-600">Complemento adicionado ao argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-600">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="8eafc-601">O problema com `storage entity query` foi corrigido</span><span class="sxs-lookup"><span data-stu-id="8eafc-601">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-602">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-602">VM</span></span>

* <span data-ttu-id="8eafc-603">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-603">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="8eafc-604">O mesmo suporte pode ser acessado por meio de `vm update` ou `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="8eafc-604">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="8eafc-605">Imagem de extensão fixa correspondente em `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="8eafc-605">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="8eafc-606">`--boot-diagnostics-storage` foi adicionado a `vm create` para capturar o log de inicialização</span><span class="sxs-lookup"><span data-stu-id="8eafc-606">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="8eafc-607">`--license-type` foi adicionado a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-607">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="8eafc-608">7 de maio de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-608">May 7, 2018</span></span>

<span data-ttu-id="8eafc-609">Versão 2.0.32</span><span class="sxs-lookup"><span data-stu-id="8eafc-609">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-610">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-610">Core</span></span>

* <span data-ttu-id="8eafc-611">Foi corrigida uma exceção sem tratamento ao recuperar segredos de uma conta de entidade de serviço com certificado</span><span class="sxs-lookup"><span data-stu-id="8eafc-611">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="8eafc-612">Adicionado suporte limitado para argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="8eafc-612">Added limited support for positional arguments</span></span>
* <span data-ttu-id="8eafc-613">Corrigir problema no qual `--query` não pôde ser usado com `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-613">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="8eafc-614">#5591</span><span class="sxs-lookup"><span data-stu-id="8eafc-614">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="8eafc-615">Foram melhorados os cenários de redirecionamento de comandos ao usar `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-615">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="8eafc-616">Oferece suporte a `-o tsv` com uma consulta especificada ou `-o json` sem especificar uma consulta</span><span class="sxs-lookup"><span data-stu-id="8eafc-616">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="8eafc-617">Foram adicionadas sugestões de comando sobre o erro se os usuários cometeram algum erro de digitação em seus comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-617">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="8eafc-618">Erro corrigido quando os usuários digitam `az ''`</span><span class="sxs-lookup"><span data-stu-id="8eafc-618">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="8eafc-619">Foram adicionados tipos de recursos personalizados com suporte para módulos de comando e extensões</span><span class="sxs-lookup"><span data-stu-id="8eafc-619">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-620">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-620">ACR</span></span>

* <span data-ttu-id="8eafc-621">Foram adicionados comandos de compilação de ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-621">Added ACR Build commands</span></span>
* <span data-ttu-id="8eafc-622">O recurso aprimorado não encontrou mensagens de erro</span><span class="sxs-lookup"><span data-stu-id="8eafc-622">Improved resource not found error messages</span></span>
* <span data-ttu-id="8eafc-623">Desempenho de criação de recurso aprimorado e tratamento de erros</span><span class="sxs-lookup"><span data-stu-id="8eafc-623">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="8eafc-624">Logon de acr aprimorado em consoles não padrão e WSL</span><span class="sxs-lookup"><span data-stu-id="8eafc-624">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="8eafc-625">Mensagens de erro de comandos de repositório aprimoradas</span><span class="sxs-lookup"><span data-stu-id="8eafc-625">Improved repository commands error messages</span></span>
* <span data-ttu-id="8eafc-626">Colunas de tabela e ordenação atualizadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-626">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-627">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-627">ACS</span></span>

* <span data-ttu-id="8eafc-628">Foi adicionado um aviso informando que `az aks` é um serviço de versão prévia</span><span class="sxs-lookup"><span data-stu-id="8eafc-628">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="8eafc-629">Foi corrigido um problema de permissão em `aks install-connector` quando `--aci-resource-group` não for especificado</span><span class="sxs-lookup"><span data-stu-id="8eafc-629">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="8eafc-630">AMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-630">AMS</span></span>

* <span data-ttu-id="8eafc-631">Versão inicial — Gerenciar recursos dos Serviços de Mídia do Azure</span><span class="sxs-lookup"><span data-stu-id="8eafc-631">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-632">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-632">Appservice</span></span>

* <span data-ttu-id="8eafc-633">Correção de bug no `webapp delete` quando `--slot` é fornecido</span><span class="sxs-lookup"><span data-stu-id="8eafc-633">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="8eafc-634">`--runtime-version` foi removido de `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-634">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="8eafc-635">Foi adicionado suporte para min\_tls\_versão e https2.0</span><span class="sxs-lookup"><span data-stu-id="8eafc-635">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="8eafc-636">Suporte adicionado para vários contêineres</span><span class="sxs-lookup"><span data-stu-id="8eafc-636">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8eafc-637">Lote AI</span><span class="sxs-lookup"><span data-stu-id="8eafc-637">Batch AI</span></span>

* <span data-ttu-id="8eafc-638">O `batchai create cluster` foi alterado para respeitar a prioridade de VM configurada no arquivo de configuração do cluster</span><span class="sxs-lookup"><span data-stu-id="8eafc-638">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8eafc-639">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-639">Cognitive Services</span></span>

* <span data-ttu-id="8eafc-640">Foi corrigido um erro de digitação no exemplo para `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="8eafc-640">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="8eafc-641">Consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-641">Consumption</span></span>

* <span data-ttu-id="8eafc-642">Foram adicionados novos comandos para a API de orçamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-642">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-643">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-643">Container</span></span>

* <span data-ttu-id="8eafc-644">Requisito removido para `--registry-server` e `container create` quando um servidor de registro estiver incluído no nome da imagem</span><span class="sxs-lookup"><span data-stu-id="8eafc-644">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8eafc-645">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8eafc-645">Cosmos DB</span></span>

* <span data-ttu-id="8eafc-646">Introdução ao suporte de rede virtual para a CLI do Azure — Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8eafc-646">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="8eafc-647">DMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-647">DMS</span></span>

* <span data-ttu-id="8eafc-648">Versão inicial — Adiciona suporte ao SQL para o cenário de migração do SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="8eafc-648">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-649">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-649">Extension</span></span>

* <span data-ttu-id="8eafc-650">Correção do bug em que os metadados de extensão pararam de ser exibidos</span><span class="sxs-lookup"><span data-stu-id="8eafc-650">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-651">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-651">Interactive</span></span>

* <span data-ttu-id="8eafc-652">Permitir que complementos interativos funcionem com argumentos posicionais</span><span class="sxs-lookup"><span data-stu-id="8eafc-652">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="8eafc-653">Resultado mais simplificado quando os usuários digitam '\'</span><span class="sxs-lookup"><span data-stu-id="8eafc-653">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="8eafc-654">Conclusões corrigidas para parâmetros sem ajuda</span><span class="sxs-lookup"><span data-stu-id="8eafc-654">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="8eafc-655">Descrições corrigidas para grupos de comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-655">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="8eafc-656">Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-656">Lab</span></span>

* <span data-ttu-id="8eafc-657">Regressões corrigidas de conversão de aptidão</span><span class="sxs-lookup"><span data-stu-id="8eafc-657">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-658">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-658">Network</span></span>

* <span data-ttu-id="8eafc-659">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--ids` removido de:</span><span class="sxs-lookup"><span data-stu-id="8eafc-659">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="8eafc-660">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-660">Profile</span></span>

* <span data-ttu-id="8eafc-661">Detecção de origem do `disk create` corrigida</span><span class="sxs-lookup"><span data-stu-id="8eafc-661">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="8eafc-662">[ALTERAÇÃO SIGNIFICATIVA] `--msi-port` e `--identity-port` removidos porque não são mais usados</span><span class="sxs-lookup"><span data-stu-id="8eafc-662">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="8eafc-663">Erro de digitação corrigido no resumo do `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="8eafc-663">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="8eafc-664">Redis</span><span class="sxs-lookup"><span data-stu-id="8eafc-664">Redis</span></span>

* <span data-ttu-id="8eafc-665">`redis patch-schedule patch-schedule show` preterido em favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-665">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="8eafc-666">`redis list-all` preterido.</span><span class="sxs-lookup"><span data-stu-id="8eafc-666">Deprecated `redis list-all`.</span></span> <span data-ttu-id="8eafc-667">Esta funcionalidade foi dobrada em `redis list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-667">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="8eafc-668">`redis import-method` preterido em favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="8eafc-668">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="8eafc-669">Foi adicionado suporte a `--ids` para vários comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-669">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-670">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-670">Role</span></span>

* <span data-ttu-id="8eafc-671">[ALTERAÇÃO SIGNIFICATIVA] Remoção de `ad sp reset-credentials` preterido</span><span class="sxs-lookup"><span data-stu-id="8eafc-671">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-672">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-672">Storage</span></span>

* <span data-ttu-id="8eafc-673">Permitir que o token SAS de destino aplique na origem a cópia do blob se a SAS de origem e a chave de conta não forem especificadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-673">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="8eafc-674">Exposto -- tempo limite do soquete para carregamentos e downloads de blobs</span><span class="sxs-lookup"><span data-stu-id="8eafc-674">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="8eafc-675">Tratar os nomes de blobs que começam com separadores de caminho como caminhos relativos</span><span class="sxs-lookup"><span data-stu-id="8eafc-675">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="8eafc-676">Permitir `storage blob copy --source-sas` com a inicialização char de consulta, '?'</span><span class="sxs-lookup"><span data-stu-id="8eafc-676">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="8eafc-677">`storage entity query --marker` foi corrigido para aceitar a lista de chaves = valores</span><span class="sxs-lookup"><span data-stu-id="8eafc-677">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-678">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-678">VM</span></span>

* <span data-ttu-id="8eafc-679">Uma lógica de detecção inválida foi corrigida no URI do blob não gerenciado</span><span class="sxs-lookup"><span data-stu-id="8eafc-679">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="8eafc-680">Adicionada criptografia de disco de suporte sem entidades de serviço fornecidas pelo usuário</span><span class="sxs-lookup"><span data-stu-id="8eafc-680">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="8eafc-681">[ALTERAÇÃO SIGNIFICATIVA] Não usar a VM 'ManagedIdentityExtension' para suporte de MSI</span><span class="sxs-lookup"><span data-stu-id="8eafc-681">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="8eafc-682">Suporte adicionado para a política de remoção em `vmss`</span><span class="sxs-lookup"><span data-stu-id="8eafc-682">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="8eafc-683">[ALTERAÇÃO SIGNIFICATIVA] Removeu `--ids` de:</span><span class="sxs-lookup"><span data-stu-id="8eafc-683">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="8eafc-684">Foi adicionado suporte do acelerador de gravação</span><span class="sxs-lookup"><span data-stu-id="8eafc-684">Added write accelerator support</span></span>
* <span data-ttu-id="8eafc-685">Adicionado `vmss perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8eafc-685">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="8eafc-686">`vm diagnostics set` foi corrigido para detectar o tipo de sistema operacional da VM de forma confiável</span><span class="sxs-lookup"><span data-stu-id="8eafc-686">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="8eafc-687">`vm resize` foi alterado para verificar se o tamanho solicitado é diferente daquele definido no momento e atualizar somente na alteração</span><span class="sxs-lookup"><span data-stu-id="8eafc-687">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="8eafc-688">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-688">April 10, 2018</span></span>

<span data-ttu-id="8eafc-689">Versão 2.0.31</span><span class="sxs-lookup"><span data-stu-id="8eafc-689">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-690">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-690">ACR</span></span>

* <span data-ttu-id="8eafc-691">Melhoria do tratamento de erros do fallback do wincred</span><span class="sxs-lookup"><span data-stu-id="8eafc-691">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-692">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-692">ACS</span></span>

* <span data-ttu-id="8eafc-693">Alteração da validade de SPNs criados pelo AKS para 5 anos</span><span class="sxs-lookup"><span data-stu-id="8eafc-693">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-694">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-694">Appservice</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="8eafc-696">Correção da exceção não identificada de planos de webapp inexistentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-696">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="8eafc-697">BatchAI</span><span class="sxs-lookup"><span data-stu-id="8eafc-697">BatchAI</span></span>

* <span data-ttu-id="8eafc-698">Adição de suporte para a API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="8eafc-698">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="8eafc-699">Montagem de nível de trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-699">Job level mounting</span></span>
 - <span data-ttu-id="8eafc-700">Variáveis de ambiente com valores secretos</span><span class="sxs-lookup"><span data-stu-id="8eafc-700">Environment variables with secret values</span></span>
 - <span data-ttu-id="8eafc-701">Configurações de contadores de desempenho</span><span class="sxs-lookup"><span data-stu-id="8eafc-701">Performance counters settings</span></span>
 - <span data-ttu-id="8eafc-702">Relatório de segmento de linha específico de trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-702">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="8eafc-703">Suporte para subpastas na API de arquivos de lista</span><span class="sxs-lookup"><span data-stu-id="8eafc-703">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="8eafc-704">Relatório de uso e limites</span><span class="sxs-lookup"><span data-stu-id="8eafc-704">Usage and limits reporting</span></span>
 - <span data-ttu-id="8eafc-705">Permitir a especificação do tipo de cache para servidores NFS</span><span class="sxs-lookup"><span data-stu-id="8eafc-705">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="8eafc-706">Suporte para imagens personalizadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-706">Support for custom images</span></span>
 - <span data-ttu-id="8eafc-707">Adição de suporte para o kit de ferramentas pyTorch</span><span class="sxs-lookup"><span data-stu-id="8eafc-707">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="8eafc-708">Adição do comando `job wait`, que permite aguardar a conclusão do trabalho e relata o código de saída de trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-708">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="8eafc-709">Adição do comando `usage show` para listar o uso e os limites do IA do Lote atual para diferentes regiões</span><span class="sxs-lookup"><span data-stu-id="8eafc-709">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="8eafc-710">Há suporte para nuvens nacionais</span><span class="sxs-lookup"><span data-stu-id="8eafc-710">National clouds are supported</span></span>
* <span data-ttu-id="8eafc-711">Adição de argumentos de linha de comando do trabalho para montar sistemas de arquivos no nível de trabalho, além de arquivos de configuração</span><span class="sxs-lookup"><span data-stu-id="8eafc-711">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="8eafc-712">Adição de mais opções para personalizar clusters — prioridade de VM, sub-rede, contagem inicial de nós para clusters de dimensionamento automático, especificando a imagem personalizada</span><span class="sxs-lookup"><span data-stu-id="8eafc-712">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="8eafc-713">Adição de opção de linha de comando para especificar o tipo de cache de NFS gerenciado por IA do Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-713">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="8eafc-714">Simplificação da especificação do sistema de arquivos de montagem nos arquivos de configuração.</span><span class="sxs-lookup"><span data-stu-id="8eafc-714">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="8eafc-715">Agora é possível omitir as credenciais do Compartilhamento de arquivos do Azure e Contêineres de Blob do Azure — a CLI preencherá credenciais ausentes usando a chave da conta de armazenamento fornecida por meio dos parâmetros de linha de comando ou especificada por meio da variável de ambiente ou consultará a chave a partir do Armazenamento do Azure (se a conta de armazenamento pertencer à assinatura atual)</span><span class="sxs-lookup"><span data-stu-id="8eafc-715">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="8eafc-716">O comando do fluxo de arquivo de trabalho agora é preenchido automaticamente quando o trabalho é concluído (com êxito, com falha, encerrado ou excluído)</span><span class="sxs-lookup"><span data-stu-id="8eafc-716">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="8eafc-717">Melhoria da saída de `table` para operações de `show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-717">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="8eafc-718">Adição da opção `--use-auto-storage` para a criação de cluster.</span><span class="sxs-lookup"><span data-stu-id="8eafc-718">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="8eafc-719">Essa opção simplifica o gerenciamento de contas de armazenamento e a montagem do Compartilhamento de arquivos do Azure e dos Contêineres de Blob do Azure para clusters</span><span class="sxs-lookup"><span data-stu-id="8eafc-719">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="8eafc-720">Adição da opção `--generate-ssh-keys` para `cluster create` e `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-720">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="8eafc-721">Adição da capacidade de fornecer a tarefa de configuração de nó por meio da linha de comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-721">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="8eafc-722">[ALTERAÇÃO SIGNIFICATIVA] Comandos `job stream-file` e `job list-files` movidos para o grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="8eafc-722">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="8eafc-723">[ALTERAÇÃO SIGNIFICATIVA] `--admin-user-name` renomeado para `--user-name` no comando `file-server create` para ser consistente com o comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-723">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="8eafc-724">Cobrança</span><span class="sxs-lookup"><span data-stu-id="8eafc-724">Billing</span></span>

* <span data-ttu-id="8eafc-725">Adição de comandos da conta de registro</span><span class="sxs-lookup"><span data-stu-id="8eafc-725">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="8eafc-726">Consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-726">Consumption</span></span>

* <span data-ttu-id="8eafc-727">Adicionados os comandos `marketplace`</span><span class="sxs-lookup"><span data-stu-id="8eafc-727">Added `marketplace` commands</span></span>
* <span data-ttu-id="8eafc-728">[ALTERAÇÃO SIGNIFICATIVA] `reservations summaries` renomeado para `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="8eafc-728">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="8eafc-729">[ALTERAÇÃO SIGNIFICATIVA] `reservations details` renomeado para `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="8eafc-729">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="8eafc-730">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--reservation-order-id` e `--reservation-id` para os comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="8eafc-730">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="8eafc-731">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--grain` para os comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="8eafc-731">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="8eafc-732">[ALTERAÇÃO SIGNIFICATIVA] Removidas as opções abreviadas `--include-meter-details` para os comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="8eafc-732">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-733">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-733">Container</span></span>

* <span data-ttu-id="8eafc-734">Adição dos parâmetros de montagem de volume de repositório git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` e `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="8eafc-734">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="8eafc-735">Correção de [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` com falha com --container-name especificado</span><span class="sxs-lookup"><span data-stu-id="8eafc-735">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-736">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-736">Extension</span></span>

* <span data-ttu-id="8eafc-737">Alteração da mensagem de verificação de distribuição para ser de nível de depuração</span><span class="sxs-lookup"><span data-stu-id="8eafc-737">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-738">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-738">Interactive</span></span>

* <span data-ttu-id="8eafc-739">Alteração para interromper as conclusões após comandos não reconhecidos</span><span class="sxs-lookup"><span data-stu-id="8eafc-739">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="8eafc-740">Adição de ganchos de eventos antes e depois da criação da subárvore do comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-740">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="8eafc-741">Adição de conclusão para parâmetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="8eafc-741">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-742">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-742">Network</span></span>

* <span data-ttu-id="8eafc-743">Correção de [#5936](https://github.com/Azure/azure-cli/issues/5936): as marcas `application-gateway create` não podiam ser definidas</span><span class="sxs-lookup"><span data-stu-id="8eafc-743">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="8eafc-744">Adição do argumento `--auth-certs` para anexar certificados de autenticação para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-744">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="8eafc-745">#4910</span><span class="sxs-lookup"><span data-stu-id="8eafc-745">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="8eafc-746">Adição dos comandos `ddos-protection` para criar planos de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="8eafc-746">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="8eafc-747">Adição de suporte de `--ddos-protection-plan` a `vnet [create|update]` para associar uma VNET a um plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="8eafc-747">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="8eafc-748">Correção do problema com o sinalizador `--disable-bgp-route-propagation` em `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-748">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="8eafc-749">Remoção de argumentos fictícios `--public-ip-address-type` e `--subnet-type` para `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-749">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="8eafc-750">Adição de suporte para registros TXT com sequências de escape RFC 1035 para `network dns zone [import|export]` e `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="8eafc-750">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-751">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-751">Profile</span></span>

* <span data-ttu-id="8eafc-752">Adição de suporte para contas clássicas do Azure em `account list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-752">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="8eafc-753">[ALTERAÇÃO SIGNIFICATIVA] Remoção dos argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="8eafc-753">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-754">RDBMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-754">RDBMS</span></span>

* <span data-ttu-id="8eafc-755">Adicionado o comando `georestore`</span><span class="sxs-lookup"><span data-stu-id="8eafc-755">Added `georestore` command</span></span>
* <span data-ttu-id="8eafc-756">Remoção da restrição de tamanho de armazenamento do comando `create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-756">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-757">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-757">Resource</span></span>

* <span data-ttu-id="8eafc-758">Adicionado o suporte ao `--metadata` para `policy definition create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-758">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="8eafc-759">Adição de suporte para `--metadata`, `--set`, `--add`, `--remove` para `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-759">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-760">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-760">SQL</span></span>

* <span data-ttu-id="8eafc-761">Adição de `sql elastic-pool op list` e `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="8eafc-761">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-762">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-762">Storage</span></span>

* <span data-ttu-id="8eafc-763">Melhoria de mensagens de erro para cadeias de conexão malformadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-763">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-764">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-764">VM</span></span>

* <span data-ttu-id="8eafc-765">Adição de suporte para configurar a contagem de domínios de falha da plataforma para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-765">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="8eafc-766">Alteração de `vmss create` para balanceador de carga padrão para um conjunto de dimensionamento desabilitado zonal, grande ou de único grupo de posicionamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-766">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [ALTERAÇÃO SIGNIFICATIVA]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="8eafc-768">Adição de suporte para a SKU de IP público para `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-768">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="8eafc-769">Adição dos argumentos `--keyvault` e `--resource-group` para `vm secret format` para oferecer suporte a cenários em que o comando não é capaz de resolver a ID do cofre.</span><span class="sxs-lookup"><span data-stu-id="8eafc-769">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="8eafc-770">#5718</span><span class="sxs-lookup"><span data-stu-id="8eafc-770">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="8eafc-771">Melhoria de erros de `[vm|vmss create]` quando um local do grupo de recursos não tem suporte de zona</span><span class="sxs-lookup"><span data-stu-id="8eafc-771">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="8eafc-772">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-772">March 27, 2018</span></span>

<span data-ttu-id="8eafc-773">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="8eafc-773">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-774">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-774">Core</span></span>

* <span data-ttu-id="8eafc-775">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="8eafc-775">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-776">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-776">ACS</span></span>

* <span data-ttu-id="8eafc-777">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8eafc-777">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-778">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-778">Appservice</span></span>

* <span data-ttu-id="8eafc-779">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-779">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="8eafc-780">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-780">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8eafc-781">Backup</span><span class="sxs-lookup"><span data-stu-id="8eafc-781">Backup</span></span>

* <span data-ttu-id="8eafc-782">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-782">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="8eafc-783">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-783">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="8eafc-784">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="8eafc-784">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="8eafc-785">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-785">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-786">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-786">Container</span></span>

* <span data-ttu-id="8eafc-787">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-787">Added `container exec` command.</span></span> <span data-ttu-id="8eafc-788">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="8eafc-788">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="8eafc-789">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-789">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-790">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-790">Extension</span></span>

* <span data-ttu-id="8eafc-791">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="8eafc-791">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="8eafc-792">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="8eafc-792">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="8eafc-793">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-793">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-794">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-794">Interactive</span></span>

* <span data-ttu-id="8eafc-795">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-795">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="8eafc-796">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="8eafc-796">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="8eafc-797">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-797">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="8eafc-798">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="8eafc-798">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="8eafc-799">Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-799">Lab</span></span>

* <span data-ttu-id="8eafc-800">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="8eafc-800">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-801">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-801">Monitor</span></span>

* <span data-ttu-id="8eafc-802">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="8eafc-802">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="8eafc-803">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="8eafc-803">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="8eafc-804">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="8eafc-804">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-805">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-805">Network</span></span>

* <span data-ttu-id="8eafc-806">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="8eafc-806">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-807">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-807">Profile</span></span>

* <span data-ttu-id="8eafc-808">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="8eafc-808">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-809">RDBMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-809">RDBMS</span></span>

* <span data-ttu-id="8eafc-810">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="8eafc-810">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-811">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-811">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="8eafc-813">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-813">Role</span></span>

* <span data-ttu-id="8eafc-814">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-814">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="8eafc-815">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="8eafc-815">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="8eafc-816">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-816">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="8eafc-817">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-817">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="8eafc-818">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="8eafc-818">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-819">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-819">Storage</span></span>

* <span data-ttu-id="8eafc-820">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="8eafc-820">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="8eafc-821">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="8eafc-821">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-822">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-822">VM</span></span>

* <span data-ttu-id="8eafc-823">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="8eafc-823">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="8eafc-824">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-824">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="8eafc-825">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="8eafc-825">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="8eafc-826">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="8eafc-826">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="8eafc-827">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-827">March 13, 2018</span></span>

<span data-ttu-id="8eafc-828">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="8eafc-828">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-829">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-829">ACR</span></span>

* <span data-ttu-id="8eafc-830">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="8eafc-830">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="8eafc-831">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="8eafc-831">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="8eafc-832">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="8eafc-832">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-833">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-833">ACS</span></span>

* <span data-ttu-id="8eafc-834">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="8eafc-834">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="8eafc-835">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="8eafc-835">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="8eafc-836">Supervisor</span><span class="sxs-lookup"><span data-stu-id="8eafc-836">Advisor</span></span>

* <span data-ttu-id="8eafc-837">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-837">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="8eafc-838">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-838">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="8eafc-839">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="8eafc-839">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="8eafc-840">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-840">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="8eafc-841">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-841">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-842">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-842">Appservice</span></span>

* <span data-ttu-id="8eafc-843">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-843">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="8eafc-844">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-844">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="8eafc-845">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="8eafc-845">Eventhubs</span></span>

* <span data-ttu-id="8eafc-846">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-846">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-847">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-847">Extension</span></span>

* <span data-ttu-id="8eafc-848">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="8eafc-848">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-849">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-849">Interactive</span></span>

* <span data-ttu-id="8eafc-850">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-850">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="8eafc-851">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="8eafc-851">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="8eafc-852">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="8eafc-852">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="8eafc-853">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="8eafc-853">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-854">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-854">Monitor</span></span>

* <span data-ttu-id="8eafc-855">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-855">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="8eafc-856">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="8eafc-856">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="8eafc-857">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="8eafc-857">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="8eafc-858">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="8eafc-858">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-859">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-859">Network</span></span>

* <span data-ttu-id="8eafc-860">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-860">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="8eafc-861">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="8eafc-861">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="8eafc-862">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-862">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="8eafc-863">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="8eafc-863">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-864">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-864">Profile</span></span>

* <span data-ttu-id="8eafc-865">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="8eafc-865">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="8eafc-866">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="8eafc-866">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-867">RDBMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-867">RDBMS</span></span>

* <span data-ttu-id="8eafc-868">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="8eafc-868">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="8eafc-869">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-869">Service Bus</span></span>

* <span data-ttu-id="8eafc-870">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-870">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-871">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-871">Storage</span></span>

* <span data-ttu-id="8eafc-872">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="8eafc-872">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="8eafc-873">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="8eafc-873">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-874">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-874">VM</span></span>

* <span data-ttu-id="8eafc-875">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="8eafc-875">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="8eafc-876">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-876">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="8eafc-877">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="8eafc-877">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="8eafc-878">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="8eafc-878">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="8eafc-879">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-879">February 27, 2018</span></span>

<span data-ttu-id="8eafc-880">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="8eafc-880">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-881">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-881">Core</span></span>

* <span data-ttu-id="8eafc-882">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="8eafc-882">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="8eafc-883">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="8eafc-883">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="8eafc-884">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="8eafc-884">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-885">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-885">ACS</span></span>

* <span data-ttu-id="8eafc-886">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-886">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="8eafc-887">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="8eafc-887">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="8eafc-888">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="8eafc-888">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="8eafc-889">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="8eafc-889">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-890">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-890">Appservice</span></span>

* <span data-ttu-id="8eafc-891">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="8eafc-891">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="8eafc-892">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="8eafc-892">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8eafc-893">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-893">Cognitive Services</span></span>

* <span data-ttu-id="8eafc-894">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-894">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="8eafc-895">Consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-895">Consumption</span></span>

* <span data-ttu-id="8eafc-896">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="8eafc-896">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="8eafc-897">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="8eafc-897">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-898">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-898">Container</span></span>

* <span data-ttu-id="8eafc-899">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="8eafc-899">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-900">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-900">Network</span></span>

* <span data-ttu-id="8eafc-901">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="8eafc-901">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-902">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-902">Resource</span></span>

* <span data-ttu-id="8eafc-903">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="8eafc-903">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-904">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-904">Role</span></span>

* <span data-ttu-id="8eafc-905">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-905">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-906">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-906">SQL</span></span>

* <span data-ttu-id="8eafc-907">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="8eafc-907">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-908">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-908">Storage</span></span>

* <span data-ttu-id="8eafc-909">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-909">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-910">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-910">VM</span></span>

* <span data-ttu-id="8eafc-911">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="8eafc-911">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="8eafc-912">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-912">February 13, 2018</span></span>

<span data-ttu-id="8eafc-913">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="8eafc-913">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-914">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-914">Core</span></span>

* <span data-ttu-id="8eafc-915">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="8eafc-915">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-916">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-916">ACS</span></span>

* <span data-ttu-id="8eafc-917">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="8eafc-917">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="8eafc-918">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-918">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="8eafc-919">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="8eafc-919">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="8eafc-920">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-920">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="8eafc-921">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="8eafc-921">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="8eafc-922">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="8eafc-922">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="8eafc-923">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="8eafc-923">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="8eafc-924">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="8eafc-924">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-925">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-925">Appservice</span></span>

* <span data-ttu-id="8eafc-926">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="8eafc-926">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="8eafc-927">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="8eafc-927">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="8eafc-928">CDN</span><span class="sxs-lookup"><span data-stu-id="8eafc-928">CDN</span></span>

* <span data-ttu-id="8eafc-929">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-929">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-930">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-930">Container</span></span>

* <span data-ttu-id="8eafc-931">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="8eafc-931">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="8eafc-932">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-932">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8eafc-933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-933">CosmosDB</span></span>

* <span data-ttu-id="8eafc-934">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="8eafc-934">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-935">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-935">Extension</span></span>

* <span data-ttu-id="8eafc-936">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-936">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="8eafc-937">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-937">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="8eafc-938">Comentários</span><span class="sxs-lookup"><span data-stu-id="8eafc-938">Feedback</span></span>

* <span data-ttu-id="8eafc-939">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="8eafc-939">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-940">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-940">Interactive</span></span>

* <span data-ttu-id="8eafc-941">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="8eafc-941">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="8eafc-942">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-942">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-943">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-943">IoT</span></span>

* <span data-ttu-id="8eafc-944">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="8eafc-944">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8eafc-945">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="8eafc-945">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8eafc-946">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-946">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="8eafc-947">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="8eafc-947">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-948">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-948">Monitor</span></span>

* <span data-ttu-id="8eafc-949">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-949">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-950">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-950">Network</span></span>

* <span data-ttu-id="8eafc-951">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="8eafc-951">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="8eafc-952">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-952">Profile</span></span>

* <span data-ttu-id="8eafc-953">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-953">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-954">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-954">Resource</span></span>

* <span data-ttu-id="8eafc-955">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-955">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-956">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-956">Role</span></span>

* <span data-ttu-id="8eafc-957">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-957">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-958">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-958">SQL</span></span>

* <span data-ttu-id="8eafc-959">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="8eafc-959">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="8eafc-960">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="8eafc-960">Added `sql db rename`</span></span>
* <span data-ttu-id="8eafc-961">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="8eafc-961">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-962">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-962">Storage</span></span>

* <span data-ttu-id="8eafc-963">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="8eafc-963">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-964">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-964">VM</span></span>

* <span data-ttu-id="8eafc-965">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="8eafc-965">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="8eafc-966">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="8eafc-966">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="8eafc-967">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="8eafc-967">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="8eafc-968">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-968">January 31, 2018</span></span>

<span data-ttu-id="8eafc-969">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="8eafc-969">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-970">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-970">Core</span></span>

* <span data-ttu-id="8eafc-971">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="8eafc-971">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="8eafc-972">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="8eafc-972">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="8eafc-973">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="8eafc-973">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="8eafc-974">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="8eafc-974">Use `--verbose` to see</span></span>
* <span data-ttu-id="8eafc-975">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="8eafc-975">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-976">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-976">ACS</span></span>

* <span data-ttu-id="8eafc-977">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="8eafc-977">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="8eafc-978">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="8eafc-978">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-979">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-979">Appservice</span></span>

* <span data-ttu-id="8eafc-980">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="8eafc-980">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="8eafc-981">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="8eafc-981">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="8eafc-982">CDN</span><span class="sxs-lookup"><span data-stu-id="8eafc-982">CDN</span></span>

* <span data-ttu-id="8eafc-983">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-983">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8eafc-984">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-984">CosmosDB</span></span>

* <span data-ttu-id="8eafc-985">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="8eafc-985">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-986">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-986">Interactive</span></span>

* <span data-ttu-id="8eafc-987">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="8eafc-987">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-988">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-988">Network</span></span>

* <span data-ttu-id="8eafc-989">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-989">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="8eafc-990">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="8eafc-990">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="8eafc-991">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-991">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="8eafc-992">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-992">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="8eafc-993">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="8eafc-993">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="8eafc-994">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="8eafc-994">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="8eafc-995">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-995">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="8eafc-996">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="8eafc-996">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="8eafc-997">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="8eafc-997">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="8eafc-998">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="8eafc-998">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-999">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-999">Profile</span></span>

* <span data-ttu-id="8eafc-1000">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="8eafc-1000">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1001">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1001">Resource</span></span>

* <span data-ttu-id="8eafc-1002">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1002">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1003">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1003">Storage</span></span>

* <span data-ttu-id="8eafc-1004">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="8eafc-1004">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="8eafc-1005">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="8eafc-1005">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="8eafc-1006">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1006">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="8eafc-1007">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1007">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="8eafc-1008">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="8eafc-1008">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1009">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1009">VM</span></span>

* <span data-ttu-id="8eafc-1010">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="8eafc-1010">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="8eafc-1011">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1011">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="8eafc-1012">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1012">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="8eafc-1013">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1013">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="8eafc-1014">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="8eafc-1014">January 17, 2018</span></span>

<span data-ttu-id="8eafc-1015">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="8eafc-1015">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-1016">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1016">ACR</span></span>

* <span data-ttu-id="8eafc-1017">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="8eafc-1017">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="8eafc-1018">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="8eafc-1018">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1019">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1019">ACS</span></span>

* <span data-ttu-id="8eafc-1020">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1020">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="8eafc-1021">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1021">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1022">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1022">Appservice</span></span>

* <span data-ttu-id="8eafc-1023">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1023">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="8eafc-1024">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1024">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="8eafc-1025">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1025">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="8eafc-1026">Backup</span><span class="sxs-lookup"><span data-stu-id="8eafc-1026">Backup</span></span>

* <span data-ttu-id="8eafc-1027">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="8eafc-1027">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="8eafc-1028">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1028">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="8eafc-1029">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1029">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="8eafc-1030">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="8eafc-1030">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="8eafc-1031">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1031">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-1032">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1032">Batch</span></span>

* <span data-ttu-id="8eafc-1033">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="8eafc-1033">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="8eafc-1034">Nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1034">Cloud</span></span>

* <span data-ttu-id="8eafc-1035">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1035">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="8eafc-1036">Consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1036">Consumption</span></span>

* <span data-ttu-id="8eafc-1037">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1037">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="8eafc-1038">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1038">Event Grid</span></span>

* <span data-ttu-id="8eafc-1039">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1039">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8eafc-1040">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1040">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8eafc-1041">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1041">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="8eafc-1042">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1042">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="8eafc-1043">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1043">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="8eafc-1044">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1044">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="8eafc-1045">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1045">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="8eafc-1046">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1046">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-1047">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1047">Interactive</span></span>

* <span data-ttu-id="8eafc-1048">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="8eafc-1048">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="8eafc-1049">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="8eafc-1049">Fixed errors on startup</span></span>
* <span data-ttu-id="8eafc-1050">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1050">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-1051">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-1051">IoT</span></span>

* <span data-ttu-id="8eafc-1052">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1052">Added support for device provisioning service</span></span>
* <span data-ttu-id="8eafc-1053">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-1053">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="8eafc-1054">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-1054">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1055">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1055">Monitor</span></span>

* <span data-ttu-id="8eafc-1056">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1056">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="8eafc-1057">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1057">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="8eafc-1058">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1058">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1059">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1059">Network</span></span>

* <span data-ttu-id="8eafc-1060">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1060">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="8eafc-1061">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1061">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-1062">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-1062">Profile</span></span>

* <span data-ttu-id="8eafc-1063">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="8eafc-1063">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-1064">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-1064">Role</span></span>

* <span data-ttu-id="8eafc-1065">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1065">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8eafc-1066">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8eafc-1066">Service Fabric</span></span>

* <span data-ttu-id="8eafc-1067">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="8eafc-1067">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="8eafc-1068">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1068">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1069">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1069">VM</span></span>

* <span data-ttu-id="8eafc-1070">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1070">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="8eafc-1071">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="8eafc-1071">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="8eafc-1072">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="8eafc-1072">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="8eafc-1073">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="8eafc-1073">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="8eafc-1074">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1074">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="8eafc-1075">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1075">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8eafc-1076">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1076">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="8eafc-1077">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1077">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="8eafc-1078">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1078">December 19, 2017</span></span>

<span data-ttu-id="8eafc-1079">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="8eafc-1079">Version 2.0.23</span></span>

* <span data-ttu-id="8eafc-1080">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="8eafc-1080">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-1081">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1081">Container</span></span>

* <span data-ttu-id="8eafc-1082">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1082">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1083">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1083">Network</span></span>

* <span data-ttu-id="8eafc-1084">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1084">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="8eafc-1085">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1085">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1086">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1086">Storage</span></span>

* <span data-ttu-id="8eafc-1087">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="8eafc-1087">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1088">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1088">VM</span></span>

* <span data-ttu-id="8eafc-1089">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1089">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="8eafc-1090">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1090">December 5, 2017</span></span>

<span data-ttu-id="8eafc-1091">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="8eafc-1091">Version 2.0.22</span></span>

* <span data-ttu-id="8eafc-1092">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1092">Removed `az component` commands.</span></span> <span data-ttu-id="8eafc-1093">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1093">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-1094">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1094">Core</span></span>
* <span data-ttu-id="8eafc-1095">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="8eafc-1095">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="8eafc-1096">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1096">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1097">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1097">ACS</span></span>

* <span data-ttu-id="8eafc-1098">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1098">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="8eafc-1099">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1099">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="8eafc-1100">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1100">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="8eafc-1101">Supervisor</span><span class="sxs-lookup"><span data-stu-id="8eafc-1101">Advisor</span></span>

* <span data-ttu-id="8eafc-1102">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-1102">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1103">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1103">Appservice</span></span>

* <span data-ttu-id="8eafc-1104">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1104">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="8eafc-1105">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1105">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="8eafc-1106">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1106">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="8eafc-1107">Consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1107">Consumption</span></span>

* <span data-ttu-id="8eafc-1108">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1108">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-1109">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1109">Container</span></span>

* <span data-ttu-id="8eafc-1110">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1110">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1111">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1111">Monitor</span></span>

* <span data-ttu-id="8eafc-1112">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1112">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1113">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1113">Resource</span></span>

* <span data-ttu-id="8eafc-1114">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1114">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-1115">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-1115">Role</span></span>

* <span data-ttu-id="8eafc-1116">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1116">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="8eafc-1117">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="8eafc-1117">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="8eafc-1118">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1118">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1119">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1119">SQL</span></span>

* <span data-ttu-id="8eafc-1120">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1120">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="8eafc-1121">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1121">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1122">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1122">VM</span></span>

* <span data-ttu-id="8eafc-1123">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1123">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="8eafc-1124">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1124">November 14, 2017</span></span>

<span data-ttu-id="8eafc-1125">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="8eafc-1125">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-1126">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1126">ACR</span></span>

* <span data-ttu-id="8eafc-1127">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="8eafc-1127">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="8eafc-1128">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1128">ACS</span></span>

* <span data-ttu-id="8eafc-1129">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1129">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="8eafc-1130">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1130">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="8eafc-1131">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1131">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="8eafc-1132">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="8eafc-1132">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="8eafc-1133">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="8eafc-1133">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1134">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1134">Appservice</span></span>

* <span data-ttu-id="8eafc-1135">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="8eafc-1135">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="8eafc-1136">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1136">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="8eafc-1137">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1137">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="8eafc-1138">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1138">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="8eafc-1139">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="8eafc-1139">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="8eafc-1140">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1140">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-1141">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1141">Batch</span></span>

* <span data-ttu-id="8eafc-1142">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1142">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="8eafc-1143">Batchai</span><span class="sxs-lookup"><span data-stu-id="8eafc-1143">Batchai</span></span>

* <span data-ttu-id="8eafc-1144">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1144">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="8eafc-1145">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1145">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="8eafc-1146">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1146">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="8eafc-1147">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1147">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="8eafc-1148">Nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1148">Cloud</span></span>

* <span data-ttu-id="8eafc-1149">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="8eafc-1149">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-1150">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1150">Container</span></span>

* <span data-ttu-id="8eafc-1151">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1151">Added support to open multiple ports</span></span>
* <span data-ttu-id="8eafc-1152">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1152">Added container group restart policy</span></span>
* <span data-ttu-id="8eafc-1153">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="8eafc-1153">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="8eafc-1154">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1154">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8eafc-1155">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8eafc-1155">Data Lake Analytics</span></span>

* <span data-ttu-id="8eafc-1156">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1156">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8eafc-1157">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1157">Data Lake Store</span></span>

* <span data-ttu-id="8eafc-1158">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1158">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-1159">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1159">Extension</span></span>

* <span data-ttu-id="8eafc-1160">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8eafc-1160">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="8eafc-1161">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="8eafc-1161">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-1162">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-1162">IoT</span></span>

* <span data-ttu-id="8eafc-1163">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1163">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1164">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1164">Monitor</span></span>

* <span data-ttu-id="8eafc-1165">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1165">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1166">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1166">Network</span></span>

* <span data-ttu-id="8eafc-1167">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="8eafc-1167">Added support for CAA DNS records</span></span>
* <span data-ttu-id="8eafc-1168">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1168">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="8eafc-1169">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1169">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="8eafc-1170">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1170">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="8eafc-1171">Reservas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1171">Reservations</span></span>

* <span data-ttu-id="8eafc-1172">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-1172">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1173">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1173">Resource</span></span>

* <span data-ttu-id="8eafc-1174">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1174">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1175">SQL</span></span>

* <span data-ttu-id="8eafc-1176">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1176">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1177">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1177">Storage</span></span>

* <span data-ttu-id="8eafc-1178">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1178">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="8eafc-1179">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="8eafc-1179">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="8eafc-1180">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1180">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="8eafc-1181">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1181">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="8eafc-1182">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1182">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="8eafc-1183">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1183">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="8eafc-1184">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1184">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1185">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1185">VM</span></span>

* <span data-ttu-id="8eafc-1186">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1186">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="8eafc-1187">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="8eafc-1187">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="8eafc-1188">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1188">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="8eafc-1189">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1189">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="8eafc-1190">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1190">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="8eafc-1191">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1191">October 24, 2017</span></span>

<span data-ttu-id="8eafc-1192">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="8eafc-1192">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-1193">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1193">Core</span></span>

* <span data-ttu-id="8eafc-1194">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1194">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1195">ACR</span></span>

* <span data-ttu-id="8eafc-1196">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1196">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="8eafc-1197">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1197">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="8eafc-1198">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="8eafc-1198">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1199">ACS</span></span>

* <span data-ttu-id="8eafc-1200">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1200">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="8eafc-1201">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="8eafc-1201">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1202">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1202">Appservice</span></span>

* <span data-ttu-id="8eafc-1203">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1203">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="8eafc-1204">Componente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1204">Component</span></span>

* <span data-ttu-id="8eafc-1205">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="8eafc-1205">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1206">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1206">Monitor</span></span>

* <span data-ttu-id="8eafc-1207">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1207">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1208">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1208">Resource</span></span>

* <span data-ttu-id="8eafc-1209">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1209">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="8eafc-1210">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1210">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1211">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1211">VM</span></span>

* <span data-ttu-id="8eafc-1212">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1212">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="8eafc-1213">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1213">October 9, 2017</span></span>

<span data-ttu-id="8eafc-1214">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="8eafc-1214">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-1215">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1215">Core</span></span>

* <span data-ttu-id="8eafc-1216">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8eafc-1216">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1217">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1217">Appservice</span></span>

* <span data-ttu-id="8eafc-1218">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1218">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-1219">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1219">Batch</span></span>

* <span data-ttu-id="8eafc-1220">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="8eafc-1220">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="8eafc-1221">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="8eafc-1221">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="8eafc-1222">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1222">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="8eafc-1223">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1223">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="8eafc-1224">Batchai</span><span class="sxs-lookup"><span data-stu-id="8eafc-1224">Batchai</span></span>

* <span data-ttu-id="8eafc-1225">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1225">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-1226">Keyvault</span><span class="sxs-lookup"><span data-stu-id="8eafc-1226">Keyvault</span></span>

* <span data-ttu-id="8eafc-1227">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1227">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="8eafc-1228">(#4448)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1228">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="8eafc-1229">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1229">Network</span></span>

* <span data-ttu-id="8eafc-1230">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="8eafc-1230">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="8eafc-1231">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1231">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1232">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1232">Resource</span></span>

* <span data-ttu-id="8eafc-1233">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1233">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="8eafc-1234">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-1234">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="8eafc-1235">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1235">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="8eafc-1236">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1236">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1237">Sql</span><span class="sxs-lookup"><span data-stu-id="8eafc-1237">Sql</span></span>

* <span data-ttu-id="8eafc-1238">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="8eafc-1238">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="8eafc-1239">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1239">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="8eafc-1240">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1240">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1241">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1241">Storage</span></span>

* <span data-ttu-id="8eafc-1242">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1242">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1243">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1243">Vm</span></span>

* <span data-ttu-id="8eafc-1244">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1244">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="8eafc-1245">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1245">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="8eafc-1246">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1246">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="8eafc-1247">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1247">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="8eafc-1248">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1248">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="8eafc-1249">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1249">September 22, 2017</span></span>

<span data-ttu-id="8eafc-1250">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="8eafc-1250">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1251">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1251">Resource</span></span>

* <span data-ttu-id="8eafc-1252">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1252">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="8eafc-1253">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="8eafc-1253">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="8eafc-1254">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1254">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="8eafc-1255">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1255">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1256">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1256">Network</span></span>

* <span data-ttu-id="8eafc-1257">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1257">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="8eafc-1258">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1258">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="8eafc-1259">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1259">Added `asg` application security group commands</span></span>
* <span data-ttu-id="8eafc-1260">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1260">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="8eafc-1261">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1261">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8eafc-1262">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1262">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="8eafc-1263">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1263">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1264">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1264">Storage</span></span>

* <span data-ttu-id="8eafc-1265">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="8eafc-1265">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8eafc-1266">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1266">Eventgrid</span></span>

* <span data-ttu-id="8eafc-1267">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="8eafc-1267">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1268">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1268">SQL</span></span>

* <span data-ttu-id="8eafc-1269">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1269">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="8eafc-1270">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1270">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="8eafc-1271">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1271">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-1272">Keyvault</span><span class="sxs-lookup"><span data-stu-id="8eafc-1272">Keyvault</span></span>

* <span data-ttu-id="8eafc-1273">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="8eafc-1273">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1274">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1274">VM</span></span>

* <span data-ttu-id="8eafc-1275">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1275">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="8eafc-1276">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="8eafc-1276">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="8eafc-1277">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1277">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="8eafc-1278">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1278">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="8eafc-1279">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1279">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="8eafc-1280">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1280">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1281">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1281">ACS</span></span>

* <span data-ttu-id="8eafc-1282">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1282">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1283">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1283">Appservice</span></span>

* <span data-ttu-id="8eafc-1284">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1284">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8eafc-1285">Backup</span><span class="sxs-lookup"><span data-stu-id="8eafc-1285">Backup</span></span>

* <span data-ttu-id="8eafc-1286">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="8eafc-1286">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="8eafc-1287">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1287">September 11, 2017</span></span>

<span data-ttu-id="8eafc-1288">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="8eafc-1288">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="8eafc-1289">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1289">Core</span></span>

* <span data-ttu-id="8eafc-1290">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="8eafc-1290">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="8eafc-1291">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1291">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1292">Acs</span><span class="sxs-lookup"><span data-stu-id="8eafc-1292">Acs</span></span>

* <span data-ttu-id="8eafc-1293">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1293">Added `acs list-locations` command</span></span>
* <span data-ttu-id="8eafc-1294">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1294">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1295">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1295">Appservice</span></span>

* <span data-ttu-id="8eafc-1296">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1296">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="8eafc-1297">CDN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1297">CDN</span></span>

* <span data-ttu-id="8eafc-1298">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1298">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="8eafc-1299">Extensão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1299">Extension</span></span>

* <span data-ttu-id="8eafc-1300">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-1300">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-1301">Keyvault</span><span class="sxs-lookup"><span data-stu-id="8eafc-1301">Keyvault</span></span>

* <span data-ttu-id="8eafc-1302">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1302">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1303">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1303">Network</span></span>

* <span data-ttu-id="8eafc-1304">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1304">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8eafc-1305">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1305">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="8eafc-1306">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1306">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="8eafc-1307">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1307">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8eafc-1308">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1308">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1309">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1309">Resource</span></span>

* <span data-ttu-id="8eafc-1310">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1310">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="8eafc-1311">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1311">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="8eafc-1312">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="8eafc-1312">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="8eafc-1313">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1313">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1314">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1314">SQL</span></span>

* <span data-ttu-id="8eafc-1315">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1315">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1316">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1316">VM</span></span>

* <span data-ttu-id="8eafc-1317">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="8eafc-1317">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="8eafc-1318">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="8eafc-1318">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="8eafc-1319">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1319">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="8eafc-1320">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1320">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="8eafc-1321">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="8eafc-1321">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="8eafc-1322">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1322">August 31, 2017</span></span>

<span data-ttu-id="8eafc-1323">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="8eafc-1323">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-1324">Keyvault</span><span class="sxs-lookup"><span data-stu-id="8eafc-1324">Keyvault</span></span>

* <span data-ttu-id="8eafc-1325">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1325">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="8eafc-1326">Sf</span><span class="sxs-lookup"><span data-stu-id="8eafc-1326">Sf</span></span>

* <span data-ttu-id="8eafc-1327">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1327">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1328">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1328">Storage</span></span>

* <span data-ttu-id="8eafc-1329">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="8eafc-1329">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="8eafc-1330">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1330">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="8eafc-1331">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1331">August 28, 2017</span></span>

<span data-ttu-id="8eafc-1332">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="8eafc-1332">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="8eafc-1333">CLI</span><span class="sxs-lookup"><span data-stu-id="8eafc-1333">CLI</span></span>

* <span data-ttu-id="8eafc-1334">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1334">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1335">ACS</span></span>

* <span data-ttu-id="8eafc-1336">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="8eafc-1336">Corrected preview regions</span></span>
* <span data-ttu-id="8eafc-1337">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1337">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="8eafc-1338">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1338">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1339">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1339">Appservice</span></span>

* <span data-ttu-id="8eafc-1340">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1340">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="8eafc-1341">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1341">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="8eafc-1342">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1342">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="8eafc-1343">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1343">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="8eafc-1344">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1344">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-1345">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-1345">IoT</span></span>

* <span data-ttu-id="8eafc-1346">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1346">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1347">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1347">Network</span></span>

* <span data-ttu-id="8eafc-1348">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1348">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8eafc-1349">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1349">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="8eafc-1350">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1350">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8eafc-1351">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1351">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8eafc-1352">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1352">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-1353">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-1353">Profile</span></span>

* <span data-ttu-id="8eafc-1354">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="8eafc-1354">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8eafc-1355">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8eafc-1355">Service Fabric</span></span>

* <span data-ttu-id="8eafc-1356">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="8eafc-1356">Preview release</span></span>
* <span data-ttu-id="8eafc-1357">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-1357">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="8eafc-1358">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="8eafc-1358">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="8eafc-1359">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="8eafc-1359">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1360">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1360">Storage</span></span>

* <span data-ttu-id="8eafc-1361">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="8eafc-1361">Enabled setting blob tier</span></span>
* <span data-ttu-id="8eafc-1362">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="8eafc-1362">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="8eafc-1363">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="8eafc-1363">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="8eafc-1364">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1364">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="8eafc-1365">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1365">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="8eafc-1366">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="8eafc-1366">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1367">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1367">VM</span></span>

* <span data-ttu-id="8eafc-1368">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1368">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="8eafc-1369">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1369">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="8eafc-1370">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1370">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="8eafc-1371">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1371">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="8eafc-1372">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="8eafc-1372">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="8eafc-1373">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1373">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="8eafc-1374">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1374">August 15, 2017</span></span>

<span data-ttu-id="8eafc-1375">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="8eafc-1375">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1376">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1376">ACS</span></span>

* <span data-ttu-id="8eafc-1377">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1377">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1378">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1378">Appservice</span></span>

* <span data-ttu-id="8eafc-1379">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="8eafc-1379">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="8eafc-1380">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1380">Event Grid</span></span>

* <span data-ttu-id="8eafc-1381">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="8eafc-1381">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="8eafc-1382">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1382">August 11, 2017</span></span>

<span data-ttu-id="8eafc-1383">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="8eafc-1383">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1384">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1384">ACS</span></span>

* <span data-ttu-id="8eafc-1385">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="8eafc-1385">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-1386">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1386">Batch</span></span>

* <span data-ttu-id="8eafc-1387">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="8eafc-1387">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="8eafc-1388">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-1388">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="8eafc-1389">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1389">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="8eafc-1390">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="8eafc-1390">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="8eafc-1391">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="8eafc-1391">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="8eafc-1392">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="8eafc-1392">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="8eafc-1393">Componente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1393">Component</span></span>

* <span data-ttu-id="8eafc-1394">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="8eafc-1394">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="8eafc-1395">Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1395">Container</span></span>

* <span data-ttu-id="8eafc-1396">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1396">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="8eafc-1397">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1397">Data Lake Store</span></span>

* <span data-ttu-id="8eafc-1398">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1398">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="8eafc-1399">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1399">Event Grid</span></span>

* <span data-ttu-id="8eafc-1400">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="8eafc-1400">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1401">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1401">Network</span></span>

* <span data-ttu-id="8eafc-1402">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1402">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="8eafc-1403">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1403">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="8eafc-1404">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1404">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="8eafc-1405">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1405">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-1406">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-1406">Profile</span></span>

* <span data-ttu-id="8eafc-1407">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="8eafc-1407">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1408">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1408">Storage</span></span>

* <span data-ttu-id="8eafc-1409">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="8eafc-1409">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1410">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1410">VM</span></span>

* <span data-ttu-id="8eafc-1411">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1411">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="8eafc-1412">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1412">Exposed `list-skus` command</span></span>
* <span data-ttu-id="8eafc-1413">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="8eafc-1413">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="8eafc-1414">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1414">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="8eafc-1415">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1415">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="8eafc-1416">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1416">July 28, 2017</span></span>

<span data-ttu-id="8eafc-1417">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="8eafc-1417">Version 2.0.12</span></span>

* <span data-ttu-id="8eafc-1418">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1418">Added container commands</span></span>
* <span data-ttu-id="8eafc-1419">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1419">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="8eafc-1420">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1420">Core</span></span>

* <span data-ttu-id="8eafc-1421">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1421">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="8eafc-1422">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="8eafc-1422">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="8eafc-1423">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="8eafc-1423">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="8eafc-1424">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1424">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="8eafc-1425">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-1425">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="8eafc-1426">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1426">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="8eafc-1427">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1427">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8eafc-1428">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1428">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="8eafc-1429">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1429">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="8eafc-1430">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="8eafc-1430">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="8eafc-1431">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1431">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="8eafc-1432">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1432">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="8eafc-1433">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1433">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="8eafc-1434">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="8eafc-1434">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="8eafc-1435">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="8eafc-1435">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="8eafc-1436">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1436">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="8eafc-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1437">ACR</span></span>

* <span data-ttu-id="8eafc-1438">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1438">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="8eafc-1439">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1439">Support SKU update for managed registries</span></span>
* <span data-ttu-id="8eafc-1440">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1440">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="8eafc-1441">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1441">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="8eafc-1442">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1442">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="8eafc-1443">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="8eafc-1443">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1444">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1444">ACS</span></span>

* <span data-ttu-id="8eafc-1445">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="8eafc-1445">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1446">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1446">Appservice</span></span>

* <span data-ttu-id="8eafc-1447">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1447">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="8eafc-1448">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="8eafc-1448">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="8eafc-1449">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1449">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="8eafc-1450">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1450">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="8eafc-1451">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1451">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="8eafc-1452">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1452">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="8eafc-1453">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1453">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="8eafc-1454">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1454">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="8eafc-1455">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1455">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="8eafc-1456">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1456">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="8eafc-1457">Lote</span><span class="sxs-lookup"><span data-stu-id="8eafc-1457">Batch</span></span>

* <span data-ttu-id="8eafc-1458">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="8eafc-1458">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="8eafc-1459">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1459">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="8eafc-1460">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1460">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="8eafc-1461">CDN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1461">CDN</span></span>

* <span data-ttu-id="8eafc-1462">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="8eafc-1462">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="8eafc-1463">Nuvem</span><span class="sxs-lookup"><span data-stu-id="8eafc-1463">Cloud</span></span>

* <span data-ttu-id="8eafc-1464">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="8eafc-1464">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="8eafc-1465">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="8eafc-1465">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="8eafc-1466">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1466">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="8eafc-1467">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="8eafc-1467">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="8eafc-1468">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1468">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8eafc-1469">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1469">CosmosDB</span></span>

* <span data-ttu-id="8eafc-1470">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1470">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="8eafc-1471">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="8eafc-1471">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8eafc-1472">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8eafc-1472">Data Lake Analytics</span></span>

* <span data-ttu-id="8eafc-1473">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1473">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="8eafc-1474">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1474">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="8eafc-1475">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1475">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8eafc-1476">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1476">Data Lake Store</span></span>

* <span data-ttu-id="8eafc-1477">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1477">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="8eafc-1478">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="8eafc-1478">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="8eafc-1479">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1479">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="8eafc-1480">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1480">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="8eafc-1481">Interativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1481">Interactive</span></span>

* <span data-ttu-id="8eafc-1482">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="8eafc-1482">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="8eafc-1483">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="8eafc-1483">Increased test coverage</span></span>
* <span data-ttu-id="8eafc-1484">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="8eafc-1484">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="8eafc-1485">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1485">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="8eafc-1486">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1486">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="8eafc-1487">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1487">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="8eafc-1488">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1488">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8eafc-1489">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1489">Added `--progress` flag</span></span>
* <span data-ttu-id="8eafc-1490">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="8eafc-1490">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="8eafc-1491">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1491">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="8eafc-1492">IoT</span><span class="sxs-lookup"><span data-stu-id="8eafc-1492">IoT</span></span>

* <span data-ttu-id="8eafc-1493">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1493">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="8eafc-1494">(#3934)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1494">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="8eafc-1495">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="8eafc-1495">Key vault</span></span>

* <span data-ttu-id="8eafc-1496">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1496">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="8eafc-1497">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1497">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="8eafc-1498">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1498">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8eafc-1499">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1499">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8eafc-1500">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1500">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="8eafc-1501">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1501">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="8eafc-1502">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1502">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="8eafc-1503">(#3307)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1503">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="8eafc-1504">Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1504">Lab</span></span>

* <span data-ttu-id="8eafc-1505">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1505">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="8eafc-1506">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1506">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1507">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1507">Monitor</span></span>

* <span data-ttu-id="8eafc-1508">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1508">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="8eafc-1509">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1509">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="8eafc-1510">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1510">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="8eafc-1511">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1511">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="8eafc-1512">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1512">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="8eafc-1513">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1513">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="8eafc-1514">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="8eafc-1514">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="8eafc-1515">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="8eafc-1515">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="8eafc-1516">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="8eafc-1516">`location` no longer required</span></span>
  * <span data-ttu-id="8eafc-1517">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="8eafc-1517">Add name and ID support for target</span></span>
  * <span data-ttu-id="8eafc-1518">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1518">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="8eafc-1519">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="8eafc-1519">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="8eafc-1520">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="8eafc-1520">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="8eafc-1521">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="8eafc-1521">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="8eafc-1522">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1522">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="8eafc-1523">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1523">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1524">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1524">Network</span></span>

* <span data-ttu-id="8eafc-1525">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1525">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="8eafc-1526">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1526">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="8eafc-1527">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="8eafc-1527">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="8eafc-1528">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="8eafc-1528">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="8eafc-1529">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1529">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="8eafc-1530">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1530">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="8eafc-1531">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1531">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="8eafc-1532">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1532">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="8eafc-1533">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1533">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="8eafc-1534">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1534">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="8eafc-1535">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1535">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="8eafc-1536">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1536">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="8eafc-1537">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1537">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="8eafc-1538">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1538">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="8eafc-1539">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1539">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="8eafc-1540">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1540">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="8eafc-1541">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1541">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="8eafc-1542">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1542">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="8eafc-1543">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1543">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="8eafc-1544">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1544">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="8eafc-1545">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1545">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="8eafc-1546">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1546">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="8eafc-1547">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1547">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="8eafc-1548">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="8eafc-1548">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="8eafc-1549">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="8eafc-1549">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="8eafc-1550">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="8eafc-1550">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="8eafc-1551">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="8eafc-1551">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-1552">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-1552">Profile</span></span>

* <span data-ttu-id="8eafc-1553">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1553">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="8eafc-1554">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="8eafc-1554">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="8eafc-1555">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1555">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="8eafc-1556">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="8eafc-1556">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="8eafc-1557">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1557">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="8eafc-1558">RDBMS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1558">RDBMS</span></span>

* <span data-ttu-id="8eafc-1559">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1559">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="8eafc-1560">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1560">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="8eafc-1561">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1561">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="8eafc-1562">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1562">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1563">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1563">Resource</span></span>

* <span data-ttu-id="8eafc-1564">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1564">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="8eafc-1565">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1565">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="8eafc-1566">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1566">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="8eafc-1567">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1567">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="8eafc-1568">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1568">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="8eafc-1569">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1569">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="8eafc-1570">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1570">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="8eafc-1571">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1571">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-1572">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-1572">Role</span></span>

* <span data-ttu-id="8eafc-1573">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1573">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="8eafc-1574">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1574">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="8eafc-1575">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1575">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="8eafc-1576">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1576">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="8eafc-1577">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1577">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8eafc-1578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8eafc-1578">Service Fabric</span></span>
* <span data-ttu-id="8eafc-1579">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1579">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="8eafc-1580">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1580">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="8eafc-1581">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1581">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1582">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1582">SQL</span></span>

* <span data-ttu-id="8eafc-1583">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1583">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="8eafc-1584">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1584">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="8eafc-1585">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1585">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1586">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1586">Storage</span></span>

* <span data-ttu-id="8eafc-1587">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1587">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="8eafc-1588">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="8eafc-1588">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="8eafc-1589">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1589">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="8eafc-1590">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1590">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="8eafc-1591">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1591">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="8eafc-1592">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1592">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1593">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1593">VM</span></span>

* <span data-ttu-id="8eafc-1594">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="8eafc-1594">Support configuring nsg</span></span>
* <span data-ttu-id="8eafc-1595">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1595">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="8eafc-1596">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="8eafc-1596">Support managed service identities</span></span>
* <span data-ttu-id="8eafc-1597">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1597">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="8eafc-1598">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="8eafc-1598">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="8eafc-1599">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1599">May 10, 2017</span></span>

<span data-ttu-id="8eafc-1600">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="8eafc-1600">Version 2.0.6</span></span>

* <span data-ttu-id="8eafc-1601">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1601">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="8eafc-1602">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1602">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="8eafc-1603">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1603">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="8eafc-1604">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1604">Include Cognitive Services module</span></span>
* <span data-ttu-id="8eafc-1605">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8eafc-1605">Include Service Fabric module</span></span>
* <span data-ttu-id="8eafc-1606">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1606">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="8eafc-1607">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1607">Add support for CDN commands</span></span>
* <span data-ttu-id="8eafc-1608">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="8eafc-1608">Remove Container module</span></span>
* <span data-ttu-id="8eafc-1609">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1609">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="8eafc-1610">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1610">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="8eafc-1611">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1611">Core</span></span>

* <span data-ttu-id="8eafc-1612">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="8eafc-1612">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="8eafc-1613">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1613">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="8eafc-1614">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1614">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="8eafc-1615">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1615">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="8eafc-1616">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1616">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="8eafc-1617">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1617">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="8eafc-1618">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1618">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="8eafc-1619">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1619">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="8eafc-1620">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1620">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="8eafc-1621">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="8eafc-1621">core: Improved performance</span></span>
* <span data-ttu-id="8eafc-1622">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="8eafc-1622">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="8eafc-1623">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="8eafc-1623">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1624">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1624">ACS</span></span>

* <span data-ttu-id="8eafc-1625">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eafc-1625">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="8eafc-1626">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="8eafc-1626">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="8eafc-1627">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="8eafc-1627">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="8eafc-1628">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1628">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1629">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1629">AppService</span></span>

* <span data-ttu-id="8eafc-1630">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1630">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="8eafc-1631">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1631">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="8eafc-1632">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1632">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="8eafc-1633">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="8eafc-1633">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="8eafc-1634">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1634">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="8eafc-1635">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1635">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="8eafc-1636">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="8eafc-1636">support slot swap with preview</span></span>
* <span data-ttu-id="8eafc-1637">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1637">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="8eafc-1638">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1638">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8eafc-1639">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1639">CosmosDB</span></span>

* <span data-ttu-id="8eafc-1640">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1640">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="8eafc-1641">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="8eafc-1641">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="8eafc-1642">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="8eafc-1642">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="8eafc-1643">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="8eafc-1643">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8eafc-1644">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8eafc-1644">Data Lake Analytics</span></span>

* <span data-ttu-id="8eafc-1645">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="8eafc-1645">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="8eafc-1646">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1646">Add support for new catalog item type: package.</span></span> <span data-ttu-id="8eafc-1647">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1647">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="8eafc-1648">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="8eafc-1648">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="8eafc-1649">Tabela</span><span class="sxs-lookup"><span data-stu-id="8eafc-1649">Table</span></span>
  * <span data-ttu-id="8eafc-1650">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="8eafc-1650">Table valued function</span></span>
  * <span data-ttu-id="8eafc-1651">Visualizar</span><span class="sxs-lookup"><span data-stu-id="8eafc-1651">View</span></span>
  * <span data-ttu-id="8eafc-1652">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1652">Table Statistics.</span></span> <span data-ttu-id="8eafc-1653">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="8eafc-1653">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8eafc-1654">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1654">Data Lake Store</span></span>

* <span data-ttu-id="8eafc-1655">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="8eafc-1655">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="8eafc-1656">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1656">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="8eafc-1657">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1657">missed help for access show.</span></span> <span data-ttu-id="8eafc-1658">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1658">adding it.</span></span> <span data-ttu-id="8eafc-1659">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="8eafc-1660">Localizar</span><span class="sxs-lookup"><span data-stu-id="8eafc-1660">Find</span></span>

* <span data-ttu-id="8eafc-1661">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="8eafc-1661">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="8eafc-1662">KeyVault</span><span class="sxs-lookup"><span data-stu-id="8eafc-1662">KeyVault</span></span>

* <span data-ttu-id="8eafc-1663">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="8eafc-1663">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="8eafc-1664">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="8eafc-1664">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="8eafc-1665">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="8eafc-1665">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="8eafc-1666">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1666">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="8eafc-1667">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1667">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="8eafc-1668">Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1668">Lab</span></span>

* <span data-ttu-id="8eafc-1669">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1669">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="8eafc-1670">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1670">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="8eafc-1671">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1671">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="8eafc-1672">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1672">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="8eafc-1673">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="8eafc-1673">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="8eafc-1674">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1674">Monitor</span></span>

* <span data-ttu-id="8eafc-1675">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1675">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="8eafc-1676">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1676">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="8eafc-1677">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1677">Network</span></span>

* <span data-ttu-id="8eafc-1678">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1678">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="8eafc-1679">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1679">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="8eafc-1680">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1680">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="8eafc-1681">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1681">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="8eafc-1682">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="8eafc-1682">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="8eafc-1683">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="8eafc-1683">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="8eafc-1684">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1684">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="8eafc-1685">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="8eafc-1685">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="8eafc-1686">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1686">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="8eafc-1687">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="8eafc-1687">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="8eafc-1688">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1688">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="8eafc-1689">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1689">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="8eafc-1690">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1690">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="8eafc-1691">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="8eafc-1691">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="8eafc-1692">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="8eafc-1692">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="8eafc-1693">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1693">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="8eafc-1694">Perfil</span><span class="sxs-lookup"><span data-stu-id="8eafc-1694">Profile</span></span>

* <span data-ttu-id="8eafc-1695">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1695">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="8eafc-1696">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1696">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="8eafc-1697">Redis</span><span class="sxs-lookup"><span data-stu-id="8eafc-1697">Redis</span></span>

* <span data-ttu-id="8eafc-1698">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="8eafc-1698">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="8eafc-1699">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="8eafc-1699">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="8eafc-1700">Recurso</span><span class="sxs-lookup"><span data-stu-id="8eafc-1700">Resource</span></span>

* <span data-ttu-id="8eafc-1701">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1701">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="8eafc-1702">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1702">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="8eafc-1703">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1703">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="8eafc-1704">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1704">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="8eafc-1705">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="8eafc-1706">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1706">Add docs for az lock update.</span></span> <span data-ttu-id="8eafc-1707">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="8eafc-1708">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1708">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="8eafc-1709">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="8eafc-1710">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1710">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="8eafc-1711">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="8eafc-1712">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1712">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="8eafc-1713">Função</span><span class="sxs-lookup"><span data-stu-id="8eafc-1713">Role</span></span>

* <span data-ttu-id="8eafc-1714">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1714">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="8eafc-1715">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1715">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="8eafc-1716">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1716">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="8eafc-1717">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="8eafc-1717">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="8eafc-1718">SQL</span><span class="sxs-lookup"><span data-stu-id="8eafc-1718">SQL</span></span>

* <span data-ttu-id="8eafc-1719">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="8eafc-1719">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="8eafc-1720">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1720">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="8eafc-1721">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1721">Storage</span></span>

* <span data-ttu-id="8eafc-1722">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1722">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="8eafc-1723">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="8eafc-1723">Add support for incremental blob copy</span></span>
* <span data-ttu-id="8eafc-1724">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="8eafc-1724">Add support for large block blob upload</span></span>
* <span data-ttu-id="8eafc-1725">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1725">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1726">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1726">VM</span></span>

* <span data-ttu-id="8eafc-1727">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="8eafc-1727">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="8eafc-1728">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1728">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="8eafc-1729">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="8eafc-1729">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="8eafc-1730">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="8eafc-1730">az vm/vmss disk</span></span>
  3. <span data-ttu-id="8eafc-1731">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="8eafc-1731">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="8eafc-1732">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="8eafc-1732">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="8eafc-1733">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1733">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="8eafc-1734">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1734">April 3, 2017</span></span>

<span data-ttu-id="8eafc-1735">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="8eafc-1735">Version 2.0.2</span></span>

<span data-ttu-id="8eafc-1736">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1736">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="8eafc-1737">Núcleo</span><span class="sxs-lookup"><span data-stu-id="8eafc-1737">Core</span></span>

* <span data-ttu-id="8eafc-1738">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1738">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="8eafc-1739">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1739">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="8eafc-1740">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1740">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="8eafc-1741">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1741">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8eafc-1742">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1742">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="8eafc-1743">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1743">Add prompting for missing template parameters.</span></span> <span data-ttu-id="8eafc-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="8eafc-1745">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="8eafc-1745">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="8eafc-1746">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="8eafc-1746">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="8eafc-1747">ACS</span><span class="sxs-lookup"><span data-stu-id="8eafc-1747">ACS</span></span>

* <span data-ttu-id="8eafc-1748">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1748">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="8eafc-1749">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1749">Add support for ssh key password prompting.</span></span> <span data-ttu-id="8eafc-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="8eafc-1751">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1751">Add support for windows clusters.</span></span> <span data-ttu-id="8eafc-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="8eafc-1753">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="8eafc-1753">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="8eafc-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="8eafc-1755">AppService</span><span class="sxs-lookup"><span data-stu-id="8eafc-1755">AppService</span></span>

* <span data-ttu-id="8eafc-1756">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1756">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="8eafc-1757">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1757">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="8eafc-1758">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1758">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="8eafc-1759">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1759">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="8eafc-1760">DataLake</span><span class="sxs-lookup"><span data-stu-id="8eafc-1760">DataLake</span></span>

* <span data-ttu-id="8eafc-1761">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8eafc-1761">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="8eafc-1762">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8eafc-1762">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="8eafc-1763">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="8eafc-1763">DocuemntDB</span></span>

* <span data-ttu-id="8eafc-1764">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1764">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="8eafc-1765">VM</span><span class="sxs-lookup"><span data-stu-id="8eafc-1765">VM</span></span>

* <span data-ttu-id="8eafc-1766">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1766">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="8eafc-1767">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1767">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="8eafc-1768">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1768">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="8eafc-1769">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1769">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8eafc-1770">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1770">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="8eafc-1771">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1771">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="8eafc-1772">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="8eafc-1772">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="8eafc-1773">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="8eafc-1773">February 27, 2017</span></span>

<span data-ttu-id="8eafc-1774">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8eafc-1774">Version 2.0.0</span></span>

<span data-ttu-id="8eafc-1775">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1775">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="8eafc-1776">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1776">Container Service (acs)</span></span>
- <span data-ttu-id="8eafc-1777">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1777">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="8eafc-1778">Rede</span><span class="sxs-lookup"><span data-stu-id="8eafc-1778">Networking</span></span>
- <span data-ttu-id="8eafc-1779">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="8eafc-1779">Storage</span></span>

<span data-ttu-id="8eafc-1780">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1780">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="8eafc-1781">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="8eafc-1781">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="8eafc-1782">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="8eafc-1782">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="8eafc-1783">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="8eafc-1783">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="8eafc-1784">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1784">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="8eafc-1785">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="8eafc-1785">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="8eafc-1786">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1786">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="8eafc-1787">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="8eafc-1787">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="8eafc-1788">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="8eafc-1788">Provide feedback from the command line with the `az feedback` command</span></span>

