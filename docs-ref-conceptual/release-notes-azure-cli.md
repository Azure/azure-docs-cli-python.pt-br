---
title: Notas de versão da CLI do Azure 2.0
description: Saiba mais sobre as últimas atualizações da CLI do Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 116fa95e51399b9b97c1b35c38445f30db7efc94
ms.sourcegitcommit: fefb5bb6a21cab30c44592c0577408a8d1a2ccc7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/17/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="f2621-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="f2621-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f2621-104">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="f2621-104">March 13, 2018</span></span>

<span data-ttu-id="f2621-105">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f2621-105">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f2621-106">ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-106">ACR</span></span>

* <span data-ttu-id="f2621-107">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f2621-107">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f2621-108">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="f2621-108">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f2621-109">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="f2621-109">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-110">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-110">ACS</span></span>

* <span data-ttu-id="f2621-111">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="f2621-111">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f2621-112">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="f2621-112">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f2621-113">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f2621-113">Advisor</span></span>

* <span data-ttu-id="f2621-114">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="f2621-114">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f2621-115">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="f2621-115">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f2621-116">[ALTERAÇÃO SIGNIFICATIVA] Removida `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="f2621-116">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="f2621-117">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="f2621-117">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f2621-118">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="f2621-118">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-119">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-119">Appservice</span></span>

* <span data-ttu-id="f2621-120">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="f2621-120">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f2621-121">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-121">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f2621-122">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="f2621-122">Eventhubs</span></span>

* <span data-ttu-id="f2621-123">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2621-123">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f2621-124">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2621-124">Extension</span></span>

* <span data-ttu-id="f2621-125">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="f2621-125">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f2621-126">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-126">Interactive</span></span>

* <span data-ttu-id="f2621-127">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="f2621-127">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f2621-128">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="f2621-128">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f2621-129">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="f2621-129">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f2621-130">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="f2621-130">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-131">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-131">Monitor</span></span>

* <span data-ttu-id="f2621-132">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="f2621-132">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f2621-133">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="f2621-133">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f2621-134">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="f2621-134">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f2621-135">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="f2621-135">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f2621-136">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-136">Network</span></span>

* <span data-ttu-id="f2621-137">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="f2621-137">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f2621-138">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f2621-138">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f2621-139">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-139">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f2621-140">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f2621-140">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-141">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-141">Profile</span></span>

* <span data-ttu-id="f2621-142">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="f2621-142">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f2621-143">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="f2621-143">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2621-144">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2621-144">RDBMS</span></span>

* <span data-ttu-id="f2621-145">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="f2621-145">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f2621-146">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="f2621-146">Service Bus</span></span>

* <span data-ttu-id="f2621-147">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2621-147">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-148">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-148">Storage</span></span>

* <span data-ttu-id="f2621-149">[4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure.</span><span class="sxs-lookup"><span data-stu-id="f2621-149">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds.</span></span>
* <span data-ttu-id="f2621-150">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="f2621-150">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-151">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-151">VM</span></span>

* <span data-ttu-id="f2621-152">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="f2621-152">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f2621-153">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="f2621-153">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f2621-154">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="f2621-154">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f2621-155">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="f2621-155">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f2621-156">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2621-156">February 27, 2018</span></span>

<span data-ttu-id="f2621-157">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f2621-157">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f2621-158">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-158">Core</span></span>

* <span data-ttu-id="f2621-159">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="f2621-159">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f2621-160">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="f2621-160">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f2621-161">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="f2621-161">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-162">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-162">ACS</span></span>

* <span data-ttu-id="f2621-163">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="f2621-163">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f2621-164">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="f2621-164">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f2621-165">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="f2621-165">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f2621-166">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="f2621-166">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-167">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-167">Appservice</span></span>

* <span data-ttu-id="f2621-168">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f2621-168">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f2621-169">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="f2621-169">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f2621-170">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2621-170">Cognitive Services</span></span>

* <span data-ttu-id="f2621-171">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="f2621-171">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f2621-172">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2621-172">Consumption</span></span>

* <span data-ttu-id="f2621-173">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="f2621-173">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f2621-174">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="f2621-174">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f2621-175">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-175">Container</span></span>

* <span data-ttu-id="f2621-176">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="f2621-176">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f2621-177">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-177">Network</span></span>

* <span data-ttu-id="f2621-178">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="f2621-178">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-179">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-179">Resource</span></span>

* <span data-ttu-id="f2621-180">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="f2621-180">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f2621-181">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-181">Role</span></span>

* <span data-ttu-id="f2621-182">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f2621-182">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-183">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-183">SQL</span></span>

* <span data-ttu-id="f2621-184">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="f2621-184">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-185">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-185">Storage</span></span>

* <span data-ttu-id="f2621-186">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="f2621-186">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-187">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-187">VM</span></span>

* <span data-ttu-id="f2621-188">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="f2621-188">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f2621-189">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2621-189">February 13, 2018</span></span>

<span data-ttu-id="f2621-190">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f2621-190">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f2621-191">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-191">Core</span></span>

* <span data-ttu-id="f2621-192">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="f2621-192">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-193">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-193">ACS</span></span>

* <span data-ttu-id="f2621-194">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="f2621-194">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f2621-195">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="f2621-195">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f2621-196">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2621-196">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f2621-197">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="f2621-197">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f2621-198">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="f2621-198">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f2621-199">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="f2621-199">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f2621-200">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2621-200">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f2621-201">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="f2621-201">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-202">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-202">Appservice</span></span>

* <span data-ttu-id="f2621-203">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="f2621-203">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f2621-204">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="f2621-204">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f2621-205">CDN</span><span class="sxs-lookup"><span data-stu-id="f2621-205">CDN</span></span>

* <span data-ttu-id="f2621-206">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="f2621-206">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f2621-207">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-207">Container</span></span>

* <span data-ttu-id="f2621-208">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="f2621-208">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f2621-209">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-209">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2621-210">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2621-210">CosmosDB</span></span>

* <span data-ttu-id="f2621-211">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="f2621-211">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f2621-212">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2621-212">Extension</span></span>

* <span data-ttu-id="f2621-213">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-213">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f2621-214">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-214">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f2621-215">Comentários</span><span class="sxs-lookup"><span data-stu-id="f2621-215">Feedback</span></span>

* <span data-ttu-id="f2621-216">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="f2621-216">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f2621-217">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-217">Interactive</span></span>

* <span data-ttu-id="f2621-218">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="f2621-218">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f2621-219">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="f2621-219">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f2621-220">IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-220">IoT</span></span>

* <span data-ttu-id="f2621-221">Corrigido o problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso.</span><span class="sxs-lookup"><span data-stu-id="f2621-221">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="f2621-222">Corrigido o problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso.</span><span class="sxs-lookup"><span data-stu-id="f2621-222">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="f2621-223">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-223">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f2621-224">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="f2621-224">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-225">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-225">Monitor</span></span>

* <span data-ttu-id="f2621-226">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="f2621-226">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f2621-227">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-227">Network</span></span>

* <span data-ttu-id="f2621-228">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="f2621-228">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f2621-229">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-229">Profile</span></span>

* <span data-ttu-id="f2621-230">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-230">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-231">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-231">Resource</span></span>

* <span data-ttu-id="f2621-232">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="f2621-232">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f2621-233">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-233">Role</span></span>

* <span data-ttu-id="f2621-234">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f2621-234">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-235">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-235">SQL</span></span>

* <span data-ttu-id="f2621-236">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="f2621-236">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f2621-237">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="f2621-237">Added `sql db rename`</span></span>
* <span data-ttu-id="f2621-238">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="f2621-238">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-239">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-239">Storage</span></span>

* <span data-ttu-id="f2621-240">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="f2621-240">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-241">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-241">VM</span></span>

* <span data-ttu-id="f2621-242">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="f2621-242">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f2621-243">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="f2621-243">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f2621-244">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="f2621-244">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f2621-245">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2621-245">January 31, 2018</span></span>

<span data-ttu-id="f2621-246">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f2621-246">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f2621-247">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-247">Core</span></span>

* <span data-ttu-id="f2621-248">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="f2621-248">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f2621-249">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="f2621-249">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f2621-250">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="f2621-250">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f2621-251">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="f2621-251">Use `--verbose` to see</span></span>
* <span data-ttu-id="f2621-252">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="f2621-252">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-253">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-253">ACS</span></span>

* <span data-ttu-id="f2621-254">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="f2621-254">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f2621-255">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="f2621-255">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-256">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-256">Appservice</span></span>

* <span data-ttu-id="f2621-257">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="f2621-257">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f2621-258">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="f2621-258">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f2621-259">CDN</span><span class="sxs-lookup"><span data-stu-id="f2621-259">CDN</span></span>

* <span data-ttu-id="f2621-260">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="f2621-260">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2621-261">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2621-261">CosmosDB</span></span>

* <span data-ttu-id="f2621-262">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="f2621-262">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f2621-263">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-263">Interactive</span></span>

* <span data-ttu-id="f2621-264">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="f2621-264">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f2621-265">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-265">Network</span></span>

* <span data-ttu-id="f2621-266">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="f2621-266">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f2621-267">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="f2621-267">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f2621-268">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f2621-268">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f2621-269">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="f2621-269">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f2621-270">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="f2621-270">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f2621-271">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="f2621-271">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f2621-272">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="f2621-272">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f2621-273">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="f2621-273">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f2621-274">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f2621-274">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="f2621-275">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="f2621-275">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-276">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-276">Profile</span></span>

* <span data-ttu-id="f2621-277">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="f2621-277">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-278">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-278">Resource</span></span>

* <span data-ttu-id="f2621-279">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="f2621-279">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-280">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-280">Storage</span></span>

* <span data-ttu-id="f2621-281">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f2621-281">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f2621-282">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="f2621-282">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f2621-283">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="f2621-283">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="f2621-284">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="f2621-284">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f2621-285">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="f2621-285">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-286">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-286">VM</span></span>

* <span data-ttu-id="f2621-287">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="f2621-287">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f2621-288">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="f2621-288">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f2621-289">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="f2621-289">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f2621-290">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-290">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f2621-291">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="f2621-291">January 17, 2018</span></span>

<span data-ttu-id="f2621-292">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f2621-292">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f2621-293">ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-293">ACR</span></span>

* <span data-ttu-id="f2621-294">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="f2621-294">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f2621-295">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="f2621-295">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-296">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-296">ACS</span></span>

* <span data-ttu-id="f2621-297">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f2621-297">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f2621-298">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="f2621-298">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-299">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-299">Appservice</span></span>

* <span data-ttu-id="f2621-300">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="f2621-300">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f2621-301">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="f2621-301">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f2621-302">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="f2621-302">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f2621-303">Backup</span><span class="sxs-lookup"><span data-stu-id="f2621-303">Backup</span></span>

* <span data-ttu-id="f2621-304">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="f2621-304">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f2621-305">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="f2621-305">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f2621-306">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2621-306">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f2621-307">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="f2621-307">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f2621-308">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="f2621-308">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f2621-309">Batch</span><span class="sxs-lookup"><span data-stu-id="f2621-309">Batch</span></span>

* <span data-ttu-id="f2621-310">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="f2621-310">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f2621-311">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2621-311">Cloud</span></span>

* <span data-ttu-id="f2621-312">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="f2621-312">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f2621-313">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2621-313">Consumption</span></span>

* <span data-ttu-id="f2621-314">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="f2621-314">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2621-315">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2621-315">Event Grid</span></span>

* <span data-ttu-id="f2621-316">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid topic event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f2621-316">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f2621-317">[ALTERAÇÃO SIGNIFICATIVA] Movidos os comandos `az eventgrid resource event-subscription` para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="f2621-317">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f2621-318">[ALTERAÇÃO SIGNIFICATIVA] Removido o comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f2621-318">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f2621-319">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="f2621-319">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f2621-320">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="f2621-320">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f2621-321">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="f2621-321">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f2621-322">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="f2621-322">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f2621-323">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="f2621-323">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f2621-324">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-324">Interactive</span></span>

* <span data-ttu-id="f2621-325">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="f2621-325">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f2621-326">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="f2621-326">Fixed errors on startup</span></span>
* <span data-ttu-id="f2621-327">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-327">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f2621-328">IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-328">IoT</span></span>

* <span data-ttu-id="f2621-329">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f2621-329">Added support for device provisioning service</span></span>
* <span data-ttu-id="f2621-330">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="f2621-330">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f2621-331">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-331">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-332">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-332">Monitor</span></span>

* <span data-ttu-id="f2621-333">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="f2621-333">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f2621-334">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="f2621-334">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f2621-335">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f2621-335">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f2621-336">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-336">Network</span></span>

* <span data-ttu-id="f2621-337">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="f2621-337">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f2621-338">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-338">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-339">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-339">Profile</span></span>

* <span data-ttu-id="f2621-340">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f2621-340">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f2621-341">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-341">Role</span></span>

* <span data-ttu-id="f2621-342">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="f2621-342">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2621-343">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2621-343">Service Fabric</span></span>

* <span data-ttu-id="f2621-344">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="f2621-344">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f2621-345">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="f2621-345">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-346">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-346">VM</span></span>

* <span data-ttu-id="f2621-347">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="f2621-347">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f2621-348">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="f2621-348">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f2621-349">[ALTERAÇÃO SIGNIFICATIVA] Alterado `externalIdentities` para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="f2621-349">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f2621-350">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f2621-350">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f2621-351">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="f2621-351">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f2621-352">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-352">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2621-353">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-353">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2621-354">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="f2621-354">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f2621-355">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-355">December 19, 2017</span></span>

<span data-ttu-id="f2621-356">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f2621-356">Version 2.0.23</span></span>

* <span data-ttu-id="f2621-357">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="f2621-357">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f2621-358">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-358">Container</span></span>

* <span data-ttu-id="f2621-359">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-359">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f2621-360">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-360">Network</span></span>

* <span data-ttu-id="f2621-361">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-361">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f2621-362">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-362">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-363">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-363">Storage</span></span>

* <span data-ttu-id="f2621-364">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="f2621-364">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-365">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-365">VM</span></span>

* <span data-ttu-id="f2621-366">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="f2621-366">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f2621-367">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-367">December 5, 2017</span></span>

<span data-ttu-id="f2621-368">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f2621-368">Version 2.0.22</span></span>

* <span data-ttu-id="f2621-369">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="f2621-369">Removed `az component` commands.</span></span> <span data-ttu-id="f2621-370">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="f2621-370">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f2621-371">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-371">Core</span></span>
* <span data-ttu-id="f2621-372">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="f2621-372">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f2621-373">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="f2621-373">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-374">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-374">ACS</span></span>

* <span data-ttu-id="f2621-375">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-375">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f2621-376">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f2621-376">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f2621-377">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="f2621-377">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f2621-378">Supervisor</span><span class="sxs-lookup"><span data-stu-id="f2621-378">Advisor</span></span>

* <span data-ttu-id="f2621-379">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2621-379">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-380">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-380">Appservice</span></span>

* <span data-ttu-id="f2621-381">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="f2621-381">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f2621-382">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="f2621-382">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f2621-383">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="f2621-383">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f2621-384">Consumo</span><span class="sxs-lookup"><span data-stu-id="f2621-384">Consumption</span></span>

* <span data-ttu-id="f2621-385">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="f2621-385">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f2621-386">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-386">Container</span></span>

* <span data-ttu-id="f2621-387">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="f2621-387">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-388">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-388">Monitor</span></span>

* <span data-ttu-id="f2621-389">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="f2621-389">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-390">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-390">Resource</span></span>

* <span data-ttu-id="f2621-391">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="f2621-391">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f2621-392">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-392">Role</span></span>

* <span data-ttu-id="f2621-393">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="f2621-393">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f2621-394">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="f2621-394">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f2621-395">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f2621-395">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-396">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-396">SQL</span></span>

* <span data-ttu-id="f2621-397">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-397">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f2621-398">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-398">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-399">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-399">VM</span></span>

* <span data-ttu-id="f2621-400">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="f2621-400">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f2621-401">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-401">November 14, 2017</span></span>

<span data-ttu-id="f2621-402">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f2621-402">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f2621-403">ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-403">ACR</span></span>

* <span data-ttu-id="f2621-404">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="f2621-404">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f2621-405">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-405">ACS</span></span>

* <span data-ttu-id="f2621-406">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="f2621-406">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f2621-407">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="f2621-407">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f2621-408">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="f2621-408">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f2621-409">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f2621-409">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f2621-410">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="f2621-410">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-411">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-411">Appservice</span></span>

* <span data-ttu-id="f2621-412">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="f2621-412">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f2621-413">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f2621-413">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f2621-414">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="f2621-414">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f2621-415">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="f2621-415">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f2621-416">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="f2621-416">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f2621-417">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="f2621-417">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f2621-418">Batch</span><span class="sxs-lookup"><span data-stu-id="f2621-418">Batch</span></span>

* <span data-ttu-id="f2621-419">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="f2621-419">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f2621-420">Batchai</span><span class="sxs-lookup"><span data-stu-id="f2621-420">Batchai</span></span>

* <span data-ttu-id="f2621-421">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="f2621-421">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f2621-422">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="f2621-422">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f2621-423">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="f2621-423">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f2621-424">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="f2621-424">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f2621-425">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2621-425">Cloud</span></span>

* <span data-ttu-id="f2621-426">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="f2621-426">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f2621-427">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-427">Container</span></span>

* <span data-ttu-id="f2621-428">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="f2621-428">Added support to open multiple ports</span></span>
* <span data-ttu-id="f2621-429">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="f2621-429">Added container group restart policy</span></span>
* <span data-ttu-id="f2621-430">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="f2621-430">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f2621-431">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="f2621-431">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2621-432">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2621-432">Data Lake Analytics</span></span>

* <span data-ttu-id="f2621-433">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f2621-433">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2621-434">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="f2621-434">Data Lake Store</span></span>

* <span data-ttu-id="f2621-435">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="f2621-435">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f2621-436">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2621-436">Extension</span></span>

* <span data-ttu-id="f2621-437">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="f2621-437">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f2621-438">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="f2621-438">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f2621-439">IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-439">IoT</span></span>

* <span data-ttu-id="f2621-440">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="f2621-440">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-441">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-441">Monitor</span></span>

* <span data-ttu-id="f2621-442">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="f2621-442">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f2621-443">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-443">Network</span></span>

* <span data-ttu-id="f2621-444">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="f2621-444">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f2621-445">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="f2621-445">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f2621-446">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="f2621-446">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f2621-447">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="f2621-447">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f2621-448">Reservas</span><span class="sxs-lookup"><span data-stu-id="f2621-448">Reservations</span></span>

* <span data-ttu-id="f2621-449">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="f2621-449">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-450">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-450">Resource</span></span>

* <span data-ttu-id="f2621-451">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-451">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-452">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-452">SQL</span></span>

* <span data-ttu-id="f2621-453">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-453">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-454">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-454">Storage</span></span>

* <span data-ttu-id="f2621-455">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="f2621-455">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f2621-456">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="f2621-456">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f2621-457">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="f2621-457">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f2621-458">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="f2621-458">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f2621-459">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="f2621-459">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f2621-460">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="f2621-460">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f2621-461">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-461">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-462">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-462">VM</span></span>

* <span data-ttu-id="f2621-463">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="f2621-463">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f2621-464">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="f2621-464">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f2621-465">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-465">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f2621-466">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="f2621-466">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f2621-467">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f2621-467">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f2621-468">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-468">October 24, 2017</span></span>

<span data-ttu-id="f2621-469">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f2621-469">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f2621-470">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-470">Core</span></span>

* <span data-ttu-id="f2621-471">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f2621-471">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f2621-472">ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-472">ACR</span></span>

* <span data-ttu-id="f2621-473">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f2621-473">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f2621-474">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="f2621-474">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f2621-475">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="f2621-475">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-476">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-476">ACS</span></span>

* <span data-ttu-id="f2621-477">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="f2621-477">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f2621-478">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="f2621-478">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-479">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-479">Appservice</span></span>

* <span data-ttu-id="f2621-480">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="f2621-480">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f2621-481">Componente</span><span class="sxs-lookup"><span data-stu-id="f2621-481">Component</span></span>

* <span data-ttu-id="f2621-482">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="f2621-482">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-483">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-483">Monitor</span></span>

* <span data-ttu-id="f2621-484">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="f2621-484">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-485">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-485">Resource</span></span>

* <span data-ttu-id="f2621-486">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="f2621-486">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f2621-487">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="f2621-487">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-488">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-488">VM</span></span>

* <span data-ttu-id="f2621-489">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2621-489">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f2621-490">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-490">October 9, 2017</span></span>

<span data-ttu-id="f2621-491">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f2621-491">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f2621-492">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-492">Core</span></span>

* <span data-ttu-id="f2621-493">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f2621-493">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-494">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-494">Appservice</span></span>

* <span data-ttu-id="f2621-495">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="f2621-495">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f2621-496">Batch</span><span class="sxs-lookup"><span data-stu-id="f2621-496">Batch</span></span>

* <span data-ttu-id="f2621-497">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f2621-497">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f2621-498">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="f2621-498">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f2621-499">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="f2621-499">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f2621-500">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="f2621-500">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f2621-501">Batchai</span><span class="sxs-lookup"><span data-stu-id="f2621-501">Batchai</span></span>

* <span data-ttu-id="f2621-502">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="f2621-502">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2621-503">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2621-503">Keyvault</span></span>

* <span data-ttu-id="f2621-504">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f2621-504">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f2621-505">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f2621-505">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f2621-506">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-506">Network</span></span>

* <span data-ttu-id="f2621-507">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="f2621-507">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f2621-508">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="f2621-508">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-509">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-509">Resource</span></span>

* <span data-ttu-id="f2621-510">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="f2621-510">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f2621-511">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="f2621-511">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f2621-512">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="f2621-512">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f2621-513">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-513">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-514">Sql</span><span class="sxs-lookup"><span data-stu-id="f2621-514">Sql</span></span>

* <span data-ttu-id="f2621-515">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="f2621-515">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f2621-516">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="f2621-516">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f2621-517">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="f2621-517">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-518">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-518">Storage</span></span>

* <span data-ttu-id="f2621-519">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="f2621-519">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-520">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-520">Vm</span></span>

* <span data-ttu-id="f2621-521">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="f2621-521">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f2621-522">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2621-522">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f2621-523">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f2621-523">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f2621-524">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2621-524">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f2621-525">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f2621-525">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f2621-526">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-526">September 22, 2017</span></span>

<span data-ttu-id="f2621-527">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="f2621-527">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-528">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-528">Resource</span></span>

* <span data-ttu-id="f2621-529">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="f2621-529">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f2621-530">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="f2621-530">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f2621-531">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f2621-531">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f2621-532">[ALTERAÇÃO SIGNIFICATIVA] O tipo de recurso `managedapp` foi alterado de `appliances` para `applications` e `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="f2621-532">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f2621-533">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-533">Network</span></span>

* <span data-ttu-id="f2621-534">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f2621-534">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f2621-535">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="f2621-535">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f2621-536">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2621-536">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f2621-537">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-537">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f2621-538">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-538">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f2621-539">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-539">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f2621-540">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="f2621-540">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-541">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-541">Storage</span></span>

* <span data-ttu-id="f2621-542">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="f2621-542">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f2621-543">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="f2621-543">Eventgrid</span></span>

* <span data-ttu-id="f2621-544">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="f2621-544">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-545">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-545">SQL</span></span>

* <span data-ttu-id="f2621-546">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="f2621-546">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f2621-547">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="f2621-547">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f2621-548">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-548">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2621-549">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2621-549">Keyvault</span></span>

* <span data-ttu-id="f2621-550">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="f2621-550">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-551">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-551">VM</span></span>

* <span data-ttu-id="f2621-552">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-552">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f2621-553">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="f2621-553">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f2621-554">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="f2621-554">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f2621-555">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f2621-555">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f2621-556">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f2621-556">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f2621-557">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f2621-557">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-558">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-558">ACS</span></span>

* <span data-ttu-id="f2621-559">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-559">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-560">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-560">Appservice</span></span>

* <span data-ttu-id="f2621-561">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f2621-561">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f2621-562">Backup</span><span class="sxs-lookup"><span data-stu-id="f2621-562">Backup</span></span>

* <span data-ttu-id="f2621-563">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2621-563">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f2621-564">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-564">September 11, 2017</span></span>

<span data-ttu-id="f2621-565">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f2621-565">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f2621-566">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-566">Core</span></span>

* <span data-ttu-id="f2621-567">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="f2621-567">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f2621-568">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="f2621-568">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-569">Acs</span><span class="sxs-lookup"><span data-stu-id="f2621-569">Acs</span></span>

* <span data-ttu-id="f2621-570">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="f2621-570">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f2621-571">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="f2621-571">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-572">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-572">Appservice</span></span>

* <span data-ttu-id="f2621-573">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="f2621-573">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f2621-574">CDN</span><span class="sxs-lookup"><span data-stu-id="f2621-574">CDN</span></span>

* <span data-ttu-id="f2621-575">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="f2621-575">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="f2621-576">Extensão</span><span class="sxs-lookup"><span data-stu-id="f2621-576">Extension</span></span>

* <span data-ttu-id="f2621-577">Versão Inicial.</span><span class="sxs-lookup"><span data-stu-id="f2621-577">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2621-578">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2621-578">Keyvault</span></span>

* <span data-ttu-id="f2621-579">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="f2621-579">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="f2621-580">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-580">Network</span></span>

* <span data-ttu-id="f2621-581">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f2621-581">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f2621-582">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="f2621-582">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f2621-583">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="f2621-583">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f2621-584">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f2621-584">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f2621-585">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f2621-585">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-586">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-586">Resource</span></span>

* <span data-ttu-id="f2621-587">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="f2621-587">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f2621-588">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="f2621-588">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f2621-589">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="f2621-589">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f2621-590">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="f2621-590">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-591">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-591">SQL</span></span>

* <span data-ttu-id="f2621-592">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="f2621-592">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-593">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-593">VM</span></span>

* <span data-ttu-id="f2621-594">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="f2621-594">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f2621-595">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="f2621-595">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f2621-596">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-596">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f2621-597">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="f2621-597">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f2621-598">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="f2621-598">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f2621-599">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-599">August 31, 2017</span></span>

<span data-ttu-id="f2621-600">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f2621-600">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2621-601">Keyvault</span><span class="sxs-lookup"><span data-stu-id="f2621-601">Keyvault</span></span>

* <span data-ttu-id="f2621-602">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="f2621-602">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f2621-603">Sf</span><span class="sxs-lookup"><span data-stu-id="f2621-603">Sf</span></span>

* <span data-ttu-id="f2621-604">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="f2621-604">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-605">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-605">Storage</span></span>

* <span data-ttu-id="f2621-606">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="f2621-606">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f2621-607">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="f2621-607">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f2621-608">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-608">August 28, 2017</span></span>

<span data-ttu-id="f2621-609">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f2621-609">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f2621-610">CLI</span><span class="sxs-lookup"><span data-stu-id="f2621-610">CLI</span></span>

* <span data-ttu-id="f2621-611">Nota legal adicionada ao `--version`.</span><span class="sxs-lookup"><span data-stu-id="f2621-611">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-612">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-612">ACS</span></span>

* <span data-ttu-id="f2621-613">Corrigidas as regiões de visualização.</span><span class="sxs-lookup"><span data-stu-id="f2621-613">Corrected preview regions.</span></span>
* <span data-ttu-id="f2621-614">Corrigida a formatação padrão de `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="f2621-614">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="f2621-615">Saída de comando ACS otimizada.</span><span class="sxs-lookup"><span data-stu-id="f2621-615">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-616">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-616">Appservice</span></span>

* <span data-ttu-id="f2621-617">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="f2621-617">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f2621-618">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="f2621-618">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f2621-619">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="f2621-619">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f2621-620">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2621-620">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f2621-621">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="f2621-621">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f2621-622">IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-622">IoT</span></span>

* <span data-ttu-id="f2621-623">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="f2621-623">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f2621-624">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-624">Network</span></span>

* <span data-ttu-id="f2621-625">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="f2621-625">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f2621-626">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-626">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f2621-627">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f2621-627">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f2621-628">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="f2621-628">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f2621-629">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="f2621-629">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-630">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-630">Profile</span></span>

* <span data-ttu-id="f2621-631">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="f2621-631">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2621-632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2621-632">Service Fabric</span></span>

* <span data-ttu-id="f2621-633">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="f2621-633">Preview release</span></span>
* <span data-ttu-id="f2621-634">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="f2621-634">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f2621-635">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="f2621-635">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f2621-636">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="f2621-636">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-637">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-637">Storage</span></span>

* <span data-ttu-id="f2621-638">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="f2621-638">Enabled setting blob tier</span></span>
* <span data-ttu-id="f2621-639">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="f2621-639">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f2621-640">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="f2621-640">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f2621-641">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="f2621-641">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f2621-642">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="f2621-642">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f2621-643">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="f2621-643">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-644">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-644">VM</span></span>

* <span data-ttu-id="f2621-645">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="f2621-645">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f2621-646">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="f2621-646">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f2621-647">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="f2621-647">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f2621-648">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="f2621-648">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f2621-649">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="f2621-649">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f2621-650">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="f2621-650">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f2621-651">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-651">August 15, 2017</span></span>

<span data-ttu-id="f2621-652">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f2621-652">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-653">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-653">ACS</span></span>

* <span data-ttu-id="f2621-654">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="f2621-654">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-655">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-655">Appservice</span></span>

* <span data-ttu-id="f2621-656">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="f2621-656">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2621-657">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2621-657">Event Grid</span></span>

* <span data-ttu-id="f2621-658">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="f2621-658">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f2621-659">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-659">August 11, 2017</span></span>

<span data-ttu-id="f2621-660">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f2621-660">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-661">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-661">ACS</span></span>

* <span data-ttu-id="f2621-662">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="f2621-662">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f2621-663">Batch</span><span class="sxs-lookup"><span data-stu-id="f2621-663">Batch</span></span>

* <span data-ttu-id="f2621-664">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="f2621-664">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f2621-665">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="f2621-665">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f2621-666">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-666">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f2621-667">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="f2621-667">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f2621-668">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="f2621-668">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f2621-669">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="f2621-669">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f2621-670">Componente</span><span class="sxs-lookup"><span data-stu-id="f2621-670">Component</span></span>

* <span data-ttu-id="f2621-671">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="f2621-671">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f2621-672">Contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-672">Container</span></span>

* <span data-ttu-id="f2621-673">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="f2621-673">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f2621-674">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="f2621-674">Data Lake Store</span></span>

* <span data-ttu-id="f2621-675">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="f2621-675">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f2621-676">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="f2621-676">Event Grid</span></span>

* <span data-ttu-id="f2621-677">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="f2621-677">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f2621-678">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-678">Network</span></span>

* <span data-ttu-id="f2621-679">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="f2621-679">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f2621-680">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="f2621-680">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f2621-681">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="f2621-681">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f2621-682">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="f2621-682">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-683">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-683">Profile</span></span>

* <span data-ttu-id="f2621-684">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="f2621-684">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-685">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-685">Storage</span></span>

* <span data-ttu-id="f2621-686">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="f2621-686">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-687">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-687">VM</span></span>

* <span data-ttu-id="f2621-688">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="f2621-688">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f2621-689">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="f2621-689">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f2621-690">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="f2621-690">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f2621-691">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="f2621-691">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f2621-692">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2621-692">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f2621-693">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-693">July 28, 2017</span></span>

<span data-ttu-id="f2621-694">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f2621-694">Version 2.0.12</span></span>

* <span data-ttu-id="f2621-695">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="f2621-695">Added container commands</span></span>
* <span data-ttu-id="f2621-696">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="f2621-696">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f2621-697">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-697">Core</span></span>

* <span data-ttu-id="f2621-698">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="f2621-698">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f2621-699">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="f2621-699">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f2621-700">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="f2621-700">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f2621-701">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="f2621-701">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f2621-702">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="f2621-702">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f2621-703">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="f2621-703">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f2621-704">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f2621-704">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f2621-705">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="f2621-705">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f2621-706">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="f2621-706">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f2621-707">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="f2621-707">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f2621-708">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="f2621-708">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f2621-709">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="f2621-709">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f2621-710">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2621-710">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f2621-711">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="f2621-711">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f2621-712">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="f2621-712">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f2621-713">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="f2621-713">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f2621-714">ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-714">ACR</span></span>

* <span data-ttu-id="f2621-715">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2621-715">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f2621-716">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="f2621-716">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f2621-717">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="f2621-717">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f2621-718">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-718">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f2621-719">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-719">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f2621-720">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="f2621-720">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-721">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-721">ACS</span></span>

* <span data-ttu-id="f2621-722">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="f2621-722">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-723">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-723">Appservice</span></span>

* <span data-ttu-id="f2621-724">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="f2621-724">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f2621-725">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="f2621-725">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f2621-726">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="f2621-726">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f2621-727">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="f2621-727">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f2621-728">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="f2621-728">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f2621-729">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="f2621-729">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f2621-730">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="f2621-730">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f2621-731">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="f2621-731">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f2621-732">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="f2621-732">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f2621-733">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="f2621-733">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f2621-734">Batch</span><span class="sxs-lookup"><span data-stu-id="f2621-734">Batch</span></span>

* <span data-ttu-id="f2621-735">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="f2621-735">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f2621-736">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="f2621-736">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f2621-737">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="f2621-737">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f2621-738">CDN</span><span class="sxs-lookup"><span data-stu-id="f2621-738">CDN</span></span>

* <span data-ttu-id="f2621-739">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir.</span><span class="sxs-lookup"><span data-stu-id="f2621-739">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="f2621-740">Nuvem</span><span class="sxs-lookup"><span data-stu-id="f2621-740">Cloud</span></span>

* <span data-ttu-id="f2621-741">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="f2621-741">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f2621-742">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="f2621-742">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f2621-743">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="f2621-743">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f2621-744">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="f2621-744">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f2621-745">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="f2621-745">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2621-746">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2621-746">CosmosDB</span></span>

* <span data-ttu-id="f2621-747">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="f2621-747">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f2621-748">Adicionado suporte para o TTL padrão de coleção.</span><span class="sxs-lookup"><span data-stu-id="f2621-748">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2621-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2621-749">Data Lake Analytics</span></span>

* <span data-ttu-id="f2621-750">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="f2621-750">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f2621-751">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="f2621-751">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f2621-752">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="f2621-752">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2621-753">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="f2621-753">Data Lake Store</span></span>

* <span data-ttu-id="f2621-754">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="f2621-754">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f2621-755">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="f2621-755">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f2621-756">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f2621-756">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f2621-757">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f2621-757">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f2621-758">Interativo</span><span class="sxs-lookup"><span data-stu-id="f2621-758">Interactive</span></span>

* <span data-ttu-id="f2621-759">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="f2621-759">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f2621-760">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="f2621-760">Increased test coverage</span></span>
* <span data-ttu-id="f2621-761">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="f2621-761">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f2621-762">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="f2621-762">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f2621-763">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="f2621-763">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f2621-764">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="f2621-764">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f2621-765">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="f2621-765">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f2621-766">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="f2621-766">Added `--progress` flag</span></span>
* <span data-ttu-id="f2621-767">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="f2621-767">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f2621-768">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="f2621-768">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f2621-769">IoT</span><span class="sxs-lookup"><span data-stu-id="f2621-769">IoT</span></span>

* <span data-ttu-id="f2621-770">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="f2621-770">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f2621-771">(#3934)</span><span class="sxs-lookup"><span data-stu-id="f2621-771">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f2621-772">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="f2621-772">Key vault</span></span>

* <span data-ttu-id="f2621-773">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="f2621-773">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f2621-774">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="f2621-774">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f2621-775">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="f2621-775">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f2621-776">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="f2621-776">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f2621-777">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="f2621-777">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f2621-778">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="f2621-778">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f2621-779">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="f2621-779">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f2621-780">(#3307)</span><span class="sxs-lookup"><span data-stu-id="f2621-780">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f2621-781">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2621-781">Lab</span></span>

* <span data-ttu-id="f2621-782">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="f2621-782">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f2621-783">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="f2621-783">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-784">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-784">Monitor</span></span>

* <span data-ttu-id="f2621-785">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="f2621-785">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f2621-786">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="f2621-786">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f2621-787">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="f2621-787">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f2621-788">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="f2621-788">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f2621-789">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="f2621-789">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f2621-790">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="f2621-790">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f2621-791">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="f2621-791">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f2621-792">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="f2621-792">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f2621-793">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f2621-793">`location` no longer required</span></span>
  * <span data-ttu-id="f2621-794">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="f2621-794">Add name and ID support for target</span></span>
  * <span data-ttu-id="f2621-795">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="f2621-795">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f2621-796">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="f2621-796">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f2621-797">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="f2621-797">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f2621-798">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="f2621-798">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f2621-799">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="f2621-799">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f2621-800">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="f2621-800">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f2621-801">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-801">Network</span></span>

* <span data-ttu-id="f2621-802">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="f2621-802">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f2621-803">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="f2621-803">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f2621-804">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="f2621-804">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f2621-805">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="f2621-805">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f2621-806">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="f2621-806">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f2621-807">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f2621-807">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f2621-808">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="f2621-808">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f2621-809">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="f2621-809">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f2621-810">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="f2621-810">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f2621-811">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="f2621-811">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f2621-812">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="f2621-812">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f2621-813">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="f2621-813">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f2621-814">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="f2621-814">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f2621-815">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="f2621-815">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f2621-816">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="f2621-816">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f2621-817">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="f2621-817">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f2621-818">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="f2621-818">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f2621-819">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="f2621-819">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f2621-820">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="f2621-820">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f2621-821">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="f2621-821">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f2621-822">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="f2621-822">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f2621-823">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="f2621-823">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f2621-824">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="f2621-824">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f2621-825">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2621-825">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f2621-826">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2621-826">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f2621-827">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2621-827">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f2621-828">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="f2621-828">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-829">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-829">Profile</span></span>

* <span data-ttu-id="f2621-830">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="f2621-830">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f2621-831">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="f2621-831">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f2621-832">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="f2621-832">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f2621-833">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="f2621-833">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f2621-834">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="f2621-834">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f2621-835">RDBMS</span><span class="sxs-lookup"><span data-stu-id="f2621-835">RDBMS</span></span>

* <span data-ttu-id="f2621-836">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="f2621-836">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f2621-837">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="f2621-837">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f2621-838">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="f2621-838">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f2621-839">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="f2621-839">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-840">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-840">Resource</span></span>

* <span data-ttu-id="f2621-841">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="f2621-841">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f2621-842">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f2621-842">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f2621-843">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="f2621-843">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f2621-844">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="f2621-844">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f2621-845">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="f2621-845">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f2621-846">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="f2621-846">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f2621-847">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="f2621-847">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f2621-848">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="f2621-848">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f2621-849">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-849">Role</span></span>

* <span data-ttu-id="f2621-850">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="f2621-850">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f2621-851">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="f2621-851">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f2621-852">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="f2621-852">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f2621-853">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="f2621-853">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f2621-854">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="f2621-854">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f2621-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f2621-855">Service Fabric</span></span>
* <span data-ttu-id="f2621-856">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="f2621-856">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f2621-857">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="f2621-857">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f2621-858">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="f2621-858">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-859">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-859">SQL</span></span>

* <span data-ttu-id="f2621-860">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="f2621-860">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f2621-861">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="f2621-861">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f2621-862">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="f2621-862">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-863">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-863">Storage</span></span>

* <span data-ttu-id="f2621-864">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="f2621-864">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f2621-865">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="f2621-865">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f2621-866">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="f2621-866">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f2621-867">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="f2621-867">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f2621-868">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="f2621-868">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f2621-869">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="f2621-869">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-870">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-870">VM</span></span>

* <span data-ttu-id="f2621-871">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="f2621-871">Support configuring nsg</span></span>
* <span data-ttu-id="f2621-872">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="f2621-872">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f2621-873">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="f2621-873">Support managed service identities</span></span>
* <span data-ttu-id="f2621-874">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="f2621-874">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="f2621-875">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="f2621-875">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f2621-876">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-876">May 10, 2017</span></span>

<span data-ttu-id="f2621-877">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f2621-877">Version 2.0.6</span></span>

* <span data-ttu-id="f2621-878">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2621-878">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f2621-879">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="f2621-879">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f2621-880">Inclusão dos módulos Data Lake Analytics e Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f2621-880">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="f2621-881">Inclusão do módulo Serviços Cognitivos.</span><span class="sxs-lookup"><span data-stu-id="f2621-881">Include Cognitive Services module.</span></span>
* <span data-ttu-id="f2621-882">Inclusão do módulo Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="f2621-882">Include Service Fabric module.</span></span>
* <span data-ttu-id="f2621-883">Inclusão do módulo Interativo (renomeação de az-shell).</span><span class="sxs-lookup"><span data-stu-id="f2621-883">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="f2621-884">Adição de suporte para comandos CDN.</span><span class="sxs-lookup"><span data-stu-id="f2621-884">Add support for CDN commands.</span></span>
* <span data-ttu-id="f2621-885">Remoção do módulo Contêiner.</span><span class="sxs-lookup"><span data-stu-id="f2621-885">Remove Container module.</span></span>
* <span data-ttu-id="f2621-886">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="f2621-886">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f2621-887">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f2621-887">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f2621-888">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-888">Core</span></span>

* <span data-ttu-id="f2621-889">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="f2621-889">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f2621-890">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="f2621-890">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f2621-891">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="f2621-891">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f2621-892">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="f2621-892">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f2621-893">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="f2621-893">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f2621-894">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="f2621-894">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f2621-895">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="f2621-895">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f2621-896">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="f2621-896">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f2621-897">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="f2621-897">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f2621-898">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="f2621-898">core: Improved performance</span></span>
* <span data-ttu-id="f2621-899">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="f2621-899">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f2621-900">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="f2621-900">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-901">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-901">ACS</span></span>

* <span data-ttu-id="f2621-902">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f2621-902">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f2621-903">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="f2621-903">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f2621-904">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="f2621-904">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f2621-905">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="f2621-905">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-906">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-906">AppService</span></span>

* <span data-ttu-id="f2621-907">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="f2621-907">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f2621-908">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="f2621-908">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f2621-909">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="f2621-909">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f2621-910">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="f2621-910">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f2621-911">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="f2621-911">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f2621-912">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="f2621-912">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f2621-913">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="f2621-913">support slot swap with preview</span></span>
* <span data-ttu-id="f2621-914">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="f2621-914">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f2621-915">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="f2621-915">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f2621-916">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="f2621-916">CosmosDB</span></span>

* <span data-ttu-id="f2621-917">Renomeação do módulo DocumentDB para CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="f2621-917">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="f2621-918">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="f2621-918">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f2621-919">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="f2621-919">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f2621-920">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="f2621-920">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f2621-921">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f2621-921">Data Lake Analytics</span></span>

* <span data-ttu-id="f2621-922">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro.</span><span class="sxs-lookup"><span data-stu-id="f2621-922">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="f2621-923">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="f2621-923">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f2621-924">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="f2621-924">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f2621-925">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="f2621-925">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f2621-926">Tabela</span><span class="sxs-lookup"><span data-stu-id="f2621-926">Table</span></span>
  * <span data-ttu-id="f2621-927">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="f2621-927">Table valued function</span></span>
  * <span data-ttu-id="f2621-928">Visualizar</span><span class="sxs-lookup"><span data-stu-id="f2621-928">View</span></span>
  * <span data-ttu-id="f2621-929">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="f2621-929">Table Statistics.</span></span> <span data-ttu-id="f2621-930">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela.</span><span class="sxs-lookup"><span data-stu-id="f2621-930">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f2621-931">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="f2621-931">Data Lake Store</span></span>

* <span data-ttu-id="f2621-932">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="f2621-932">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="f2621-933">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="f2621-933">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f2621-934">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="f2621-934">missed help for access show.</span></span> <span data-ttu-id="f2621-935">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="f2621-935">adding it.</span></span> <span data-ttu-id="f2621-936">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f2621-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f2621-937">Localizar</span><span class="sxs-lookup"><span data-stu-id="f2621-937">Find</span></span>

* <span data-ttu-id="f2621-938">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="f2621-938">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f2621-939">KeyVault</span><span class="sxs-lookup"><span data-stu-id="f2621-939">KeyVault</span></span>

* <span data-ttu-id="f2621-940">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="f2621-940">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f2621-941">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço.</span><span class="sxs-lookup"><span data-stu-id="f2621-941">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="f2621-942">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="f2621-942">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f2621-943">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”.</span><span class="sxs-lookup"><span data-stu-id="f2621-943">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="f2621-944">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="f2621-944">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f2621-945">Laboratório</span><span class="sxs-lookup"><span data-stu-id="f2621-945">Lab</span></span>

* <span data-ttu-id="f2621-946">Adição dos comandos create, show, delete e list ao ambiente do laboratório.</span><span class="sxs-lookup"><span data-stu-id="f2621-946">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="f2621-947">Adição dos comandos show e list para exibir modelos ARM no laboratório.</span><span class="sxs-lookup"><span data-stu-id="f2621-947">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="f2621-948">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório.</span><span class="sxs-lookup"><span data-stu-id="f2621-948">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="f2621-949">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório.</span><span class="sxs-lookup"><span data-stu-id="f2621-949">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="f2621-950">Adição de comandos para gerenciar segredos em um Laboratório.</span><span class="sxs-lookup"><span data-stu-id="f2621-950">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="f2621-951">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="f2621-951">Monitor</span></span>

* <span data-ttu-id="f2621-952">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="f2621-952">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f2621-953">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="f2621-953">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f2621-954">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-954">Network</span></span>

* <span data-ttu-id="f2621-955">Adição do comando `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="f2621-955">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="f2621-956">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="f2621-956">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="f2621-957">Adição de suporte para drenagem de conexão do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2621-957">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="f2621-958">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2621-958">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="f2621-959">Adição de suporte para filtros de rota e regras do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="f2621-959">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="f2621-960">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego.</span><span class="sxs-lookup"><span data-stu-id="f2621-960">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="f2621-961">Adição de suporte para seletores de tráfego baseados em política da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f2621-961">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="f2621-962">Adição de suporte para políticas IPsec da conexão VPN.</span><span class="sxs-lookup"><span data-stu-id="f2621-962">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="f2621-963">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`.</span><span class="sxs-lookup"><span data-stu-id="f2621-963">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="f2621-964">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="f2621-964">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f2621-965">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="f2621-965">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="f2621-966">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="f2621-966">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f2621-967">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente.</span><span class="sxs-lookup"><span data-stu-id="f2621-967">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="f2621-968">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente.</span><span class="sxs-lookup"><span data-stu-id="f2621-968">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="f2621-969">Correção de um bug em que `traffic-manager endpoint update` não funciona.</span><span class="sxs-lookup"><span data-stu-id="f2621-969">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="f2621-970">Adição de comandos de visualização “network watcher”.</span><span class="sxs-lookup"><span data-stu-id="f2621-970">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="f2621-971">Perfil</span><span class="sxs-lookup"><span data-stu-id="f2621-971">Profile</span></span>

* <span data-ttu-id="f2621-972">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="f2621-972">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f2621-973">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="f2621-973">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f2621-974">Redis</span><span class="sxs-lookup"><span data-stu-id="f2621-974">Redis</span></span>

* <span data-ttu-id="f2621-975">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="f2621-975">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f2621-976">Preterição do comando “update-settings”.</span><span class="sxs-lookup"><span data-stu-id="f2621-976">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="f2621-977">Recurso</span><span class="sxs-lookup"><span data-stu-id="f2621-977">Resource</span></span>

* <span data-ttu-id="f2621-978">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="f2621-978">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f2621-979">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="f2621-979">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f2621-980">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="f2621-980">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f2621-981">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="f2621-981">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f2621-982">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f2621-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f2621-983">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="f2621-983">Add docs for az lock update.</span></span> <span data-ttu-id="f2621-984">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f2621-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f2621-985">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="f2621-985">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f2621-986">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f2621-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f2621-987">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="f2621-987">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f2621-988">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f2621-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f2621-989">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="f2621-989">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f2621-990">Função</span><span class="sxs-lookup"><span data-stu-id="f2621-990">Role</span></span>

* <span data-ttu-id="f2621-991">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="f2621-991">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f2621-992">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="f2621-992">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f2621-993">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="f2621-993">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f2621-994">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="f2621-994">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f2621-995">SQL</span><span class="sxs-lookup"><span data-stu-id="f2621-995">SQL</span></span>

* <span data-ttu-id="f2621-996">Adição dos comandos az sql server list-usages e az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="f2621-996">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="f2621-997">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="f2621-997">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f2621-998">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-998">Storage</span></span>

* <span data-ttu-id="f2621-999">Localização padrão da localização do grupo de recursos de `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="f2621-999">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="f2621-1000">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="f2621-1000">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f2621-1001">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="f2621-1001">Add support for large block blob upload</span></span>
* <span data-ttu-id="f2621-1002">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="f2621-1002">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-1003">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-1003">VM</span></span>

* <span data-ttu-id="f2621-1004">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="f2621-1004">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f2621-1005">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="f2621-1005">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f2621-1006">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f2621-1006">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f2621-1007">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f2621-1007">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f2621-1008">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="f2621-1008">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f2621-1009">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="f2621-1009">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f2621-1010">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="f2621-1010">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f2621-1011">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-1011">April 3, 2017</span></span>

<span data-ttu-id="f2621-1012">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f2621-1012">Version 2.0.2</span></span>

<span data-ttu-id="f2621-1013">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão.</span><span class="sxs-lookup"><span data-stu-id="f2621-1013">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="f2621-1014">Núcleo</span><span class="sxs-lookup"><span data-stu-id="f2621-1014">Core</span></span>

* <span data-ttu-id="f2621-1015">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão.</span><span class="sxs-lookup"><span data-stu-id="f2621-1015">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="f2621-1016">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="f2621-1016">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f2621-1017">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="f2621-1017">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f2621-1018">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f2621-1018">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f2621-1019">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="f2621-1019">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f2621-1020">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="f2621-1020">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f2621-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="f2621-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f2621-1022">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="f2621-1022">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f2621-1023">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="f2621-1023">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f2621-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="f2621-1024">ACS</span></span>

* <span data-ttu-id="f2621-1025">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="f2621-1025">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f2621-1026">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="f2621-1026">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f2621-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="f2621-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f2621-1028">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="f2621-1028">Add support for windows clusters.</span></span> <span data-ttu-id="f2621-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="f2621-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f2621-1030">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="f2621-1030">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f2621-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="f2621-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f2621-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="f2621-1032">AppService</span></span>

* <span data-ttu-id="f2621-1033">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="f2621-1033">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f2621-1034">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="f2621-1034">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f2621-1035">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="f2621-1035">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f2621-1036">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="f2621-1036">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f2621-1037">DataLake</span><span class="sxs-lookup"><span data-stu-id="f2621-1037">DataLake</span></span>

* <span data-ttu-id="f2621-1038">Versão inicial do módulo do Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="f2621-1038">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="f2621-1039">Versão inicial do módulo do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f2621-1039">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f2621-1040">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="f2621-1040">DocuemntDB</span></span>

* <span data-ttu-id="f2621-1041">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="f2621-1041">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f2621-1042">VM</span><span class="sxs-lookup"><span data-stu-id="f2621-1042">VM</span></span>

* <span data-ttu-id="f2621-1043">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="f2621-1043">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f2621-1044">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="f2621-1044">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f2621-1045">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="f2621-1045">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f2621-1046">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="f2621-1046">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f2621-1047">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="f2621-1047">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f2621-1048">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="f2621-1048">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="f2621-1049">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="f2621-1049">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f2621-1050">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="f2621-1050">February 27, 2017</span></span>

<span data-ttu-id="f2621-1051">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f2621-1051">Version 2.0.0</span></span>

<span data-ttu-id="f2621-1052">Essa versão da CLI do Azure 2.0 é a primeira versão “Disponível”.</span><span class="sxs-lookup"><span data-stu-id="f2621-1052">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="f2621-1053">A disponibilidade se aplica a esses módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="f2621-1053">General availability applies to these command modules:</span></span>
- <span data-ttu-id="f2621-1054">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="f2621-1054">Container Service (acs)</span></span>
- <span data-ttu-id="f2621-1055">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="f2621-1055">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f2621-1056">Rede</span><span class="sxs-lookup"><span data-stu-id="f2621-1056">Networking</span></span>
- <span data-ttu-id="f2621-1057">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="f2621-1057">Storage</span></span>

<span data-ttu-id="f2621-1058">Esses módulos de comando podem ser usados na produção e são compatíveis com o SLA do Microsoft padrão.</span><span class="sxs-lookup"><span data-stu-id="f2621-1058">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="f2621-1059">Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="f2621-1059">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="f2621-1060">Você pode fazer perguntas sobre [StackOverflow usando a marcação azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) ou entrar em contato com a equipe do produto pelo endereço [ azfeedback@microsoft.com ](mailto:azfeedback@microsoft.com). Você pode fornecer comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f2621-1060">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="f2621-1061">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="f2621-1061">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="f2621-1062">Para verificar a versão da CLI, utilize `az --version`.</span><span class="sxs-lookup"><span data-stu-id="f2621-1062">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="f2621-1063">A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando.</span><span class="sxs-lookup"><span data-stu-id="f2621-1063">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="f2621-1064">Alguns dos módulos de comando têm um "b*n*" ou "rc*n*" como sufixo.</span><span class="sxs-lookup"><span data-stu-id="f2621-1064">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="f2621-1065">Esses módulos de comando ainda estão em visualização e estarão disponíveis no futuro.</span><span class="sxs-lookup"><span data-stu-id="f2621-1065">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="f2621-1066">Também temos compilações de visualização diárias da CLI.</span><span class="sxs-lookup"><span data-stu-id="f2621-1066">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="f2621-1067">Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f2621-1067">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="f2621-1068">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="f2621-1068">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f2621-1069">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="f2621-1069">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f2621-1070">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="f2621-1070">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="f2621-1071">Forneça comentários a partir da linha de comando com o comando `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f2621-1071">Provide feedback from the command line with the `az feedback` command.</span></span>

