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
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="e797e-103">Notas de versão da CLI do Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e797e-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="e797e-104">27 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-104">March 27, 2018</span></span>

<span data-ttu-id="e797e-105">Versão 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e797e-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e797e-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-106">Core</span></span>

* <span data-ttu-id="e797e-107">Mostrar mensagem para extensões marcadas como versão prévia na Ajuda</span><span class="sxs-lookup"><span data-stu-id="e797e-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-108">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-108">ACS</span></span>

* <span data-ttu-id="e797e-109">Corrija o erro de verificação de certificado SSL para `aks install-cli` no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e797e-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-110">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-110">Appservice</span></span>

* <span data-ttu-id="e797e-111">Adição do suporte somente para HTTPS para `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e797e-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="e797e-112">Adição do suporte para os slots `az webapp identity [assign|show]` e `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="e797e-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e797e-113">Backup</span><span class="sxs-lookup"><span data-stu-id="e797e-113">Backup</span></span>

* <span data-ttu-id="e797e-114">Adição do novo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="e797e-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e797e-115">Esse comando pode ser usado para verificar se o backup de uma VM é realizado por qualquer cofre na assinatura</span><span class="sxs-lookup"><span data-stu-id="e797e-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e797e-116">Habilitação das IDs de objeto do Azure para os parâmetros `--resource-group` e `--vault-name` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e797e-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e797e-117">`--name` parâmetros alterados a fim de aceitar o formato de saída dos comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="e797e-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e797e-118">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-118">Container</span></span>

* <span data-ttu-id="e797e-119">Adição do comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="e797e-119">Added `container exec` command.</span></span> <span data-ttu-id="e797e-120">Executa comandos em um contêiner para um grupo de contêiner em execução</span><span class="sxs-lookup"><span data-stu-id="e797e-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e797e-121">Permitir a saída da tabela para criar e atualizar um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e797e-122">Extensão</span><span class="sxs-lookup"><span data-stu-id="e797e-122">Extension</span></span>

* <span data-ttu-id="e797e-123">Mensagem adicionada para `extension add`, se a extensão estiver no modo de versão prévia</span><span class="sxs-lookup"><span data-stu-id="e797e-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e797e-124">`extension list-available` alterado para mostrar dados de extensão total com `--show-details`</span><span class="sxs-lookup"><span data-stu-id="e797e-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="e797e-125">[ALTERAÇÃO SIGNIFICATIVA] `extension list-available` alterado para mostrar dados de extensão simplificados por padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-126">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-126">Interactive</span></span>

* <span data-ttu-id="e797e-127">Alteração nas conclusões para ativar após a conclusão do carregamento da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e797e-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e797e-128">Correção de bug usando o parâmetro `--style`</span><span class="sxs-lookup"><span data-stu-id="e797e-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e797e-129">Analisador léxico interativo instanciado após a falta do despejo da tabela de comandos</span><span class="sxs-lookup"><span data-stu-id="e797e-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e797e-130">Suporte aprimorado ao completador</span><span class="sxs-lookup"><span data-stu-id="e797e-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e797e-131">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-131">Lab</span></span>

* <span data-ttu-id="e797e-132">Correção de bugs com o comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="e797e-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-133">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-133">Monitor</span></span>

* <span data-ttu-id="e797e-134">Adição de suporte para `--top`, `--orderby` e `--namespace` para `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e797e-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e797e-135">[#4529](https://github.com/Azure/azure-cli/issues/5785) corrigido: `metrics list` aceita uma lista separada por espaços de métricas para recuperação</span><span class="sxs-lookup"><span data-stu-id="e797e-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e797e-136">Adição de suporte para `--namespace` para `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="e797e-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e797e-137">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-137">Network</span></span>

* <span data-ttu-id="e797e-138">Adição de suporte para zonas DNS privado</span><span class="sxs-lookup"><span data-stu-id="e797e-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-139">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-139">Profile</span></span>

* <span data-ttu-id="e797e-140">Adição de avisos para `--identity-port` e `--msi-port` para `login`</span><span class="sxs-lookup"><span data-stu-id="e797e-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e797e-141">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e797e-141">RDBMS</span></span>

* <span data-ttu-id="e797e-142">Adição de modelo de negócios GA API versão 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="e797e-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-143">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-143">Resource</span></span>

* [ALTERAÇÃO SIGNIFICATIVA]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e797e-145">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-145">Role</span></span>

* <span data-ttu-id="e797e-146">Adição de suporte para configurações de acesso necessário e clientes nativos para `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="e797e-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="e797e-147">`rbac` comandos alterados para retornar menos de 1000 IDs na resolução do objeto</span><span class="sxs-lookup"><span data-stu-id="e797e-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e797e-148">Adição de comandos de gerenciamento de credencial `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="e797e-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="e797e-149">[ALTERAÇÃO SIGNIFICATIVA] "Propriedades" removidas da saída `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e797e-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e797e-150">Adição de suporte para as permissões `dataActions` e `notDataActions` para `role definition`</span><span class="sxs-lookup"><span data-stu-id="e797e-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-151">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-151">Storage</span></span>

* <span data-ttu-id="e797e-152">Correção de problema ao carregar um arquivo com tamanho entre 195 e 200 GB</span><span class="sxs-lookup"><span data-stu-id="e797e-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e797e-153">[4049#](https://github.com/Azure/azure-cli/issues/4049) corrigido: problemas com o acréscimo de uploads de blob ignorando os parâmetros da condição</span><span class="sxs-lookup"><span data-stu-id="e797e-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-154">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-154">VM</span></span>

* <span data-ttu-id="e797e-155">Adição de aviso para `vmss create` para alterações de falha futuras para conjuntos com mais de 100 instâncias</span><span class="sxs-lookup"><span data-stu-id="e797e-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e797e-156">Adição de suporte com flexibilidade de região para `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="e797e-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="e797e-157">Alteração no modo de exibição de instância de disco para reportar status de criptografia mais adequados</span><span class="sxs-lookup"><span data-stu-id="e797e-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e797e-158">[ALTERAÇÃO SIGNIFICATIVA] `vm extension delete` alterado para não retornar mais a saída</span><span class="sxs-lookup"><span data-stu-id="e797e-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e797e-159">13 de março de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-159">March 13, 2018</span></span>

<span data-ttu-id="e797e-160">Versão 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e797e-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e797e-161">ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-161">ACR</span></span>

* <span data-ttu-id="e797e-162">Suporte adicionado do parâmetro `--image` a `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e797e-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="e797e-163">Parâmetros `--manifest` e `--tag` preteridos do comando `repository delete`</span><span class="sxs-lookup"><span data-stu-id="e797e-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e797e-164">Comando `repository untag` adicionado para remover uma marcação sem excluir dados</span><span class="sxs-lookup"><span data-stu-id="e797e-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-165">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-165">ACS</span></span>

* <span data-ttu-id="e797e-166">Comando `aks upgrade-connector` adicionado para atualizar um conector existente</span><span class="sxs-lookup"><span data-stu-id="e797e-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e797e-167">Arquivos de configuração `kubectl` alterados para usar um YAML mais legível em bloco</span><span class="sxs-lookup"><span data-stu-id="e797e-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e797e-168">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e797e-168">Advisor</span></span>

* <span data-ttu-id="e797e-169">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration get` renomeado para `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="e797e-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="e797e-170">[ALTERAÇÃO SIGNIFICATIVA] `advisor configuration set` renomeado para `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="e797e-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="e797e-171">[ALTERAÇÃO SIGNIFICATIVA] `advisor recommendation generate` removido</span><span class="sxs-lookup"><span data-stu-id="e797e-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="e797e-172">Parâmetro `--refresh` adicionado a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="e797e-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="e797e-173">Adicionado o comando `advisor recommendation show`</span><span class="sxs-lookup"><span data-stu-id="e797e-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-174">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-174">Appservice</span></span>

* <span data-ttu-id="e797e-175">Preterido `[webapp|functionapp] assign-identity`</span><span class="sxs-lookup"><span data-stu-id="e797e-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="e797e-176">Comandos de identidade gerenciada `webapp identity [assign|show]` e `functionapp identity [assign|show]` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="e797e-177">Hubs de eventos</span><span class="sxs-lookup"><span data-stu-id="e797e-177">Eventhubs</span></span>

* <span data-ttu-id="e797e-178">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e797e-179">Extensão</span><span class="sxs-lookup"><span data-stu-id="e797e-179">Extension</span></span>

* <span data-ttu-id="e797e-180">Verificação adicionada para avisar ao usuário se a distribuição usada é diferente da armazenado no arquivo de origem do pacote, pois isso pode levar a erros</span><span class="sxs-lookup"><span data-stu-id="e797e-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-181">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-181">Interactive</span></span>

* <span data-ttu-id="e797e-182">[5625](https://github.com/Azure/azure-cli/issues/5625) corrigido: manter histórico em sessões diferentes</span><span class="sxs-lookup"><span data-stu-id="e797e-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e797e-183">[3016](https://github.com/Azure/azure-cli/issues/3016) corrigido: histórico não registrado no escopo</span><span class="sxs-lookup"><span data-stu-id="e797e-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e797e-184">[5688](https://github.com/Azure/azure-cli/issues/5688) corrigido: as conclusões não aparecerão se o carregamento da tabela de comando encontrou uma exceção</span><span class="sxs-lookup"><span data-stu-id="e797e-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e797e-185">Medidor de progresso corrigido para operações de longa execução</span><span class="sxs-lookup"><span data-stu-id="e797e-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-186">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-186">Monitor</span></span>

* <span data-ttu-id="e797e-187">Comandos `monitor autoscale-settings` preteridos</span><span class="sxs-lookup"><span data-stu-id="e797e-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e797e-188">Adicionados os comandos `monitor autoscale`</span><span class="sxs-lookup"><span data-stu-id="e797e-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e797e-189">Adicionados os comandos `monitor autoscale profile`</span><span class="sxs-lookup"><span data-stu-id="e797e-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e797e-190">Adicionados os comandos `monitor autoscale rule`</span><span class="sxs-lookup"><span data-stu-id="e797e-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e797e-191">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-191">Network</span></span>

* <span data-ttu-id="e797e-192">[ALTERAÇÃO SIGNIFICATIVA] Parâmetro `--tags` removido de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="e797e-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="e797e-193">Valores padrão incorretos removidos dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e797e-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e797e-194">Comandos `network watcher connection-monitor` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e797e-195">Parâmetros `--vnet` e `--subnet` adicionados a `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e797e-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-196">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-196">Profile</span></span>

* <span data-ttu-id="e797e-197">Parâmetro `--msi` preterido de `az login`</span><span class="sxs-lookup"><span data-stu-id="e797e-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="e797e-198">Parâmetro `--identity` adicionado de `az login` para substituir `--msi`</span><span class="sxs-lookup"><span data-stu-id="e797e-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="e797e-199">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e797e-199">RDBMS</span></span>

* <span data-ttu-id="e797e-200">[VISUALIZAÇÃO] Alterado para usar a API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="e797e-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e797e-201">Barramento de Serviço</span><span class="sxs-lookup"><span data-stu-id="e797e-201">Service Bus</span></span>

* <span data-ttu-id="e797e-202">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-203">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-203">Storage</span></span>

* <span data-ttu-id="e797e-204">[#4971](https://github.com/Azure/azure-cli/issues/4971) corrigido: `storage blob copy` agora dá suporte a outras nuvens do Azure</span><span class="sxs-lookup"><span data-stu-id="e797e-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e797e-205">[5286](https://github.com/Azure/azure-cli/issues/5286) corrigido: os comandos em lotes `storage blob [delete-batch|download-batch|upload-batch]` não geram mais um erro após falhas da pré-condição</span><span class="sxs-lookup"><span data-stu-id="e797e-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-206">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-206">VM</span></span>

* <span data-ttu-id="e797e-207">Suporte adicionado a `[vm|vmss] create` anexar discos de dados não gerenciados e configurar o cache</span><span class="sxs-lookup"><span data-stu-id="e797e-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e797e-208">`[vm|vmss] assign-identity` e `[vm|vmss] remove-identity` preteridos</span><span class="sxs-lookup"><span data-stu-id="e797e-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="e797e-209">Comandos `vm identity [assign|remove|show]` e `vmss identity [assign|remove|show]` adicionados para substituir comandos preteridos</span><span class="sxs-lookup"><span data-stu-id="e797e-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e797e-210">Prioridade padrão alterada em `vmss create` para None</span><span class="sxs-lookup"><span data-stu-id="e797e-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e797e-211">27 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-211">February 27, 2018</span></span>

<span data-ttu-id="e797e-212">Versão 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e797e-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e797e-213">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-213">Core</span></span>

* <span data-ttu-id="e797e-214">Correção [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalação do Homebrew</span><span class="sxs-lookup"><span data-stu-id="e797e-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e797e-215">Adição de suporte para telemetria de extensão com chaves personalizadas</span><span class="sxs-lookup"><span data-stu-id="e797e-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e797e-216">Adição de log HTTP em `--debug`</span><span class="sxs-lookup"><span data-stu-id="e797e-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-217">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-217">ACS</span></span>

* <span data-ttu-id="e797e-218">Alteração para usa o gráfico `virtual-kubelet-for-aks` do Helm para `aks install-connector` por padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e797e-219">Correção do problema de permissão insuficiente para entidades de serviço criarem um grupo de contêiner ACI</span><span class="sxs-lookup"><span data-stu-id="e797e-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e797e-220">Adição dos parâmetros `--aci-container-group`, `--location` e `--image-tag` ao `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="e797e-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="e797e-221">Remoção do aviso de reprovação de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="e797e-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-222">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-222">Appservice</span></span>

* <span data-ttu-id="e797e-223">Atualizações para a nova versão do SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e797e-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e797e-224">Correção [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` relatado como SKU inválido</span><span class="sxs-lookup"><span data-stu-id="e797e-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e797e-225">Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e797e-225">Cognitive Services</span></span>

* <span data-ttu-id="e797e-226">Atualização do “aviso” ao criar uma nova conta dos Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e797e-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e797e-227">Consumo</span><span class="sxs-lookup"><span data-stu-id="e797e-227">Consumption</span></span>

* <span data-ttu-id="e797e-228">Adição de novos comandos para a API pricesheet</span><span class="sxs-lookup"><span data-stu-id="e797e-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e797e-229">Atualização dos formatos existentes de Detalhes de uso e Detalhes de reserva</span><span class="sxs-lookup"><span data-stu-id="e797e-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e797e-230">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-230">Container</span></span>

* <span data-ttu-id="e797e-231">Adição dos argumentos `--secrets` e `--secrets-mount-path` ao `container create` para usar segredos na ACI</span><span class="sxs-lookup"><span data-stu-id="e797e-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e797e-232">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-232">Network</span></span>

* <span data-ttu-id="e797e-233">Correção [#5559](https://github.com/Azure/azure-cli/issues/5559): cliente ausente em `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="e797e-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-234">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-234">Resource</span></span>

* <span data-ttu-id="e797e-235">Alteração do `group deployment export` para exibir um modelo parcial e erros ao falhar</span><span class="sxs-lookup"><span data-stu-id="e797e-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e797e-236">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-236">Role</span></span>

* <span data-ttu-id="e797e-237">Adição de `role assignment list-changelogs` para permitir a auditoria das funções da entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="e797e-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-238">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-238">SQL</span></span>

* <span data-ttu-id="e797e-239">Adição de suporte para a redundância de zona para os bancos de dados e pools elásticos em criação ou atualização</span><span class="sxs-lookup"><span data-stu-id="e797e-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-240">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-240">Storage</span></span>

* <span data-ttu-id="e797e-241">Habilitação de especificação de caminho de destino/prefixo do `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="e797e-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-242">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-242">VM</span></span>

* <span data-ttu-id="e797e-243">Adição de suporte para anexar/desanexar discos em uma instância única de VMSS</span><span class="sxs-lookup"><span data-stu-id="e797e-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e797e-244">13 de fevereiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-244">February 13, 2018</span></span>

<span data-ttu-id="e797e-245">Versão 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e797e-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e797e-246">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-246">Core</span></span>

* <span data-ttu-id="e797e-247">Alterada a autenticação para chave tanto na ID de assinatura quanto no nome de logon do MSI</span><span class="sxs-lookup"><span data-stu-id="e797e-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-248">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-248">ACS</span></span>

* <span data-ttu-id="e797e-249">[ALTERAÇÃO SIGNIFICATIVA] `aks get-versions` renomeado para `aks get-upgrades` para fins de precisão</span><span class="sxs-lookup"><span data-stu-id="e797e-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e797e-250">`aks get-versions` alterado para mostrar versões do Kubernetes disponíveis para `aks create`</span><span class="sxs-lookup"><span data-stu-id="e797e-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="e797e-251">Alterados os padrões de `aks create` para permitir que o servidor escolha a versão do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e797e-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e797e-252">Atualizadas as mensagens de ajuda sobre a entidade de serviço gerada pelo AKS</span><span class="sxs-lookup"><span data-stu-id="e797e-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e797e-253">Alterados os tamanhos de nó padrão para `aks create` de “Standard\_D1\_v2” para “Standard\_DS1\_v2”</span><span class="sxs-lookup"><span data-stu-id="e797e-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e797e-254">Aumentada a confiabilidade ao localizar o pod de painel para `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="e797e-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="e797e-255">`aks get-credentials` corrigido para tratar de erros de Unicode ao carregar arquivos de configuração do Kubernetes</span><span class="sxs-lookup"><span data-stu-id="e797e-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e797e-256">Adicionada uma mensagem para `az aks install-cli` para ajudar a obter `kubectl` em `$PATH`</span><span class="sxs-lookup"><span data-stu-id="e797e-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-257">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-257">Appservice</span></span>

* <span data-ttu-id="e797e-258">Corrigido o problema em que `webapp [backup|restore]` falhou devido a uma referência nula</span><span class="sxs-lookup"><span data-stu-id="e797e-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e797e-259">Adicionado suporte para planos de serviço de aplicativo padrão por meio de `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="e797e-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="e797e-260">CDN</span><span class="sxs-lookup"><span data-stu-id="e797e-260">CDN</span></span>

* <span data-ttu-id="e797e-261">Adicionados os comandos `cdn custom-domain [enable-https|disable-https]`</span><span class="sxs-lookup"><span data-stu-id="e797e-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e797e-262">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-262">Container</span></span>

* <span data-ttu-id="e797e-263">Adicionada a opção `--follow` para `az container logs` para logs de streaming</span><span class="sxs-lookup"><span data-stu-id="e797e-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e797e-264">Adicionado o comando `container attach` que anexa fluxos locais de saída e erro padrão para um contêiner em um grupo de contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e797e-265">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-265">CosmosDB</span></span>

* <span data-ttu-id="e797e-266">Adicionado suporte para a configuração de recursos</span><span class="sxs-lookup"><span data-stu-id="e797e-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e797e-267">Extensão</span><span class="sxs-lookup"><span data-stu-id="e797e-267">Extension</span></span>

* <span data-ttu-id="e797e-268">Adicionado suporte para parâmetro `--pip-proxy` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e797e-269">Adicionado suporte para argumento `--pip-extra-index-urls` para comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e797e-270">Comentários</span><span class="sxs-lookup"><span data-stu-id="e797e-270">Feedback</span></span>

* <span data-ttu-id="e797e-271">Adicionadas informações de extensão aos dados de telemetria</span><span class="sxs-lookup"><span data-stu-id="e797e-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-272">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-272">Interactive</span></span>

* <span data-ttu-id="e797e-273">Corrigido o problema em que o usuário é solicitado a fazer logon ao usar o modo interativo no Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="e797e-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e797e-274">Corrigida a regressão com conclusões de parâmetro ausentes</span><span class="sxs-lookup"><span data-stu-id="e797e-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e797e-275">IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-275">IoT</span></span>

* <span data-ttu-id="e797e-276">Correção do problema em que `iot dps access policy [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e797e-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e797e-277">Correção do problema em que `iot dps linked-hub [create|update]` retornaria um erro ‘não encontrado’ em caso de sucesso</span><span class="sxs-lookup"><span data-stu-id="e797e-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e797e-278">Adicionado o suporte `--no-wait` para `iot dps access policy [create|update]` e `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="e797e-279">`iot hub create` alterado para permitir a especificação do número de partições</span><span class="sxs-lookup"><span data-stu-id="e797e-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-280">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-280">Monitor</span></span>

* <span data-ttu-id="e797e-281">Corrigido o comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="e797e-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e797e-282">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-282">Network</span></span>

* <span data-ttu-id="e797e-283">Corrigida a opção `--tags` para os seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="e797e-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e797e-284">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-284">Profile</span></span>

* <span data-ttu-id="e797e-285">`az login` habilitado no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-286">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-286">Resource</span></span>

* <span data-ttu-id="e797e-287">`feature show` adicionado novamente</span><span class="sxs-lookup"><span data-stu-id="e797e-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="e797e-288">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-288">Role</span></span>

* <span data-ttu-id="e797e-289">Adicionado o argumento `--available-to-other-tenants` para `ad app update`</span><span class="sxs-lookup"><span data-stu-id="e797e-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-290">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-290">SQL</span></span>

* <span data-ttu-id="e797e-291">Adicionados os comandos `sql server dns-alias`</span><span class="sxs-lookup"><span data-stu-id="e797e-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e797e-292">Adicionado `sql db rename`</span><span class="sxs-lookup"><span data-stu-id="e797e-292">Added `sql db rename`</span></span>
* <span data-ttu-id="e797e-293">Adicionado suporte para o argumento `--ids` para todos os comandos sql</span><span class="sxs-lookup"><span data-stu-id="e797e-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-294">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-294">Storage</span></span>

* <span data-ttu-id="e797e-295">Adicionados os comandos `storage blob service-properties delete-policy` e `storage blob undelete` para habilitar a exclusão reversível</span><span class="sxs-lookup"><span data-stu-id="e797e-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-296">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-296">VM</span></span>

* <span data-ttu-id="e797e-297">Corrigida uma falha quando a criptografia de VM não pode ser totalmente inicializada</span><span class="sxs-lookup"><span data-stu-id="e797e-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e797e-298">Adicionada saída de ID de entidade de segurança ao habilitar o MSI</span><span class="sxs-lookup"><span data-stu-id="e797e-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e797e-299">`vm boot-diagnostics get-boot-log` fixo</span><span class="sxs-lookup"><span data-stu-id="e797e-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="e797e-300">31 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-300">January 31, 2018</span></span>

<span data-ttu-id="e797e-301">Versão 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e797e-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e797e-302">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-302">Core</span></span>

* <span data-ttu-id="e797e-303">Adicionado suporte para recuperação de token bruto no contexto MSI</span><span class="sxs-lookup"><span data-stu-id="e797e-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e797e-304">Removida a cadeia de caracteres do indicador de sondagem depois de terminar o LRO no Windows cmd.exe</span><span class="sxs-lookup"><span data-stu-id="e797e-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e797e-305">Adicionado um aviso que aparece ao usar um padrão configurado que foi alterado para uma entrada de nível de informações.</span><span class="sxs-lookup"><span data-stu-id="e797e-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e797e-306">Usar `--verbose` para ver</span><span class="sxs-lookup"><span data-stu-id="e797e-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="e797e-307">Adicionar um indicador de progresso para comandos de espera</span><span class="sxs-lookup"><span data-stu-id="e797e-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-308">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-308">ACS</span></span>

* <span data-ttu-id="e797e-309">Argumento `--disable-browser` esclarecido</span><span class="sxs-lookup"><span data-stu-id="e797e-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e797e-310">Preenchimento de guia melhorado para argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="e797e-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-311">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-311">Appservice</span></span>

* <span data-ttu-id="e797e-312">`webapp log [tail|download]` fixo</span><span class="sxs-lookup"><span data-stu-id="e797e-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="e797e-313">Removida a verificação de `kind` em aplicativos Web e funções</span><span class="sxs-lookup"><span data-stu-id="e797e-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e797e-314">CDN</span><span class="sxs-lookup"><span data-stu-id="e797e-314">CDN</span></span>

* <span data-ttu-id="e797e-315">Corrigido o problema de cliente ausente com `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e797e-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e797e-316">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-316">CosmosDB</span></span>

* <span data-ttu-id="e797e-317">Corrigida a descrição do parâmetro para políticas de failover</span><span class="sxs-lookup"><span data-stu-id="e797e-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-318">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-318">Interactive</span></span>

* <span data-ttu-id="e797e-319">Corrigido o problema em que as conclusões de opção de comando não aparecem mais</span><span class="sxs-lookup"><span data-stu-id="e797e-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e797e-320">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-320">Network</span></span>

* <span data-ttu-id="e797e-321">Adicionada a proteção para `--cert-password` para `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="e797e-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="e797e-322">Corrigido o problema com `application-gateway update` em que `--sku` aplicou um valor padrão de forma errada</span><span class="sxs-lookup"><span data-stu-id="e797e-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e797e-323">Adicionada proteção para `--shared-key` e `--authorization-key` para `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e797e-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="e797e-324">Corrigido o problema de cliente ausente com `asg create`</span><span class="sxs-lookup"><span data-stu-id="e797e-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="e797e-325">Adicionado o parâmetro `--file-name / -f` para nomes exportados para `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="e797e-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="e797e-326">Os seguintes problemas foram corrigidos com `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="e797e-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e797e-327">Corrigido o problema em que registros TXT longos foram exportados incorretamente</span><span class="sxs-lookup"><span data-stu-id="e797e-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e797e-328">Corrigido o problema em que registros TXT entre aspas foram exportados incorretamente sem as aspas com caracteres de escape</span><span class="sxs-lookup"><span data-stu-id="e797e-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e797e-329">Corrigido o problema em que determinados registros foram importados duas vezes com `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e797e-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="e797e-330">Restaurados os comandos `vnet-gateway root-cert` e `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="e797e-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-331">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-331">Profile</span></span>

* <span data-ttu-id="e797e-332">`get-access-token` corrigido para trabalhar em uma VM com identidade</span><span class="sxs-lookup"><span data-stu-id="e797e-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-333">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-333">Resource</span></span>

* <span data-ttu-id="e797e-334">Corrigido o bug com `deployment [create|validate]` em que um aviso era exibido incorretamente quando um campo ‘tipo’ do modelo continha valores maiúsculos</span><span class="sxs-lookup"><span data-stu-id="e797e-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-335">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-335">Storage</span></span>

* <span data-ttu-id="e797e-336">Corrigido o problema com a migração de contas de Armazenamento V1 para Armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e797e-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e797e-337">Adicionado o relatório de andamento de todos os comandos de upload/download</span><span class="sxs-lookup"><span data-stu-id="e797e-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e797e-338">Corrigido o bug que impedia a opção “-n” arg com `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="e797e-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="e797e-339">Adicionada a coluna ‘instantâneo’ à saída de tabela para `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="e797e-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="e797e-340">Corrigidos bugs com vários parâmetros que precisam ser analisados como ints</span><span class="sxs-lookup"><span data-stu-id="e797e-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-341">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-341">VM</span></span>

* <span data-ttu-id="e797e-342">Adicionado o comando `vm image accept-terms` para permitir a criação de VMs a partir de imagens com encargos adicionais</span><span class="sxs-lookup"><span data-stu-id="e797e-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e797e-343">`[vm|vmss create]` corrigido para garantir que comandos possam ser executados sob o proxy com certificados não assinados</span><span class="sxs-lookup"><span data-stu-id="e797e-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e797e-344">[VERSÃO PRÉVIA] Adicionado suporte para “baixa” prioridade para VMSS</span><span class="sxs-lookup"><span data-stu-id="e797e-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e797e-345">Adicionada a proteção para `--admin-password` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="e797e-346">17 de janeiro de 2018</span><span class="sxs-lookup"><span data-stu-id="e797e-346">January 17, 2018</span></span>

<span data-ttu-id="e797e-347">Versão 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e797e-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e797e-348">ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-348">ACR</span></span>

* <span data-ttu-id="e797e-349">Adicionado fallback de logon de acr em erros de credencial do Windows</span><span class="sxs-lookup"><span data-stu-id="e797e-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e797e-350">Habilitados os logs de registro</span><span class="sxs-lookup"><span data-stu-id="e797e-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-351">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-351">ACS</span></span>

* <span data-ttu-id="e797e-352">Corrigido o comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="e797e-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e797e-353">Removido o requisito de função do SPN</span><span class="sxs-lookup"><span data-stu-id="e797e-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-354">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-354">Appservice</span></span>

* <span data-ttu-id="e797e-355">Corrigido o bug com `config ssl upload` onde `hosting_environment_profile` era nulo</span><span class="sxs-lookup"><span data-stu-id="e797e-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e797e-356">Adicionado suporte para URLs personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="e797e-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="e797e-357">Corrigido o suporte de slot para `log tail`</span><span class="sxs-lookup"><span data-stu-id="e797e-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="e797e-358">Backup</span><span class="sxs-lookup"><span data-stu-id="e797e-358">Backup</span></span>

* <span data-ttu-id="e797e-359">Alterada a opção `--container-name` de `backup item list` para ser opcional</span><span class="sxs-lookup"><span data-stu-id="e797e-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e797e-360">Adicionadas opções da conta de armazenamento para `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="e797e-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="e797e-361">Corrigido o check-in de local de `backup protection enable-for-vm` para não diferenciar maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="e797e-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e797e-362">Corrigido o problema em que os comandos falhavam com um nome de contêiner inválido</span><span class="sxs-lookup"><span data-stu-id="e797e-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e797e-363">Alterado `backup item list` para incluir o 'Status de Integridade' como padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e797e-364">Batch</span><span class="sxs-lookup"><span data-stu-id="e797e-364">Batch</span></span>

* <span data-ttu-id="e797e-365">Alterado `batch login` para retornar detalhes de autenticação</span><span class="sxs-lookup"><span data-stu-id="e797e-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e797e-366">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e797e-366">Cloud</span></span>

* <span data-ttu-id="e797e-367">Alterado para não exigir pontos de extremidade ao definir `--profile` em uma nuvem</span><span class="sxs-lookup"><span data-stu-id="e797e-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e797e-368">Consumo</span><span class="sxs-lookup"><span data-stu-id="e797e-368">Consumption</span></span>

* <span data-ttu-id="e797e-369">Adicionados novos comandos para reservas: `consumption reservations summaries` e `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="e797e-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="e797e-370">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e797e-370">Event Grid</span></span>

* <span data-ttu-id="e797e-371">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid topic event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e797e-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e797e-372">[ALTERAÇÃO SIGNIFICATIVA] Comandos `az eventgrid resource event-subscription` transferidos para `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="e797e-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="e797e-373">[ALTERAÇÃO SIGNIFICATIVA] Comando `eventgrid event-subscription show-endpoint-url` removido.</span><span class="sxs-lookup"><span data-stu-id="e797e-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e797e-374">Usar `eventgrid event-subscription show --include-full-endpoint-url`</span><span class="sxs-lookup"><span data-stu-id="e797e-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e797e-375">Adicionado o comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="e797e-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="e797e-376">Adicionado o comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="e797e-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="e797e-377">Adicionado o parâmetro `--ids` para comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="e797e-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e797e-378">Adicionado o suporte de conclusão de guia para nomes de tópico</span><span class="sxs-lookup"><span data-stu-id="e797e-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-379">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-379">Interactive</span></span>

* <span data-ttu-id="e797e-380">Corrigido o problema em que o modo interativo não funcionava com o Python 2.x</span><span class="sxs-lookup"><span data-stu-id="e797e-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e797e-381">Corrigidos os erros na inicialização</span><span class="sxs-lookup"><span data-stu-id="e797e-381">Fixed errors on startup</span></span>
* <span data-ttu-id="e797e-382">Corrigido o problema com alguns comandos que não estavam em execução no modo interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e797e-383">IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-383">IoT</span></span>

* <span data-ttu-id="e797e-384">Adicionado suporte para o serviço de provisionamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e797e-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="e797e-385">Adicionadas mensagens de reprovação em comandos e ajuda de comando</span><span class="sxs-lookup"><span data-stu-id="e797e-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e797e-386">Adicionada verificação de IoT para informar os usuários da Extensão de IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-387">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-387">Monitor</span></span>

* <span data-ttu-id="e797e-388">Adicionado o suporte de configuração de vários diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="e797e-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e797e-389">Agora o parâmetro `--name` é necessário para `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="e797e-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="e797e-390">Adicionado o comando `monitor diagnostic-settings categories` para obter a categoria de configurações de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e797e-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e797e-391">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-391">Network</span></span>

* <span data-ttu-id="e797e-392">Corrigido o problema ao tentar alterar de/para o modo ativo-em espera com `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="e797e-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="e797e-393">Adicionado o suporte para HTTP2 para `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-394">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-394">Profile</span></span>

* <span data-ttu-id="e797e-395">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e797e-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e797e-396">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-396">Role</span></span>

* <span data-ttu-id="e797e-397">Adicionado o argumento `--assignee-object-id` para `role assignment create` para ignorar a consulta do gráfico</span><span class="sxs-lookup"><span data-stu-id="e797e-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e797e-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e797e-398">Service Fabric</span></span>

* <span data-ttu-id="e797e-399">Adicionados erros detalhados à resposta de validação ao criar cluster</span><span class="sxs-lookup"><span data-stu-id="e797e-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e797e-400">Corrigido o problema de cliente ausente com vários comandos</span><span class="sxs-lookup"><span data-stu-id="e797e-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-401">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-401">VM</span></span>

* <span data-ttu-id="e797e-402">[VERSÃO PRÉVIA] Suporte entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="e797e-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="e797e-403">[ALTERAÇÃO SIGNIFICATIVA] Alterada única zona `vmss` padrão para o balanceador de carga "Padrão"</span><span class="sxs-lookup"><span data-stu-id="e797e-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e797e-404">[ALTERAÇÃO SIGNIFICATIVA] `externalIdentities` alterado para `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="e797e-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e797e-405">[VERSÃO PRÉVIA] Adicionado o suporte para a troca de disco do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e797e-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e797e-406">Adicionado o suporte para o uso de imagens da VM de outras assinaturas</span><span class="sxs-lookup"><span data-stu-id="e797e-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e797e-407">Adicionados os argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` e `--plan-publisher` para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="e797e-408">Corrigidos os problemas de erro com `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="e797e-409">Corrigido o uso excessivo de recursos causados por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="e797e-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="e797e-410">19 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-410">December 19, 2017</span></span>

<span data-ttu-id="e797e-411">Versão 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e797e-411">Version 2.0.23</span></span>

* <span data-ttu-id="e797e-412">Adicionado o suporte para logon com identidades atribuídas ao usuário</span><span class="sxs-lookup"><span data-stu-id="e797e-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e797e-413">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-413">Container</span></span>

* <span data-ttu-id="e797e-414">Corrigida a ordem incorreta de parâmetros para logs de contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e797e-415">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-415">Network</span></span>

* <span data-ttu-id="e797e-416">Adicionado o argumento `--disable-bgp-route-propagation` para `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="e797e-417">Adicionado o argumento `--ip-tags` para `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-418">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-418">Storage</span></span>

* <span data-ttu-id="e797e-419">Adicionado suporte para armazenamento V2</span><span class="sxs-lookup"><span data-stu-id="e797e-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-420">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-420">VM</span></span>

* <span data-ttu-id="e797e-421">[VERSÃO PRÉVIA] Adicionado suporte para identidades atribuídas a usuários para VMs e VMSSes</span><span class="sxs-lookup"><span data-stu-id="e797e-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e797e-422">5 de dezembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-422">December 5, 2017</span></span>

<span data-ttu-id="e797e-423">Versão 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e797e-423">Version 2.0.22</span></span>

* <span data-ttu-id="e797e-424">Comandos `az component` removidos.</span><span class="sxs-lookup"><span data-stu-id="e797e-424">Removed `az component` commands.</span></span> <span data-ttu-id="e797e-425">Usar `az extension`</span><span class="sxs-lookup"><span data-stu-id="e797e-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e797e-426">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-426">Core</span></span>
* <span data-ttu-id="e797e-427">Modificou o ponto de extremidade de autoridade AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com para login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="e797e-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e797e-428">Corrigido o problema onde a telemetria reenviaria continuamente</span><span class="sxs-lookup"><span data-stu-id="e797e-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-429">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-429">ACS</span></span>

* <span data-ttu-id="e797e-430">Comandos `aks install-connector` e `aks remove-connector` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e797e-431">Relatório de erros aprimorado para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e797e-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="e797e-432">Corrigido o uso de `aks get-credentials -f` sem um caminho totalmente qualificado</span><span class="sxs-lookup"><span data-stu-id="e797e-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e797e-433">Supervisor</span><span class="sxs-lookup"><span data-stu-id="e797e-433">Advisor</span></span>

* <span data-ttu-id="e797e-434">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-435">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-435">Appservice</span></span>

* <span data-ttu-id="e797e-436">Corrigida a geração de nome do certificado com `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="e797e-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="e797e-437">Corrigidos `webapp [list|show]` e `functionapp [list|show]` para exibir os aplicativos corretos</span><span class="sxs-lookup"><span data-stu-id="e797e-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e797e-438">Valor padrão adicionado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="e797e-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="e797e-439">Consumo</span><span class="sxs-lookup"><span data-stu-id="e797e-439">Consumption</span></span>

* <span data-ttu-id="e797e-440">Suporte adicionado para a API versão de 30/11/2017</span><span class="sxs-lookup"><span data-stu-id="e797e-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e797e-441">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-441">Container</span></span>

* <span data-ttu-id="e797e-442">Corrigida a regressão de portas padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-443">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-443">Monitor</span></span>

* <span data-ttu-id="e797e-444">Suporte de várias dimensões adicionado ao comando de métricas</span><span class="sxs-lookup"><span data-stu-id="e797e-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-445">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-445">Resource</span></span>

* <span data-ttu-id="e797e-446">Adicionado o argumento `--include-response-body` para `resource show`</span><span class="sxs-lookup"><span data-stu-id="e797e-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="e797e-447">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-447">Role</span></span>

* <span data-ttu-id="e797e-448">Exibição de atribuições padrão adicionada dos administradores "clássicos" para `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="e797e-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="e797e-449">Suporte adicionado a `ad sp reset-credentials` para adicionar as credenciais em vez de substituir</span><span class="sxs-lookup"><span data-stu-id="e797e-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e797e-450">Relatório de erros aprimorado para `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e797e-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-451">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-451">SQL</span></span>

* <span data-ttu-id="e797e-452">Comandos `sql db list-usages` e `sql db show-usage` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e797e-453">Comandos `sql server conn-policy show` e `sql server conn-policy update` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-454">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-454">VM</span></span>

* <span data-ttu-id="e797e-455">Informações da zona adicionadas a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="e797e-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="e797e-456">14 de novembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-456">November 14, 2017</span></span>

<span data-ttu-id="e797e-457">Versão 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e797e-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e797e-458">ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-458">ACR</span></span>

* <span data-ttu-id="e797e-459">Suporte adicionado para criar webhooks em regiões de replicação</span><span class="sxs-lookup"><span data-stu-id="e797e-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e797e-460">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-460">ACS</span></span>

* <span data-ttu-id="e797e-461">Alteradas todas as palavras "agente" para "nó" no AKS</span><span class="sxs-lookup"><span data-stu-id="e797e-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e797e-462">Opção `--orchestrator-release` preterida para `acs create`</span><span class="sxs-lookup"><span data-stu-id="e797e-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="e797e-463">Tamanho alterado da VM padrão do AKS para `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="e797e-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="e797e-464">`az aks browse` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e797e-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e797e-465">`az aks get-credentials` corrigido no Windows</span><span class="sxs-lookup"><span data-stu-id="e797e-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-466">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-466">Appservice</span></span>

* <span data-ttu-id="e797e-467">Origem da implantação adicional `config-zip` para webapps e aplicativos de funções</span><span class="sxs-lookup"><span data-stu-id="e797e-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e797e-468">Opção `--docker-container-logging` adicionada a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e797e-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="e797e-469">Removida a opção `storage` do parâmetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="e797e-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="e797e-470">Mensagens de erro aprimoradas para `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="e797e-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="e797e-471">Suporte adicionado para criar aplicativos de funções do Linux</span><span class="sxs-lookup"><span data-stu-id="e797e-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e797e-472">`list-locations` fixo</span><span class="sxs-lookup"><span data-stu-id="e797e-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="e797e-473">Batch</span><span class="sxs-lookup"><span data-stu-id="e797e-473">Batch</span></span>

* <span data-ttu-id="e797e-474">Bug corrigido no comando pool create quando uma ID do recurso foi usada com o sinalizador `--image`</span><span class="sxs-lookup"><span data-stu-id="e797e-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e797e-475">Batchai</span><span class="sxs-lookup"><span data-stu-id="e797e-475">Batchai</span></span>

* <span data-ttu-id="e797e-476">Opção curta adicionada `-s` para `--vm-size` ao fornecer o tamanho da VM no comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="e797e-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e797e-477">Nome da conta de armazenamento e argumentos-chave adicionados aos parâmetros `cluster create`</span><span class="sxs-lookup"><span data-stu-id="e797e-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e797e-478">Documentação corrigida para `job list-files` e `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="e797e-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="e797e-479">Opção curta adicionada `-r` para `--cluster-name` ao fornecer o nome do cluster no comando `job create`</span><span class="sxs-lookup"><span data-stu-id="e797e-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e797e-480">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e797e-480">Cloud</span></span>

* <span data-ttu-id="e797e-481">`cloud [register|update]` alterado para evitar registrar nuvens sem os pontos de extremidade necessários</span><span class="sxs-lookup"><span data-stu-id="e797e-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e797e-482">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-482">Container</span></span>

* <span data-ttu-id="e797e-483">Suporte adicionado para abrir várias portas</span><span class="sxs-lookup"><span data-stu-id="e797e-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="e797e-484">Política de reinicialização do grupo de contêiner adicionada</span><span class="sxs-lookup"><span data-stu-id="e797e-484">Added container group restart policy</span></span>
* <span data-ttu-id="e797e-485">Suporte adicionado para montar o compartilhamento de Arquivos do Azure como um volume</span><span class="sxs-lookup"><span data-stu-id="e797e-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e797e-486">Documentos de ajuda atualizados</span><span class="sxs-lookup"><span data-stu-id="e797e-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e797e-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e797e-487">Data Lake Analytics</span></span>

* <span data-ttu-id="e797e-488">`[job|account] list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e797e-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e797e-489">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="e797e-489">Data Lake Store</span></span>

* <span data-ttu-id="e797e-490">`account list` alterada para retornar informações mais concisas</span><span class="sxs-lookup"><span data-stu-id="e797e-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e797e-491">Extensão</span><span class="sxs-lookup"><span data-stu-id="e797e-491">Extension</span></span>

* <span data-ttu-id="e797e-492">`extension list-available` adicionado para permitir a listagem de extensões oficiais da Microsoft</span><span class="sxs-lookup"><span data-stu-id="e797e-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e797e-493">`--name` adicionado a `extension [add|update]` para permitir a instalação de extensões por nome</span><span class="sxs-lookup"><span data-stu-id="e797e-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e797e-494">IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-494">IoT</span></span>

* <span data-ttu-id="e797e-495">Suporte adicionado para as autoridades de certificação (CA) e cadeias de certificado</span><span class="sxs-lookup"><span data-stu-id="e797e-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-496">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-496">Monitor</span></span>

* <span data-ttu-id="e797e-497">Adicionados os comandos `activity-log alert`</span><span class="sxs-lookup"><span data-stu-id="e797e-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e797e-498">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-498">Network</span></span>

* <span data-ttu-id="e797e-499">Suporte adicionado para registros DNS da CAA</span><span class="sxs-lookup"><span data-stu-id="e797e-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e797e-500">Problema corrigido onde os pontos de extremidade não podem ser atualizados com `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="e797e-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="e797e-501">Problema corrigido onde `vnet update --dns-servers` não funcionou dependendo de como a VNET foi criada</span><span class="sxs-lookup"><span data-stu-id="e797e-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e797e-502">Problema corrigido onde os nomes DNS relativos foram importados incorretamente por`dns zone import`</span><span class="sxs-lookup"><span data-stu-id="e797e-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="e797e-503">Reservas</span><span class="sxs-lookup"><span data-stu-id="e797e-503">Reservations</span></span>

* <span data-ttu-id="e797e-504">Versão prévia inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-505">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-505">Resource</span></span>

* <span data-ttu-id="e797e-506">Suporte adicionado das IDs de recurso ao parâmetro `--resource` e bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-507">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-507">SQL</span></span>

* <span data-ttu-id="e797e-508">Parâmetro `--ignore-missing-vnet-service-endpoint` adicionado a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-509">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-509">Storage</span></span>

* <span data-ttu-id="e797e-510">`storage account create` criado ao usar o SKU `Standard_RAGRS` como padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e797e-511">Bugs corrigidos ao lidar com nomes de arquivo/blob que incluem caracteres não ascii</span><span class="sxs-lookup"><span data-stu-id="e797e-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e797e-512">Bug corrigido que impedia usar `--source-uri` com `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="e797e-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="e797e-513">Comandos adicionados para usar o glob e excluir vários objetos com `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="e797e-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="e797e-514">Problema corrigido ao habilitar métricas com `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="e797e-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="e797e-515">Problema corrigido com arquivos acima de 200 GB ao usar `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="e797e-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="e797e-516">Problema corrigido onde `--bypass` e `--default-action` foram ignorados por `storage account [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-517">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-517">VM</span></span>

* <span data-ttu-id="e797e-518">Bug corrigido com `vmss create`, que impediu o uso da camada de tamanho `Basic`</span><span class="sxs-lookup"><span data-stu-id="e797e-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e797e-519">Argumentos `--plan` adicionados a `[vm|vmss] create` para ter imagens personalizadas com informações de cobrança</span><span class="sxs-lookup"><span data-stu-id="e797e-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e797e-520">Comandos `vm secret `[add|remove|list]\` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e797e-521">`vm format-secret` renomeado para `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="e797e-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="e797e-522">Adicionado o argumento `--encrypt format` para `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e797e-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="e797e-523">24 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-523">October 24, 2017</span></span>

<span data-ttu-id="e797e-524">Versão 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e797e-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e797e-525">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-525">Core</span></span>

* <span data-ttu-id="e797e-526">Atualizado `2017-03-09-profile` para usar a `MGMT_STORAGE` versão da API`2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="e797e-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="e797e-527">ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-527">ACR</span></span>

* <span data-ttu-id="e797e-528">Gerenciamento de recursos atualizado para apontar para a versão da API `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e797e-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e797e-529">SKU 'traga seu próprio armazenamento' alterada para Clássico</span><span class="sxs-lookup"><span data-stu-id="e797e-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e797e-530">SKUs de registro renomeados como Básico, Standard e Premium</span><span class="sxs-lookup"><span data-stu-id="e797e-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-531">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-531">ACS</span></span>

* <span data-ttu-id="e797e-532">[VERSÃO PRÉVIA] Comandos `az aks` adicionados</span><span class="sxs-lookup"><span data-stu-id="e797e-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e797e-533">Kubernetes `get-credentials` corrigido</span><span class="sxs-lookup"><span data-stu-id="e797e-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-534">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-534">Appservice</span></span>

* <span data-ttu-id="e797e-535">Problema corrigido onde os logs `webapp` baixados podem ser inválidos</span><span class="sxs-lookup"><span data-stu-id="e797e-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e797e-536">Componente</span><span class="sxs-lookup"><span data-stu-id="e797e-536">Component</span></span>

* <span data-ttu-id="e797e-537">Mensagem de reprovação mais clara adicionada para todos os instaladores e prompt de confirmação</span><span class="sxs-lookup"><span data-stu-id="e797e-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-538">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-538">Monitor</span></span>

* <span data-ttu-id="e797e-539">Adicionados os comandos `action-group`</span><span class="sxs-lookup"><span data-stu-id="e797e-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-540">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-540">Resource</span></span>

* <span data-ttu-id="e797e-541">Incompatibilidade corrigida com a versão mais recente de dependência msrest em `group export`</span><span class="sxs-lookup"><span data-stu-id="e797e-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="e797e-542">`policy assignment create` corrigido para trabalhar com as definições de política internas e as definições do conjunto de políticas</span><span class="sxs-lookup"><span data-stu-id="e797e-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-543">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-543">VM</span></span>

* <span data-ttu-id="e797e-544">Adicionado o argumento `--accelerated-networking` para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e797e-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="e797e-545">9 de outubro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-545">October 9, 2017</span></span>

<span data-ttu-id="e797e-546">Versão 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e797e-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e797e-547">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-547">Core</span></span>

* <span data-ttu-id="e797e-548">Tratamento de URLs de autoridade do AD FS adicionado com uma barra à direita para o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e797e-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-549">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-549">Appservice</span></span>

* <span data-ttu-id="e797e-550">Atualização genérica adicionada com o novo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="e797e-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="e797e-551">Batch</span><span class="sxs-lookup"><span data-stu-id="e797e-551">Batch</span></span>

* <span data-ttu-id="e797e-552">Atualizado para o SDK do Lote 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e797e-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e797e-553">A opção `--image` de VirtualMachineConfiguration foi atualizada para dar suporte a referências de imagem ARM além de publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="e797e-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e797e-554">Suporte adicionado para o novo modelo de extensão da CLI para comandos de Extensões de Lote</span><span class="sxs-lookup"><span data-stu-id="e797e-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e797e-555">Removeu o suporte de Lote do modelo de componente</span><span class="sxs-lookup"><span data-stu-id="e797e-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e797e-556">Batchai</span><span class="sxs-lookup"><span data-stu-id="e797e-556">Batchai</span></span>

* <span data-ttu-id="e797e-557">Versão inicial do módulo de IA de Lote</span><span class="sxs-lookup"><span data-stu-id="e797e-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e797e-558">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e797e-558">Keyvault</span></span>

* <span data-ttu-id="e797e-559">Correção do problema de autenticação do Cofre de Chaves ao usar o AD FS no Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e797e-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e797e-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="e797e-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e797e-561">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-561">Network</span></span>

* <span data-ttu-id="e797e-562">Alterado `--server` argumento de `application-gateway address-pool create` para ser opcional, permitindo pools de endereços vazios</span><span class="sxs-lookup"><span data-stu-id="e797e-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e797e-563">`traffic-manager` foi atualizado para oferecer suporte aos recursos mais recentes</span><span class="sxs-lookup"><span data-stu-id="e797e-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-564">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-564">Resource</span></span>

* <span data-ttu-id="e797e-565">Suporte adicionado para `--resource-group/-g` opções do nome do grupo de recursos para `group`</span><span class="sxs-lookup"><span data-stu-id="e797e-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="e797e-566">Comandos adicionados a `account lock` para funcionar com bloqueios no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="e797e-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e797e-567">Comandos adicionados a `group lock` para funcionar com bloqueios no nível do grupo</span><span class="sxs-lookup"><span data-stu-id="e797e-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e797e-568">Comandos adicionados a `resource lock` para funcionar com bloqueios no nível do recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-569">Sql</span><span class="sxs-lookup"><span data-stu-id="e797e-569">Sql</span></span>

* <span data-ttu-id="e797e-570">Suporte adicionado para SQL TDE (Transparent Data Encryption) e TDE com Traga sua própria chave</span><span class="sxs-lookup"><span data-stu-id="e797e-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e797e-571">Comando `db list-deleted` e parâmetro `db restore --deleted-time` adicionados, permitindo localizar e restaurar bancos de dados excluídos</span><span class="sxs-lookup"><span data-stu-id="e797e-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e797e-572">`db op list` e `db op cancel` adicionados, permitindo listar e cancelar operações em andamento no banco de dados</span><span class="sxs-lookup"><span data-stu-id="e797e-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-573">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-573">Storage</span></span>

* <span data-ttu-id="e797e-574">Suporte adicionado para instantâneo de compartilhamento de arquivos</span><span class="sxs-lookup"><span data-stu-id="e797e-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-575">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-575">Vm</span></span>

* <span data-ttu-id="e797e-576">Correção de um bug em `vm show` onde o uso de `-d` causou uma falha nos endereços IP privados ausentes</span><span class="sxs-lookup"><span data-stu-id="e797e-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e797e-577">[VERSÃO PRÉVIA] Suporte adicionado para atualização sem interrupção para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e797e-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="e797e-578">Suporte adicionado para atualizar as configurações de criptografia com `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="e797e-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="e797e-579">Parâmetro `--os-disk-size-gb` adicionado a `vm create`</span><span class="sxs-lookup"><span data-stu-id="e797e-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="e797e-580">Parâmetro `--license-type` adicionado ao Windows para `vmss create`</span><span class="sxs-lookup"><span data-stu-id="e797e-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="e797e-581">22 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-581">September 22, 2017</span></span>

<span data-ttu-id="e797e-582">Versão 2.0.1.8</span><span class="sxs-lookup"><span data-stu-id="e797e-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-583">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-583">Resource</span></span>

* <span data-ttu-id="e797e-584">Suporte adicionado para mostrar as definições de políticas internas</span><span class="sxs-lookup"><span data-stu-id="e797e-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e797e-585">Parâmetro de modo de suporte adicionado para a criação de definições de política</span><span class="sxs-lookup"><span data-stu-id="e797e-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e797e-586">Suporte adicionado para definições de interface do usuário e modelos em `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="e797e-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="e797e-587">[ALTERAÇÃO SIGNIFICATIVA] Tipo de recurso `managedapp` alterado de `appliances` para `applications` e de `applianceDefinitions` para `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="e797e-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="e797e-588">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-588">Network</span></span>

* <span data-ttu-id="e797e-589">Suporte adicionado para a zona de disponibilidade para os subcomandos `network lb` e `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e797e-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e797e-590">Suporte adicionado ao Emparelhamento IPv6 da Microsoft para `express-route`</span><span class="sxs-lookup"><span data-stu-id="e797e-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="e797e-591">Adicionados `asg` comandos de grupo de segurança do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e797e-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e797e-592">Adicionado o argumento `--application-security-groups` para `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="e797e-593">Adicionados os argumentos `--source-asgs` e `--destination-asgs` para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e797e-594">Adicionados os argumentos `--ddos-protection` e `--vm-protection` para `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="e797e-595">Adicionados os comandos `network [vnet-gateway|vpn-client|show-url]`</span><span class="sxs-lookup"><span data-stu-id="e797e-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-596">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-596">Storage</span></span>

* <span data-ttu-id="e797e-597">Correção do problema onde `storage account network-rule` comandos poderão falhar após a atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="e797e-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e797e-598">Grade de eventos</span><span class="sxs-lookup"><span data-stu-id="e797e-598">Eventgrid</span></span>

* <span data-ttu-id="e797e-599">Atualizada SDK Python da Grade de Eventos do Azure para usar a versão de API mais recente "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="e797e-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-600">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-600">SQL</span></span>

* <span data-ttu-id="e797e-601">Alterado o `sql server list` argumento `--resource-group` para ser opcional.</span><span class="sxs-lookup"><span data-stu-id="e797e-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e797e-602">Se não for especificado, todos os servidores sql na assinatura serão retornados</span><span class="sxs-lookup"><span data-stu-id="e797e-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e797e-603">Adicionado o `--no-wait` parâmetro para `db [create|copy|restore|update|replica create|create|update]` e `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="e797e-604">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e797e-604">Keyvault</span></span>

* <span data-ttu-id="e797e-605">Adicionado suporte para comandos Keyvault por trás de um proxy</span><span class="sxs-lookup"><span data-stu-id="e797e-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-606">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-606">VM</span></span>

* <span data-ttu-id="e797e-607">Adicionado suporte à zona de disponibilidade para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="e797e-608">Correção do problema onde usar`--app-gateway ID` com `vmss create` poderia causar uma falha</span><span class="sxs-lookup"><span data-stu-id="e797e-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e797e-609">Adicionado o argumento `--asgs` para `vm create`</span><span class="sxs-lookup"><span data-stu-id="e797e-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="e797e-610">Suporte adicionado para executar comandos em VMs com `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="e797e-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="e797e-611">[VERSÃO PRÉVIA] Adicionado suporte para criptografia de disco VMSS com `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="e797e-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="e797e-612">Suporte adicionado para realizar a manutenção em VMs com `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="e797e-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-613">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-613">ACS</span></span>

* <span data-ttu-id="e797e-614">[VERSÃO PRÉVIA] Adicionado `--orchestrator-release` argumento para `acs create` para regiões de versão prévia do ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-615">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-615">Appservice</span></span>

* <span data-ttu-id="e797e-616">Adicionada a capacidade para atualizar e mostrar as configurações de autenticação com `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="e797e-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="e797e-617">Backup</span><span class="sxs-lookup"><span data-stu-id="e797e-617">Backup</span></span>

* <span data-ttu-id="e797e-618">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e797e-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e797e-619">11 de setembro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-619">September 11, 2017</span></span>

<span data-ttu-id="e797e-620">Versão 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e797e-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e797e-621">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-621">Core</span></span>

* <span data-ttu-id="e797e-622">Módulo de comando habilitado para definir sua própria ID de correlação na telemetria</span><span class="sxs-lookup"><span data-stu-id="e797e-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e797e-623">Problema de despejo de JSON corrigido quando a telemetria é definida como modo de diagnóstico</span><span class="sxs-lookup"><span data-stu-id="e797e-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-624">Acs</span><span class="sxs-lookup"><span data-stu-id="e797e-624">Acs</span></span>

* <span data-ttu-id="e797e-625">Adicionado o comando `acs list-locations`</span><span class="sxs-lookup"><span data-stu-id="e797e-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e797e-626">Fez `ssh-key-file` vir com o valor padrão esperado</span><span class="sxs-lookup"><span data-stu-id="e797e-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-627">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-627">Appservice</span></span>

* <span data-ttu-id="e797e-628">Foi incluída a capacidade de criar um aplicativo Web em um grupo de recursos que não seja o plano de serviço ativo</span><span class="sxs-lookup"><span data-stu-id="e797e-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e797e-629">CDN</span><span class="sxs-lookup"><span data-stu-id="e797e-629">CDN</span></span>

* <span data-ttu-id="e797e-630">Foi corrigido o bug 'Não é possível interar CustomDomain' para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="e797e-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="e797e-631">Extensão</span><span class="sxs-lookup"><span data-stu-id="e797e-631">Extension</span></span>

* <span data-ttu-id="e797e-632">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e797e-633">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e797e-633">Keyvault</span></span>

* <span data-ttu-id="e797e-634">Foi corrigido o problema onde permissões diferenciavam maiúsculas de minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="e797e-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="e797e-635">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-635">Network</span></span>

* <span data-ttu-id="e797e-636">`vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e797e-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e797e-637">Foi renomeado o argumento `--private-access-services` para `--service-endpoints` para `vnet subnet create/update`</span><span class="sxs-lookup"><span data-stu-id="e797e-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="e797e-638">Foi adicionado suporte a vários intervalos de IP e intervalos de portas para `nsg rule create/update`</span><span class="sxs-lookup"><span data-stu-id="e797e-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="e797e-639">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e797e-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e797e-640">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e797e-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-641">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-641">Resource</span></span>

* <span data-ttu-id="e797e-642">Permitir a passagem de definições de parâmetro de políticas de recursos em `policy definition create` e`policy definition update`</span><span class="sxs-lookup"><span data-stu-id="e797e-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="e797e-643">Permitir a passagem de valores de parâmetro para`policy assignment create`</span><span class="sxs-lookup"><span data-stu-id="e797e-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="e797e-644">Permitir a passagem de JSON ou arquivo para todos os parâmetros</span><span class="sxs-lookup"><span data-stu-id="e797e-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e797e-645">Versão da API incrementada</span><span class="sxs-lookup"><span data-stu-id="e797e-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-646">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-646">SQL</span></span>

* <span data-ttu-id="e797e-647">Adicionados os comandos `sql server vnet-rule`</span><span class="sxs-lookup"><span data-stu-id="e797e-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-648">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-648">VM</span></span>

* <span data-ttu-id="e797e-649">Corrigido: Não atribuir acesso, a menos que `--scope` seja fornecido</span><span class="sxs-lookup"><span data-stu-id="e797e-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e797e-650">Corrigido: Usar a mesma nomenclatura de extensão do que o portal</span><span class="sxs-lookup"><span data-stu-id="e797e-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e797e-651">Foi removido `subscription` da saída de `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e797e-652">Corrigido: SKU de armazenamento do `[vm|vmss] create` não é aplicada em discos de dados com uma imagem</span><span class="sxs-lookup"><span data-stu-id="e797e-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e797e-653">Corrigido: `vm format-secret --secrets` não aceita IDs de separados de nova linha</span><span class="sxs-lookup"><span data-stu-id="e797e-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e797e-654">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-654">August 31, 2017</span></span>

<span data-ttu-id="e797e-655">Versão 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e797e-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e797e-656">Keyvault</span><span class="sxs-lookup"><span data-stu-id="e797e-656">Keyvault</span></span>

* <span data-ttu-id="e797e-657">Correção do bug ao tentar resolver automaticamente a codificação secreta com `secret download`</span><span class="sxs-lookup"><span data-stu-id="e797e-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="e797e-658">Sf</span><span class="sxs-lookup"><span data-stu-id="e797e-658">Sf</span></span>

* <span data-ttu-id="e797e-659">Substituição de todos os comandos em favor da CLI do Service Fabric (sfctl)</span><span class="sxs-lookup"><span data-stu-id="e797e-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-660">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-660">Storage</span></span>

* <span data-ttu-id="e797e-661">Correção de problema onde as contas de armazenamento não conseguiam ser criadas em regiões sem suporte ao recurso NetworkACLs</span><span class="sxs-lookup"><span data-stu-id="e797e-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e797e-662">Determinar o tipo de conteúdo e a codificação do conteúdo durante o upload de arquivo e de blob se nem o tipo de conteúdo nem a codificação de conteúdo forem especificados</span><span class="sxs-lookup"><span data-stu-id="e797e-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e797e-663">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-663">August 28, 2017</span></span>

<span data-ttu-id="e797e-664">Versão 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e797e-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e797e-665">CLI</span><span class="sxs-lookup"><span data-stu-id="e797e-665">CLI</span></span>

* <span data-ttu-id="e797e-666">Nota legal adicionada ao `--version`</span><span class="sxs-lookup"><span data-stu-id="e797e-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-667">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-667">ACS</span></span>

* <span data-ttu-id="e797e-668">Corrigidas as regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e797e-668">Corrected preview regions</span></span>
* <span data-ttu-id="e797e-669">Corrigida a formatação padrão de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="e797e-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e797e-670">Saída de comando ACS otimizada</span><span class="sxs-lookup"><span data-stu-id="e797e-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-671">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-671">Appservice</span></span>

* <span data-ttu-id="e797e-672">[ALTERAÇÃO SIGNIFICATIVA] Corrigidas as inconsistências na saída de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="e797e-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="e797e-673">Adicionado um novo alias de `-i` para `az webapp config container set --docker-custom-image-name`</span><span class="sxs-lookup"><span data-stu-id="e797e-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="e797e-674">Exposto `az webapp log show`</span><span class="sxs-lookup"><span data-stu-id="e797e-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="e797e-675">Expostos novos argumentos de `az webapp delete` para manter o plano, as métricas ou o registro de DNS do serviço de aplicativo</span><span class="sxs-lookup"><span data-stu-id="e797e-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e797e-676">Correção: detectar as configurações de slot corretamente</span><span class="sxs-lookup"><span data-stu-id="e797e-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e797e-677">IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-677">IoT</span></span>

* <span data-ttu-id="e797e-678">Correção #3934: Criação de política não limpa as políticas existentes</span><span class="sxs-lookup"><span data-stu-id="e797e-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e797e-679">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-679">Network</span></span>

* <span data-ttu-id="e797e-680">[ALTERAÇÃO SIGNIFICATIVA] `vnet list-private-access-services` renomeado para `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="e797e-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="e797e-681">[ALTERAÇÃO SIGNIFICATIVA] Opção `--private-access-services` renomeada como `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="e797e-682">Adicionado suporte para vários  intervalos de IP e portas para `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="e797e-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="e797e-683">Adicionado suporte ao SKU para `lb create`</span><span class="sxs-lookup"><span data-stu-id="e797e-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="e797e-684">Adicionado suporte ao SKU para `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="e797e-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-685">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-685">Profile</span></span>

* <span data-ttu-id="e797e-686">`--msi` e `--msi-port` expostos a logon usando a identidade de uma máquina virtual</span><span class="sxs-lookup"><span data-stu-id="e797e-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e797e-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e797e-687">Service Fabric</span></span>

* <span data-ttu-id="e797e-688">Versão prévia</span><span class="sxs-lookup"><span data-stu-id="e797e-688">Preview release</span></span>
* <span data-ttu-id="e797e-689">Simplificadas as regras de registro de usuário/senha para comando</span><span class="sxs-lookup"><span data-stu-id="e797e-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e797e-690">Corrigido o prompt de senha para o usuário mesmo após a passagem do parâmetro</span><span class="sxs-lookup"><span data-stu-id="e797e-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e797e-691">Adicionado suporte para `registry_cred` vazio</span><span class="sxs-lookup"><span data-stu-id="e797e-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-692">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-692">Storage</span></span>

* <span data-ttu-id="e797e-693">Habilitada a camada de blob de configuração</span><span class="sxs-lookup"><span data-stu-id="e797e-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="e797e-694">Adicionados os argumentos `--bypass` e `--default-action` ao `storage account [create|update]` para dar suporte ao serviço de túnel</span><span class="sxs-lookup"><span data-stu-id="e797e-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e797e-695">Comandos adicionados ao `storage account network-rule` para adicionar as regras de rede virtual e regras baseadas em IP</span><span class="sxs-lookup"><span data-stu-id="e797e-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="e797e-696">Habilitada a criptografia de serviço por chave gerenciada de cliente</span><span class="sxs-lookup"><span data-stu-id="e797e-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e797e-697">[ALTERAÇÃO SIGNIFICATIVA] Opção `--encryption` renomeada como `--encryption-services` para o comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="e797e-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e797e-698">Correção #4220: `az storage account update encryption` - incompatibilidade de sintaxe</span><span class="sxs-lookup"><span data-stu-id="e797e-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-699">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-699">VM</span></span>

* <span data-ttu-id="e797e-700">Corrigido o problema em que informações incorretas extras eram exibidas para `vmss get-instance-view` ao usar `--instance-id *`</span><span class="sxs-lookup"><span data-stu-id="e797e-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="e797e-701">Adicionado suporte ao `--lb-sku` para `vmss create`:</span><span class="sxs-lookup"><span data-stu-id="e797e-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e797e-702">Removidos nomes humanos da lista de bloqueio de nome de administrador para `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="e797e-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="e797e-703">Corrigido o problema onde `[vm|vmss] create` geraria um erro se não for possível extrair informações do plano de uma imagem</span><span class="sxs-lookup"><span data-stu-id="e797e-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e797e-704">Corrigida uma falha ao criar um conjunto de dimensionamento de máquinas virtuais com um balanceamento de carga interno</span><span class="sxs-lookup"><span data-stu-id="e797e-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e797e-705">Corrigido o problema onde o argumento `--no-wait` não funcionava com `vm availability-set create`</span><span class="sxs-lookup"><span data-stu-id="e797e-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="e797e-706">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-706">August 15, 2017</span></span>

<span data-ttu-id="e797e-707">Versão 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e797e-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-708">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-708">ACS</span></span>

* <span data-ttu-id="e797e-709">Corrigido o número da porta SSH Master0 para kubernetes</span><span class="sxs-lookup"><span data-stu-id="e797e-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-710">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-710">Appservice</span></span>

* <span data-ttu-id="e797e-711">Corrigida uma exceção ao criar um novo GIT com base no aplicativo Web Linux</span><span class="sxs-lookup"><span data-stu-id="e797e-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e797e-712">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e797e-712">Event Grid</span></span>

* <span data-ttu-id="e797e-713">Adicionadas dependências SDK</span><span class="sxs-lookup"><span data-stu-id="e797e-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e797e-714">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-714">August 11, 2017</span></span>

<span data-ttu-id="e797e-715">Versão 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e797e-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-716">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-716">ACS</span></span>

* <span data-ttu-id="e797e-717">Adicionadas mais regiões de visualização</span><span class="sxs-lookup"><span data-stu-id="e797e-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e797e-718">Batch</span><span class="sxs-lookup"><span data-stu-id="e797e-718">Batch</span></span>

* <span data-ttu-id="e797e-719">Atualizado para o Lote SDK 3.1.0 e Gerenciamento de Lote SDK 4.1.0</span><span class="sxs-lookup"><span data-stu-id="e797e-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e797e-720">Adicionado um novo comando que mostra as contagens de tarefas de um trabalho</span><span class="sxs-lookup"><span data-stu-id="e797e-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e797e-721">Corrigido o bug no processamento de URL de SAS do arquivo de recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e797e-722">Ponto de extremidade da conta de lote agora dá suporte ao prefixo opcional “https://” </span><span class="sxs-lookup"><span data-stu-id="e797e-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e797e-723">Suporte para adicionar listas de mais de 100 tarefas a um trabalho</span><span class="sxs-lookup"><span data-stu-id="e797e-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e797e-724">Adicionado log de depuração para carregar o módulo do comando de Extensões</span><span class="sxs-lookup"><span data-stu-id="e797e-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e797e-725">Componente</span><span class="sxs-lookup"><span data-stu-id="e797e-725">Component</span></span>

* <span data-ttu-id="e797e-726">Aviso de substituição adicionado aos comandos 'az component'</span><span class="sxs-lookup"><span data-stu-id="e797e-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e797e-727">Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-727">Container</span></span>

* <span data-ttu-id="e797e-728">`create`: corrigido o problema onde o sinal de igual não era permitido dentro de uma variável de ambiente</span><span class="sxs-lookup"><span data-stu-id="e797e-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e797e-729">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="e797e-729">Data Lake Store</span></span>

* <span data-ttu-id="e797e-730">Habilitado o controle do andamento</span><span class="sxs-lookup"><span data-stu-id="e797e-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e797e-731">Grade de Eventos</span><span class="sxs-lookup"><span data-stu-id="e797e-731">Event Grid</span></span>

* <span data-ttu-id="e797e-732">Versão inicial</span><span class="sxs-lookup"><span data-stu-id="e797e-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e797e-733">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-733">Network</span></span>

* <span data-ttu-id="e797e-734">`lb`: corrigido o problema onde os nomes de recursos filhos específicos não eram resolvidos corretamente quando omitidos</span><span class="sxs-lookup"><span data-stu-id="e797e-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="e797e-735">`application-gateway {subresource} delete`: corrigido o problema onde `--no-wait` não foi liquidado</span><span class="sxs-lookup"><span data-stu-id="e797e-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="e797e-736">`application-gateway http-settings update`: Corrigido o problema onde `--connection-draining-timeout` não podia ser desativado</span><span class="sxs-lookup"><span data-stu-id="e797e-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e797e-737">Corrigido o erro de argumento de palavra-chave inesperado `sa_data_size_kilobyes` com `az network vpn-connection ipsec-policy add`</span><span class="sxs-lookup"><span data-stu-id="e797e-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-738">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-738">Profile</span></span>

* <span data-ttu-id="e797e-739">`account list`: adicionado `--refresh` para sincronizar as assinaturas mais recentes do servidor</span><span class="sxs-lookup"><span data-stu-id="e797e-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-740">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-740">Storage</span></span>

* <span data-ttu-id="e797e-741">Habilitar atualização de conta de armazenamento com a identidade atribuída do sistema</span><span class="sxs-lookup"><span data-stu-id="e797e-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-742">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-742">VM</span></span>

* <span data-ttu-id="e797e-743">`availability-set`: exposta a contagem de domínios de falha durante a conversão</span><span class="sxs-lookup"><span data-stu-id="e797e-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e797e-744">Exposto o comando `list-skus`</span><span class="sxs-lookup"><span data-stu-id="e797e-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e797e-745">Suporte para atribuir identidade sem criar atribuições de função</span><span class="sxs-lookup"><span data-stu-id="e797e-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e797e-746">Aplicar o SKU de armazenamento ao anexar discos de dados</span><span class="sxs-lookup"><span data-stu-id="e797e-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e797e-747">Removido o nome do disco do sistema operacional padrão e SKU de armazenamento ao usar discos gerenciados</span><span class="sxs-lookup"><span data-stu-id="e797e-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e797e-748">28 de julho de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-748">July 28, 2017</span></span>

<span data-ttu-id="e797e-749">Versão 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e797e-749">Version 2.0.12</span></span>

* <span data-ttu-id="e797e-750">Adicionado os comandos de contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-750">Added container commands</span></span>
* <span data-ttu-id="e797e-751">Adicionados módulos de cobrança e de consumo</span><span class="sxs-lookup"><span data-stu-id="e797e-751">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e797e-752">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-752">Core</span></span>

* <span data-ttu-id="e797e-753">Informações de autenticação de SDK de saída para entidades de serviço com certificados</span><span class="sxs-lookup"><span data-stu-id="e797e-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e797e-754">Corrigidas as exceções de andamento da implantação</span><span class="sxs-lookup"><span data-stu-id="e797e-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e797e-755">Usar o ponto de extremidade do ARM da nuvem atual para criar cliente da assinatura</span><span class="sxs-lookup"><span data-stu-id="e797e-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e797e-756">Melhor manipulação simultânea do arquivo clouds.config (#3636)</span><span class="sxs-lookup"><span data-stu-id="e797e-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e797e-757">Atualização da ID de solicitação do cliente para cada execução de comando</span><span class="sxs-lookup"><span data-stu-id="e797e-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e797e-758">Criar clientes de assinatura com o perfil correto do SDK (#3635)</span><span class="sxs-lookup"><span data-stu-id="e797e-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e797e-759">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e797e-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e797e-760">Adicionado suporte para escolher campos de saída da tabela através da consulta JMESpath (#3581)</span><span class="sxs-lookup"><span data-stu-id="e797e-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e797e-761">Aprimoramento da desativação de áudio de argumentos de análise e da adição do histórico com gestos (#3434)</span><span class="sxs-lookup"><span data-stu-id="e797e-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e797e-762">Criar clientes de assinatura com o perfil correto do SDK</span><span class="sxs-lookup"><span data-stu-id="e797e-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e797e-763">Mover todos os arquivos existentes de gravação para a pasta mais recente</span><span class="sxs-lookup"><span data-stu-id="e797e-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e797e-764">Corrigida a idempotência para a criação de VM/VMSS (#3586)</span><span class="sxs-lookup"><span data-stu-id="e797e-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e797e-765">Os caminhos de comando não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e797e-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e797e-766">Determinados parâmetros do tipo booliano não diferenciam mais maiúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="e797e-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e797e-767">Suporte para logon do ADFS em um servidor local como o Azure Stack</span><span class="sxs-lookup"><span data-stu-id="e797e-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e797e-768">Corrigidas as gravações simultâneas para clouds.config (#3255)</span><span class="sxs-lookup"><span data-stu-id="e797e-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e797e-769">ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-769">ACR</span></span>

* <span data-ttu-id="e797e-770">Adicionado o comando `show-usage` para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e797e-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e797e-771">Suporte para atualização do SKU para registros gerenciados</span><span class="sxs-lookup"><span data-stu-id="e797e-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e797e-772">Adicionados registros gerenciados com o SKU gerenciado</span><span class="sxs-lookup"><span data-stu-id="e797e-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e797e-773">Adicionados webhooks para registros gerenciados com o módulo de comando de webhook do ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e797e-774">Adicionada autenticação do AAD com o comando de logon de ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e797e-775">Adicionado comando de exclusão para marcas, manifestos e repositórios do Docker</span><span class="sxs-lookup"><span data-stu-id="e797e-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-776">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-776">ACS</span></span>

* <span data-ttu-id="e797e-777">Suporte para a API versão 2017-07-01</span><span class="sxs-lookup"><span data-stu-id="e797e-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-778">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-778">Appservice</span></span>

* <span data-ttu-id="e797e-779">Corrigido o bug onde listar o aplicativo Web Linux não retornava nada</span><span class="sxs-lookup"><span data-stu-id="e797e-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e797e-780">Suporte para recuperar credenciais de ACR</span><span class="sxs-lookup"><span data-stu-id="e797e-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e797e-781">Remover todos os comandos em `appservice web`</span><span class="sxs-lookup"><span data-stu-id="e797e-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="e797e-782">Ocultar as senhas de registro do Docker da saída do comando (#3656)</span><span class="sxs-lookup"><span data-stu-id="e797e-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e797e-783">Verifique se o navegador padrão é usado no macOS sem erros (#3623)</span><span class="sxs-lookup"><span data-stu-id="e797e-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e797e-784">Aprimorada a Ajuda de `webapp log tail` e `webapp log download` (#3624)</span><span class="sxs-lookup"><span data-stu-id="e797e-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e797e-785">Exposto o comando `traffic-routing` para configurar roteamento estático (#3566)</span><span class="sxs-lookup"><span data-stu-id="e797e-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e797e-786">Adicionadas correções de confiabilidade na configuração de controle do código-fonte (#3245)</span><span class="sxs-lookup"><span data-stu-id="e797e-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e797e-787">Removido o argumento `--node-version` sem suporte de `webapp config update` para aplicativos Web do Windows.</span><span class="sxs-lookup"><span data-stu-id="e797e-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e797e-788">Em vez disso, use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span><span class="sxs-lookup"><span data-stu-id="e797e-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="e797e-789">Batch</span><span class="sxs-lookup"><span data-stu-id="e797e-789">Batch</span></span>

* <span data-ttu-id="e797e-790">Atualizado para o Lote SDK 3.0.0 com suporte para VMs de baixa prioridade em pools</span><span class="sxs-lookup"><span data-stu-id="e797e-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e797e-791">Opção `pool create` renomeada como `--target-dedicated` para `--target-dedicated-nodes`</span><span class="sxs-lookup"><span data-stu-id="e797e-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="e797e-792">Adicionadas as opções `pool create` e `--target-low-priority-nodes` de `--application-licenses`</span><span class="sxs-lookup"><span data-stu-id="e797e-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="e797e-793">CDN</span><span class="sxs-lookup"><span data-stu-id="e797e-793">CDN</span></span>

* <span data-ttu-id="e797e-794">Uma mensagem de erro mais adequada foi fornecida para `cdn endpoint list` quando o perfil especificado por `--profile-name` não existir</span><span class="sxs-lookup"><span data-stu-id="e797e-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e797e-795">Nuvem</span><span class="sxs-lookup"><span data-stu-id="e797e-795">Cloud</span></span>

* <span data-ttu-id="e797e-796">Alterada a versão de API do ponto de extremidade de metadados de nuvem para o formato AAAA-MM-DD</span><span class="sxs-lookup"><span data-stu-id="e797e-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e797e-797">Ponto de extremidade da galeria não é necessário</span><span class="sxs-lookup"><span data-stu-id="e797e-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e797e-798">Suporte para registrar a nuvem somente com o ponto de extremidade de gerenciador de recursos do ARM</span><span class="sxs-lookup"><span data-stu-id="e797e-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e797e-799">Fornecida uma opção para `cloud set` para escolher o perfil ao selecionar a nuvem atual</span><span class="sxs-lookup"><span data-stu-id="e797e-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e797e-800">Exposto `endpoint_vm_image_alias_doc`</span><span class="sxs-lookup"><span data-stu-id="e797e-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e797e-801">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-801">CosmosDB</span></span>

* <span data-ttu-id="e797e-802">Corrigida a permissão para criação de coleção com chave de partição personalizada</span><span class="sxs-lookup"><span data-stu-id="e797e-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e797e-803">Adicionado suporte para o TTL padrão de coleção</span><span class="sxs-lookup"><span data-stu-id="e797e-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e797e-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e797e-804">Data Lake Analytics</span></span>

* <span data-ttu-id="e797e-805">Adicionados comandos para gerenciamento de política de computação sob o título `dla account compute-policy`</span><span class="sxs-lookup"><span data-stu-id="e797e-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e797e-806">Adicionado `dla job pipeline show`</span><span class="sxs-lookup"><span data-stu-id="e797e-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="e797e-807">Adicionado `dla job recurrence list`</span><span class="sxs-lookup"><span data-stu-id="e797e-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e797e-808">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="e797e-808">Data Lake Store</span></span>

* <span data-ttu-id="e797e-809">Adicionado suporte para a rotação de chave de cofre de chaves gerenciado do usuário em `dls account update`</span><span class="sxs-lookup"><span data-stu-id="e797e-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="e797e-810">Atualizada a versão SDK do sistema de arquivos do Data Lake Store subjacente para resolver um problema de desempenho</span><span class="sxs-lookup"><span data-stu-id="e797e-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e797e-811">Adicionado o comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e797e-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e797e-812">Esse comando tenta permitir que um Cofre de Chaves fornecido pelo usuário use a criptografia de dados em uma conta do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e797e-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e797e-813">Interativo</span><span class="sxs-lookup"><span data-stu-id="e797e-813">Interactive</span></span>

* <span data-ttu-id="e797e-814">Melhor tempo de inicialização, usando comandos em cache</span><span class="sxs-lookup"><span data-stu-id="e797e-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e797e-815">Maior cobertura de teste</span><span class="sxs-lookup"><span data-stu-id="e797e-815">Increased test coverage</span></span>
* <span data-ttu-id="e797e-816">Aprimorado o gesto “?” para injetar também o próximo comando</span><span class="sxs-lookup"><span data-stu-id="e797e-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e797e-817">Corrigidos os erros interativos com o perfil 2017-03-09-profile-preview (#3587)</span><span class="sxs-lookup"><span data-stu-id="e797e-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e797e-818">Permitido `--version` como um parâmetro para o modo interativo (#3645)</span><span class="sxs-lookup"><span data-stu-id="e797e-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e797e-819">Impedir que o modo interativo gere erros de conclusões de validação (#3570)</span><span class="sxs-lookup"><span data-stu-id="e797e-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e797e-820">Relatório de andamento para implantações de modelo (#3510)</span><span class="sxs-lookup"><span data-stu-id="e797e-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e797e-821">Adicionado o sinalizador `--progress`</span><span class="sxs-lookup"><span data-stu-id="e797e-821">Added `--progress` flag</span></span>
* <span data-ttu-id="e797e-822">Removidos `--debug` e `--verbose` de conclusões</span><span class="sxs-lookup"><span data-stu-id="e797e-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e797e-823">Removido `interactive` de conclusões (#3324)</span><span class="sxs-lookup"><span data-stu-id="e797e-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e797e-824">IoT</span><span class="sxs-lookup"><span data-stu-id="e797e-824">IoT</span></span>

* <span data-ttu-id="e797e-825">A criação de uma política não limpa as políticas existentes.</span><span class="sxs-lookup"><span data-stu-id="e797e-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e797e-826">(#3934)</span><span class="sxs-lookup"><span data-stu-id="e797e-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e797e-827">Cofre de chaves</span><span class="sxs-lookup"><span data-stu-id="e797e-827">Key vault</span></span>

* <span data-ttu-id="e797e-828">Comandos adicionados para recursos de recuperação do cofre de chaves:</span><span class="sxs-lookup"><span data-stu-id="e797e-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="e797e-829">Subcomandos `purge`, `recover`, `keyvault list-deleted` de `keyvault`</span><span class="sxs-lookup"><span data-stu-id="e797e-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="e797e-830">Subcomandos `backup`, `restore`, `purge`, `recover`, `list-deleted` de `keyvault secret`</span><span class="sxs-lookup"><span data-stu-id="e797e-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e797e-831">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault certificate`</span><span class="sxs-lookup"><span data-stu-id="e797e-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="e797e-832">Subcomandos `purge`, `recover`, `list-deleted` de `keyvault key`</span><span class="sxs-lookup"><span data-stu-id="e797e-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="e797e-833">Adicionada a integração do cofre de chaves da entidade de serviço (#3133)</span><span class="sxs-lookup"><span data-stu-id="e797e-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e797e-834">Atualizado o plano de dados de cofre de chaves para 0.3.2.</span><span class="sxs-lookup"><span data-stu-id="e797e-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e797e-835">(#3307)</span><span class="sxs-lookup"><span data-stu-id="e797e-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e797e-836">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-836">Lab</span></span>

* <span data-ttu-id="e797e-837">Adicionado o suporte para reivindicar qualquer VM no laboratório através de `az lab vm claim`</span><span class="sxs-lookup"><span data-stu-id="e797e-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="e797e-838">Adicionado o formatador de saída da tabela para `az lab vm list` e `az lab vm show`</span><span class="sxs-lookup"><span data-stu-id="e797e-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-839">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-839">Monitor</span></span>

* <span data-ttu-id="e797e-840">Correção para o arquivo de modelo com o comando `monitor autoscale-settings get-parameters-template` (#3349)</span><span class="sxs-lookup"><span data-stu-id="e797e-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e797e-841">`monitor alert-rule-incidents list` renomeado para `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="e797e-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="e797e-842">`monitor alert-rule-incidents show` renomeado para `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="e797e-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="e797e-843">`monitor metric-defintions list` renomeado para `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="e797e-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="e797e-844">`monitor alert-rules` renomeado para `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="e797e-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="e797e-845">Alterado `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="e797e-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="e797e-846">Os subcomandos `condition` e `action` não aceitarão mais JSON</span><span class="sxs-lookup"><span data-stu-id="e797e-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e797e-847">Adicionar vários parâmetros para simplificar o processo de criação de regra</span><span class="sxs-lookup"><span data-stu-id="e797e-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="e797e-848">`location` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e797e-848">`location` no longer required</span></span>
  * <span data-ttu-id="e797e-849">Adicionar nome e o suporte a ID de destino</span><span class="sxs-lookup"><span data-stu-id="e797e-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="e797e-850">Remover `--alert-rule-resource-name`</span><span class="sxs-lookup"><span data-stu-id="e797e-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="e797e-851">Renomear `is-enabled` para `enabled` não é mais necessário</span><span class="sxs-lookup"><span data-stu-id="e797e-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="e797e-852">Padrões de `description` agora baseados na condição fornecida</span><span class="sxs-lookup"><span data-stu-id="e797e-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e797e-853">Adicionar exemplos para ajudar a esclarecer o novo formato</span><span class="sxs-lookup"><span data-stu-id="e797e-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e797e-854">Suporte para nomes ou IDs para comandos `monitor metric`</span><span class="sxs-lookup"><span data-stu-id="e797e-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e797e-855">Exemplos e argumentos de conveniência adicionados ao `monitor alert rule update`</span><span class="sxs-lookup"><span data-stu-id="e797e-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="e797e-856">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-856">Network</span></span>

* <span data-ttu-id="e797e-857">Adicionado o comando `list-private-access-services`</span><span class="sxs-lookup"><span data-stu-id="e797e-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e797e-858">Adicionado argumento `--private-access-services` para `vnet subnet create` e `vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="e797e-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="e797e-859">Corrigido o problema onde `application-gateway redirect-config create` falhava</span><span class="sxs-lookup"><span data-stu-id="e797e-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e797e-860">Corrigido o problema onde `application-gateway redirect-config update` com `--no-wait` não funcionava</span><span class="sxs-lookup"><span data-stu-id="e797e-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e797e-861">Corrigido o bug ao usar o argumento `--servers` com `application-gateway address-pool create` e `application-gateway address-pool update`</span><span class="sxs-lookup"><span data-stu-id="e797e-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="e797e-862">Adicionados os comandos `application-gateway redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e797e-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e797e-863">Adicionados os comandos para `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="e797e-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="e797e-864">Adicionados os argumentos para `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="e797e-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="e797e-865">Adicionados os argumentos para `application-gateway http-settings create` e `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="e797e-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e797e-866">Adicionados os argumentos para `application-gateway url-path-map create` e `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="e797e-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="e797e-867">Adicionado o argumento `--redirect-config` para `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="e797e-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="e797e-868">Adicionado o suporte ao `--no-wait` para `application-gateway url-path-map rule delete`</span><span class="sxs-lookup"><span data-stu-id="e797e-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="e797e-869">Adicionados os argumentos para `application-gateway probe create` e `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="e797e-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="e797e-870">Adicionado o argumento `--redirect-config` para `application-gateway rule create` e `application-gateway rule update`</span><span class="sxs-lookup"><span data-stu-id="e797e-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="e797e-871">Adicionado o suporte ao `--accelerated-networking` para `nic create` e `nic update`</span><span class="sxs-lookup"><span data-stu-id="e797e-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="e797e-872">Removido o argumento `--internal-dns-name-suffix` de `nic create`</span><span class="sxs-lookup"><span data-stu-id="e797e-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="e797e-873">Adicionado suporte ao `--dns-servers` para `nic update` e `nic create`: Adicionar suporte para servidores DNS</span><span class="sxs-lookup"><span data-stu-id="e797e-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e797e-874">Corrigido o bug onde `local-gateway create` ignorava `--local-address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="e797e-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="e797e-875">Adicionado o suporte ao `--dns-servers` para `vnet update`</span><span class="sxs-lookup"><span data-stu-id="e797e-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="e797e-876">Corrigido o bug ao criar um emparelhamento sem filtragem de rotas com `express-route peering create`</span><span class="sxs-lookup"><span data-stu-id="e797e-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="e797e-877">Corrigido o bug onde os argumentos `--provider` e `--bandwidth` não funcionavam com `express-route update`</span><span class="sxs-lookup"><span data-stu-id="e797e-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="e797e-878">Corrigido o bug com a lógica padrão de `network watcher show-topology`</span><span class="sxs-lookup"><span data-stu-id="e797e-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e797e-879">Aprimorada a formatação de saída para `network list-usages`</span><span class="sxs-lookup"><span data-stu-id="e797e-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="e797e-880">Usar IP de front-end padrão para `application-gateway http-listener create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e797e-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e797e-881">Usar o pool padrão de endereços, configurações de HTTP e o ouvinte HTTP para `application-gateway rule create`, se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e797e-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e797e-882">Usar IP de front-end e pool de back-end padrão para `lb rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e797e-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e797e-883">Usar IP de front-end padrão para `lb inbound-nat-rule create` se existir apenas um</span><span class="sxs-lookup"><span data-stu-id="e797e-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-884">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-884">Profile</span></span>

* <span data-ttu-id="e797e-885">Suporte a logon em uma VM com uma identidade gerenciada</span><span class="sxs-lookup"><span data-stu-id="e797e-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e797e-886">Suporte a saída para `account show` em formato de arquivo de autenticação do SDK</span><span class="sxs-lookup"><span data-stu-id="e797e-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e797e-887">Mostrar avisos de código obsoleto ao usar o “modo de exibição expandido”</span><span class="sxs-lookup"><span data-stu-id="e797e-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e797e-888">Adicionado o comando `get-access-token` para fornecer o token bruto do AAD</span><span class="sxs-lookup"><span data-stu-id="e797e-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e797e-889">Suporte a logon com uma conta de usuário sem nenhuma assinatura associada</span><span class="sxs-lookup"><span data-stu-id="e797e-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e797e-890">RDBMS</span><span class="sxs-lookup"><span data-stu-id="e797e-890">RDBMS</span></span>

* <span data-ttu-id="e797e-891">Suporte para listar servidores em uma assinatura (#3417)</span><span class="sxs-lookup"><span data-stu-id="e797e-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e797e-892">Corrigido o `%s` não processado devido à ausência de `% server_type` (#3393)</span><span class="sxs-lookup"><span data-stu-id="e797e-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e797e-893">Corrigido o mapa do código-fonte do documento e adicionada a tarefa CI para verificação (#3361)</span><span class="sxs-lookup"><span data-stu-id="e797e-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e797e-894">Corrigida a ajuda de MySQL e PostgreSQL (#3369)</span><span class="sxs-lookup"><span data-stu-id="e797e-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-895">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-895">Resource</span></span>

* <span data-ttu-id="e797e-896">Aprimorados os prompts para parâmetros ausentes para `group deployment create`</span><span class="sxs-lookup"><span data-stu-id="e797e-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="e797e-897">Aprimorada a análise da sintaxe `--parameters KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e797e-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e797e-898">Corrigidos os problemas onde os arquivos de parâmetros `group deployment create` não eram mais reconhecidos usando a sintaxe `@<file>`</span><span class="sxs-lookup"><span data-stu-id="e797e-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e797e-899">Suporte do argumento `--ids` para os comandos `resource` e `managedapp`</span><span class="sxs-lookup"><span data-stu-id="e797e-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e797e-900">Corrigidas algumas mensagens de erro e análise (#3584)</span><span class="sxs-lookup"><span data-stu-id="e797e-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e797e-901">Corrigida a análise de `--resource-type` para o comando `lock` aceitar `<resource-namespace>` e `<resource-type>`</span><span class="sxs-lookup"><span data-stu-id="e797e-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="e797e-902">Adicionados parâmetros de verificação para modelos de link do modelo (#3629)</span><span class="sxs-lookup"><span data-stu-id="e797e-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e797e-903">Adicionado suporte para especificar parâmetros de implantação usando a sintaxe `KEY=VALUE`</span><span class="sxs-lookup"><span data-stu-id="e797e-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e797e-904">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-904">Role</span></span>

* <span data-ttu-id="e797e-905">Suporte à saída no formato de arquivo de autenticação do SDK para `create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="e797e-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="e797e-906">Limpar as atribuições de função e aplicativos relacionados ao AAD ao excluir uma entidade de serviço (#3610)</span><span class="sxs-lookup"><span data-stu-id="e797e-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e797e-907">Incluir o formato de hora nos argumentos `app create` e descrições `--start-date` e `--end-date`</span><span class="sxs-lookup"><span data-stu-id="e797e-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e797e-908">Mostrar avisos de código obsoleto ao usar `--expanded-view`</span><span class="sxs-lookup"><span data-stu-id="e797e-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="e797e-909">Adicionada a integração do cofre de chaves para os comandos `create-for-rbac` e `reset-credentials`</span><span class="sxs-lookup"><span data-stu-id="e797e-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e797e-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e797e-910">Service Fabric</span></span>
* <span data-ttu-id="e797e-911">Corrigido um problema com arquivos grandes em aplicativos que eram truncados ao serem carregados (#3666)</span><span class="sxs-lookup"><span data-stu-id="e797e-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e797e-912">Adicionados testes para os comandos do Service Fabric (#3424)</span><span class="sxs-lookup"><span data-stu-id="e797e-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e797e-913">Corrigidos vários comandos do Service Fabric (#3234)</span><span class="sxs-lookup"><span data-stu-id="e797e-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-914">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-914">SQL</span></span>

* <span data-ttu-id="e797e-915">Removido o parâmetro `sql server create` `--identity`</span><span class="sxs-lookup"><span data-stu-id="e797e-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e797e-916">Remover os valores de senha da saída dos comandos `sql server create` e `sql server update`</span><span class="sxs-lookup"><span data-stu-id="e797e-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e797e-917">Adicionados os comandos para `sql db list-editions` e `sql elastic-pool list-editions`</span><span class="sxs-lookup"><span data-stu-id="e797e-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-918">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-918">Storage</span></span>

* <span data-ttu-id="e797e-919">Removida a opção `--marker` dos comandos `storage blob list`, `storage container list`, e `storage share list` (#3745)</span><span class="sxs-lookup"><span data-stu-id="e797e-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e797e-920">Habilitado a criação de uma conta de armazenamento somente para https</span><span class="sxs-lookup"><span data-stu-id="e797e-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e797e-921">Atualizadas as métricas de armazenamento, registro em log e os comandos do CORS (#3495)</span><span class="sxs-lookup"><span data-stu-id="e797e-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e797e-922">Mensagem de exceção reformulada do ADD do CORS adicionar (#3638) (#3362)</span><span class="sxs-lookup"><span data-stu-id="e797e-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e797e-923">Convertido o gerador para uma lista no modo de simulação de comando do lote de download (#3592)</span><span class="sxs-lookup"><span data-stu-id="e797e-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e797e-924">Corrigido o problema de simulação do lote de download de blob (#3640) (#3592)</span><span class="sxs-lookup"><span data-stu-id="e797e-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-925">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-925">VM</span></span>

* <span data-ttu-id="e797e-926">Suporte para configuração de NSG</span><span class="sxs-lookup"><span data-stu-id="e797e-926">Support configuring nsg</span></span>
* <span data-ttu-id="e797e-927">Corrigido o bug onde o servidor DNS não era configurado corretamente</span><span class="sxs-lookup"><span data-stu-id="e797e-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e797e-928">Suporte às identidades de serviço gerenciado</span><span class="sxs-lookup"><span data-stu-id="e797e-928">Support managed service identities</span></span>
* <span data-ttu-id="e797e-929">Corrigido o problema onde `cmss create` com um balanceador de carga existente exigia `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="e797e-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="e797e-930">Os discos de dados criados com LUN do `vm image create` agora começam com 0</span><span class="sxs-lookup"><span data-stu-id="e797e-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e797e-931">10 de maio de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-931">May 10, 2017</span></span>

<span data-ttu-id="e797e-932">Versão 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e797e-932">Version 2.0.6</span></span>

* <span data-ttu-id="e797e-933">Renomeação do DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e797e-934">Adição do RDBMS (MySQL, Postgres)</span><span class="sxs-lookup"><span data-stu-id="e797e-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e797e-935">Inclusão dos módulos Data Lake Analytics e Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e797e-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e797e-936">Inclusão do módulo Serviços Cognitivos</span><span class="sxs-lookup"><span data-stu-id="e797e-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="e797e-937">Inclusão do módulo Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e797e-937">Include Service Fabric module</span></span>
* <span data-ttu-id="e797e-938">Inclusão do módulo Interativo (renomeação de az-shell)</span><span class="sxs-lookup"><span data-stu-id="e797e-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e797e-939">Adição de suporte para comandos CDN</span><span class="sxs-lookup"><span data-stu-id="e797e-939">Add support for CDN commands</span></span>
* <span data-ttu-id="e797e-940">Remoção do módulo Contêiner</span><span class="sxs-lookup"><span data-stu-id="e797e-940">Remove Container module</span></span>
* <span data-ttu-id="e797e-941">Adição de “az -v” como atalho para “az --version” ([nº 2926](https://github.com/Azure/azure-cli/issues/2926))</span><span class="sxs-lookup"><span data-stu-id="e797e-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e797e-942">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e797e-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e797e-943">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-943">Core</span></span>

* <span data-ttu-id="e797e-944">núcleo: captura de exceções causadas por um provedor não registrado e seu registro automático</span><span class="sxs-lookup"><span data-stu-id="e797e-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e797e-945">desempenho: persistência do cache de tokens do ADAL na memória até o encerramento do processo ([nº 2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="e797e-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e797e-946">Correção de bytes retornados da impressão digital hexadecimal -o tsv ([nº 3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="e797e-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e797e-947">Melhoria do download do Certificado do Key Vault e da integração de SP do AAD ([nº 3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="e797e-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e797e-948">Adição da localização do Python a “az —version” ([nº 2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="e797e-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e797e-949">logon: suporte ao logon quando não há nenhuma assinatura ([nº 2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="e797e-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e797e-950">núcleo: correção de uma falha ao fazer logon usando uma entidade de serviço duas vezes ([nº 2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="e797e-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e797e-951">núcleo: permissão ao caminho do arquivo accessTokens.json para ser configurável por meio de um env var ([nº 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="e797e-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e797e-952">núcleo: permissão aos padrões configurados para serem aplicados em argumentos opcionais ([nº 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="e797e-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e797e-953">núcleo: melhoria do desempenho</span><span class="sxs-lookup"><span data-stu-id="e797e-953">core: Improved performance</span></span>
* <span data-ttu-id="e797e-954">núcleo: Certificados de AC personalizados – suporte à configuração da variável de ambiente REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="e797e-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e797e-955">núcleo: configuração na nuvem – uso do ponto de extremidade do “Resource Manager” caso o ponto de extremidade de “Gerenciamento” não esteja definido</span><span class="sxs-lookup"><span data-stu-id="e797e-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-956">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-956">ACS</span></span>

* <span data-ttu-id="e797e-957">correção da contagem mestre e de agente para ser inteiro em vez de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e797e-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e797e-958">exposição de “az acs create --no-wait” e “az acs wait” para a criação assíncrona</span><span class="sxs-lookup"><span data-stu-id="e797e-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e797e-959">exposição de “az acs create --validate” para validações de simulação</span><span class="sxs-lookup"><span data-stu-id="e797e-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e797e-960">remoção do perfil do Windows antes da chamada PUT ao comando scale ([nº 2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="e797e-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-961">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-961">AppService</span></span>

* <span data-ttu-id="e797e-962">functionapp: adição de suportes completos a functionapp, incluindo create, show, list, delete, hostname, ssl, etc.</span><span class="sxs-lookup"><span data-stu-id="e797e-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e797e-963">Adição do VSTS (Team Services) como uma opção de entrega contínua a “appservice web source-control config”</span><span class="sxs-lookup"><span data-stu-id="e797e-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e797e-964">Criação de “az webapp” para substituição de “az appservice web” (para compatibilidade com versões anteriores, “az appservice web” permanecerá por duas versões)</span><span class="sxs-lookup"><span data-stu-id="e797e-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e797e-965">Exposição de argumentos para configurar a implantação e as “pilhas em tempo de execução” em webapp create</span><span class="sxs-lookup"><span data-stu-id="e797e-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e797e-966">Exposição de “webapp list-runtimes”</span><span class="sxs-lookup"><span data-stu-id="e797e-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e797e-967">suporte à configuração de cadeias de conexão ([nº 2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="e797e-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e797e-968">suporte à permuta de slots com visualização</span><span class="sxs-lookup"><span data-stu-id="e797e-968">support slot swap with preview</span></span>
* <span data-ttu-id="e797e-969">Correção de erros em comandos appservice ([nº 2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="e797e-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e797e-970">Uso do grupo de recursos do plano do serviço de aplicativo para operações de certificado ([nº 2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="e797e-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e797e-971">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-971">CosmosDB</span></span>

* <span data-ttu-id="e797e-972">Renomeação do módulo DocumentDB para CosmosDB</span><span class="sxs-lookup"><span data-stu-id="e797e-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e797e-973">Adição de suporte para APIs do plano de dados do DocumentDB: gerenciamento de banco de dados e de coleção</span><span class="sxs-lookup"><span data-stu-id="e797e-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e797e-974">Adição de suporte para habilitar o failover automático em contas de banco de dados</span><span class="sxs-lookup"><span data-stu-id="e797e-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e797e-975">Adição de suporte para nova política de consistência ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="e797e-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e797e-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e797e-976">Data Lake Analytics</span></span>

* <span data-ttu-id="e797e-977">Correção de um bug em que a filtragem no resultado e no estado das listas de trabalho gera um erro</span><span class="sxs-lookup"><span data-stu-id="e797e-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e797e-978">Adição de suporte para o novo tipo de item de catálogo: pacote.</span><span class="sxs-lookup"><span data-stu-id="e797e-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e797e-979">acessado por meio de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="e797e-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="e797e-980">Possibilidade de listar os seguintes itens de catálogo no banco de dados (sem a necessidade de especificação de esquema):</span><span class="sxs-lookup"><span data-stu-id="e797e-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e797e-981">Tabela</span><span class="sxs-lookup"><span data-stu-id="e797e-981">Table</span></span>
  * <span data-ttu-id="e797e-982">Função com valor de tabela</span><span class="sxs-lookup"><span data-stu-id="e797e-982">Table valued function</span></span>
  * <span data-ttu-id="e797e-983">Visualizar</span><span class="sxs-lookup"><span data-stu-id="e797e-983">View</span></span>
  * <span data-ttu-id="e797e-984">Estatísticas de Tabela.</span><span class="sxs-lookup"><span data-stu-id="e797e-984">Table Statistics.</span></span> <span data-ttu-id="e797e-985">Isso também pode ser listado com um esquema, mas sem a especificação de um nome de tabela</span><span class="sxs-lookup"><span data-stu-id="e797e-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e797e-986">Repositório Data Lake</span><span class="sxs-lookup"><span data-stu-id="e797e-986">Data Lake Store</span></span>

* <span data-ttu-id="e797e-987">Atualização da versão do SDK do sistema de arquivos subjacente, que fornece melhor suporte para lidar com cenários de limitação do servidor</span><span class="sxs-lookup"><span data-stu-id="e797e-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e797e-988">Melhoria do desempenho de carregamento de pacote e execução de comando ([nº 2819](https://github.com/Azure/azure-cli/issues/2819))</span><span class="sxs-lookup"><span data-stu-id="e797e-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e797e-989">Ausência de ajuda para mostrar o acesso.</span><span class="sxs-lookup"><span data-stu-id="e797e-989">missed help for access show.</span></span> <span data-ttu-id="e797e-990">Adição em andamento.</span><span class="sxs-lookup"><span data-stu-id="e797e-990">adding it.</span></span> <span data-ttu-id="e797e-991">([nº 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e797e-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e797e-992">Localizar</span><span class="sxs-lookup"><span data-stu-id="e797e-992">Find</span></span>

* <span data-ttu-id="e797e-993">melhoria dos resultados da pesquisa e permissão de controle de versão do índice de pesquisa</span><span class="sxs-lookup"><span data-stu-id="e797e-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e797e-994">KeyVault</span><span class="sxs-lookup"><span data-stu-id="e797e-994">KeyVault</span></span>

* <span data-ttu-id="e797e-995">BC:`az keyvault certificate download` alteração de -e da cadeia de caracteres ou do binário para PEM ou DER a fim de representar melhor as opções</span><span class="sxs-lookup"><span data-stu-id="e797e-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e797e-996">BC: remoção de --expires e --not-before de `keyvault certificate create`, pois esses parâmetros não têm suporte no serviço</span><span class="sxs-lookup"><span data-stu-id="e797e-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e797e-997">Adição do parâmetro --validity a `keyvault certificate create` para substituir seletivamente o valor em --policy</span><span class="sxs-lookup"><span data-stu-id="e797e-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e797e-998">Correção do problema em `keyvault certificate get-default-policy`, em que “expires” e “not_before” eram expostos, ao contrário de “validity_in_months”</span><span class="sxs-lookup"><span data-stu-id="e797e-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e797e-999">Correção do cofre de chaves para importação de PEM e PFX ([nº 2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="e797e-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e797e-1000">Laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1000">Lab</span></span>

* <span data-ttu-id="e797e-1001">Adição dos comandos create, show, delete e list ao ambiente do laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e797e-1002">Adição dos comandos show e list para exibir modelos ARM no laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e797e-1003">Adição do sinalizador --environment a `az lab vm list` para filtrar as VMs por ambiente no laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e797e-1004">Adição do comando de conveniência `az lab formula export-artifacts` para exportar o scaffold de artefato em uma fórmula do Laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e797e-1005">Adição de comandos para gerenciar segredos em um Laboratório</span><span class="sxs-lookup"><span data-stu-id="e797e-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e797e-1006">Monitoramento</span><span class="sxs-lookup"><span data-stu-id="e797e-1006">Monitor</span></span>

* <span data-ttu-id="e797e-1007">Correção de bug: modelagem de `--actions` de `az alert-rules create` para consumir a cadeia de caracteres JSON ([nº 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="e797e-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e797e-1008">Correção de bug – as configurações de diagnóstico criam, mas não aceitam logs e métrica de comandos show ([nº 2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="e797e-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e797e-1009">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-1009">Network</span></span>

* <span data-ttu-id="e797e-1010">Adição do comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="e797e-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e797e-1011">Adição de suporte para o parâmetro `--filters` de `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="e797e-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="e797e-1012">Adição de suporte para drenagem de conexão do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e797e-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e797e-1013">Adição de suporte para a configuração do conjunto de regras WAF do Gateway de Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e797e-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e797e-1014">Adição de suporte para filtros de rota e regras do ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="e797e-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e797e-1015">Adição de suporte para o roteamento geográfico do Gerenciador de Tráfego</span><span class="sxs-lookup"><span data-stu-id="e797e-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e797e-1016">Adição de suporte para seletores de tráfego baseados em política da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e797e-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e797e-1017">Adição de suporte para políticas IPsec da conexão VPN</span><span class="sxs-lookup"><span data-stu-id="e797e-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e797e-1018">Correção de um bug com `vpn-connection create` ao usar os parâmetros `--no-wait` ou `--validate`</span><span class="sxs-lookup"><span data-stu-id="e797e-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e797e-1019">Adição de suporte para gateways de VNet ativos/ativos</span><span class="sxs-lookup"><span data-stu-id="e797e-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e797e-1020">Remoção de valores nulos na saída de comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="e797e-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e797e-1021">BC: correção de um bug na saída de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="e797e-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="e797e-1022">Correção de um bug em que o argumento “--key-length” de “vpn-connection create” não é analisado corretamente</span><span class="sxs-lookup"><span data-stu-id="e797e-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e797e-1023">Correção de um bug em `dns zone import`, em que os registros não são importados corretamente</span><span class="sxs-lookup"><span data-stu-id="e797e-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e797e-1024">Correção de um bug em que `traffic-manager endpoint update` não funciona</span><span class="sxs-lookup"><span data-stu-id="e797e-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e797e-1025">Adição de comandos de visualização “network watcher”</span><span class="sxs-lookup"><span data-stu-id="e797e-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e797e-1026">Perfil</span><span class="sxs-lookup"><span data-stu-id="e797e-1026">Profile</span></span>

* <span data-ttu-id="e797e-1027">Suporte ao logon quando não há nenhuma assinatura encontrada ([nº 2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="e797e-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e797e-1028">Suporte ao nome curto do parâmetro em az account set --subscription ([nº 2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="e797e-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e797e-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="e797e-1029">Redis</span></span>

* <span data-ttu-id="e797e-1030">Adição do comando update que também adiciona a capacidade de dimensionar o Cache Redis</span><span class="sxs-lookup"><span data-stu-id="e797e-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e797e-1031">Preterição do comando “update-settings”</span><span class="sxs-lookup"><span data-stu-id="e797e-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e797e-1032">Recurso</span><span class="sxs-lookup"><span data-stu-id="e797e-1032">Resource</span></span>

* <span data-ttu-id="e797e-1033">Adição dos comandos de definição managedapp e managedapp ([nº 2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="e797e-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e797e-1034">Suporte aos comandos “provider operation” ([nº 2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="e797e-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e797e-1035">Suporte à criação de recurso genérico ([nº 2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="e797e-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e797e-1036">Correção da análise de recurso e da pesquisa de versão de API.</span><span class="sxs-lookup"><span data-stu-id="e797e-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e797e-1037">([nº 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e797e-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e797e-1038">Adição de documentos a az lock update.</span><span class="sxs-lookup"><span data-stu-id="e797e-1038">Add docs for az lock update.</span></span> <span data-ttu-id="e797e-1039">([nº 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e797e-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e797e-1040">Erro ao tentar listar recursos de um grupo que não existe.</span><span class="sxs-lookup"><span data-stu-id="e797e-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e797e-1041">([nº 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e797e-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e797e-1042">[Computação] Correção de problemas com a atualização do conjunto de disponibilidade da VMSS e da VM.</span><span class="sxs-lookup"><span data-stu-id="e797e-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e797e-1043">([nº 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e797e-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e797e-1044">Correção de lock create e delete se parent-resource-path é None ([nº 2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="e797e-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e797e-1045">Função</span><span class="sxs-lookup"><span data-stu-id="e797e-1045">Role</span></span>

* <span data-ttu-id="e797e-1046">create-for-rbac: garantia de que a data de término do SP não excederá a data de validade do certificado ([nº 2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="e797e-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e797e-1047">RBAC: adição de suporte completo a “ad group” ([nº 2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="e797e-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e797e-1048">função: correção de problemas na atualização de definição de função ([nº 2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="e797e-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e797e-1049">create-for-rbac: garantia de que a senha fornecida pelo usuário é coletada</span><span class="sxs-lookup"><span data-stu-id="e797e-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e797e-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="e797e-1050">SQL</span></span>

* <span data-ttu-id="e797e-1051">Adição dos comandos az sql server list-usages e az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="e797e-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e797e-1052">SQL – capacidade de se conectar diretamente ao provedor de recursos ([nº 2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="e797e-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e797e-1053">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-1053">Storage</span></span>

* <span data-ttu-id="e797e-1054">Localização padrão da localização do grupo de recursos de `storage account create`</span><span class="sxs-lookup"><span data-stu-id="e797e-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="e797e-1055">Adição de suporte para cópia incremental de blob</span><span class="sxs-lookup"><span data-stu-id="e797e-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e797e-1056">Adição de suporte para upload de blobs de blocos grandes</span><span class="sxs-lookup"><span data-stu-id="e797e-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="e797e-1057">Alteração do tamanho do bloco para 100MB quando o arquivo a ser carregado é maior que 200GB</span><span class="sxs-lookup"><span data-stu-id="e797e-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-1058">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-1058">VM</span></span>

* <span data-ttu-id="e797e-1059">avail-set: as contagens de domínio de UD e FD agora são opcionais</span><span class="sxs-lookup"><span data-stu-id="e797e-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e797e-1060">observação: comandos da VM em nuvens soberanas Evite recursos relacionados ao disco gerenciado, incluindo os seguintes:</span><span class="sxs-lookup"><span data-stu-id="e797e-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e797e-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e797e-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e797e-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e797e-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e797e-1063">Em “az vm/vmss create”, use “—use-unmanaged-disk” para evitar o disco gerenciado Outros comandos deverão funcionar</span><span class="sxs-lookup"><span data-stu-id="e797e-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e797e-1064">VM/VMSS: melhoria do texto de aviso ao gerar pares de chaves SSH</span><span class="sxs-lookup"><span data-stu-id="e797e-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e797e-1065">VM/VMSS: suporte à criação com base em uma imagem do Marketplace que exige informações de plano ([nº 1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="e797e-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e797e-1066">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-1066">April 3, 2017</span></span>

<span data-ttu-id="e797e-1067">Versão 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e797e-1067">Version 2.0.2</span></span>

<span data-ttu-id="e797e-1068">Lançamos os componentes ACR, Batch, KeyVault, e SQL nessa versão</span><span class="sxs-lookup"><span data-stu-id="e797e-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e797e-1069">Núcleo</span><span class="sxs-lookup"><span data-stu-id="e797e-1069">Core</span></span>

* <span data-ttu-id="e797e-1070">Adicionar módulos acr, laboratório, monitor e localizar à lista padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e797e-1071">Logon: ignorar locatário errado ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="e797e-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e797e-1072">logon: definir assinatura padrão como um com o estado de "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="e797e-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e797e-1073">Adicionar comandos de espera e suporte --no-wait para mais comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e797e-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e797e-1074">núcleo: suporte a logon usando a entidade de serviço com um certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="e797e-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e797e-1075">Adicione solicitação para parâmetros de modelo ausentes.</span><span class="sxs-lookup"><span data-stu-id="e797e-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e797e-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="e797e-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e797e-1077">Suporte à definição de valores padrão para os argumentos comuns como grupo de recursos padrão, Web padrão, vm padrão</span><span class="sxs-lookup"><span data-stu-id="e797e-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e797e-1078">Suporte a logon para um locatário específico</span><span class="sxs-lookup"><span data-stu-id="e797e-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e797e-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="e797e-1079">ACS</span></span>

* <span data-ttu-id="e797e-1080">[ACS] Adicionar suporte para configurar um cluster do ACS padrão ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="e797e-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e797e-1081">Adicione suporte para solicitação de senha de chave ssh.</span><span class="sxs-lookup"><span data-stu-id="e797e-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e797e-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="e797e-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e797e-1083">Adicione suporte para clusters do windows.</span><span class="sxs-lookup"><span data-stu-id="e797e-1083">Add support for windows clusters.</span></span> <span data-ttu-id="e797e-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="e797e-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e797e-1085">Alterne da função Proprietário para Colaborador.</span><span class="sxs-lookup"><span data-stu-id="e797e-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e797e-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="e797e-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e797e-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="e797e-1087">AppService</span></span>

* <span data-ttu-id="e797e-1088">AppService: suporte para obter o endereço ip externo usado para registros de DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="e797e-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e797e-1089">AppService: suporte à associação de certificados curinga ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="e797e-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e797e-1090">AppService: lista de suporte à publicação de perfis ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="e797e-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e797e-1091">AppService - Aciona a sincronização de controle de origem após a configuração ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="e797e-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e797e-1092">DataLake</span><span class="sxs-lookup"><span data-stu-id="e797e-1092">DataLake</span></span>

* <span data-ttu-id="e797e-1093">Versão inicial do módulo do Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e797e-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e797e-1094">Versão inicial do módulo do Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e797e-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e797e-1095">DocuemntDB</span><span class="sxs-lookup"><span data-stu-id="e797e-1095">DocuemntDB</span></span>

* <span data-ttu-id="e797e-1096">DocumentDB: Adicionar suporte para a listagem de cadeias de conexão ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="e797e-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e797e-1097">VM</span><span class="sxs-lookup"><span data-stu-id="e797e-1097">VM</span></span>

* <span data-ttu-id="e797e-1098">[Compute] Adicionar suporte a AppGateway para criar o conjunto de dimensionamento de máquinas virtuais ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="e797e-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e797e-1099">[VM/VMSS] Suporte aprimorado ao cache de disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="e797e-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e797e-1100">VM/VMSS: incorporar a lógica de validação de credenciais usada pelo portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="e797e-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e797e-1101">Adicionar comandos de espera e suporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="e797e-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e797e-1102">Conjunto de dimensionamento de máquinas virtuais: suporte à \* para listar a exibição de instâncias em vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="e797e-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e797e-1103">Adicionar: segredos da VM e do conjunto de dimensionamento de máquinas virtuais ([2212}(https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="e797e-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="e797e-1104">Permitir a criação de VMs com VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="e797e-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e797e-1105">27 de fevereiro de 2017</span><span class="sxs-lookup"><span data-stu-id="e797e-1105">February 27, 2017</span></span>

<span data-ttu-id="e797e-1106">Versão 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e797e-1106">Version 2.0.0</span></span>

<span data-ttu-id="e797e-1107">Esta versão da CLI do Azure 2.0 é a primeira versão "Amplamente Disponível". A disponibilidade geral se aplica a estes módulos de comando:</span><span class="sxs-lookup"><span data-stu-id="e797e-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e797e-1108">Serviço de Contêiner (acs)</span><span class="sxs-lookup"><span data-stu-id="e797e-1108">Container Service (acs)</span></span>
- <span data-ttu-id="e797e-1109">Computação (incluindo Gerenciador de Recursos, VM, conjunto de dimensionamento de máquinas virtuais, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="e797e-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e797e-1110">Rede</span><span class="sxs-lookup"><span data-stu-id="e797e-1110">Networking</span></span>
- <span data-ttu-id="e797e-1111">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="e797e-1111">Storage</span></span>

<span data-ttu-id="e797e-1112">Esses módulos de comando podem ser usados na produção e têm suporte do SLA padrão da Microsoft. Você pode abrir problemas diretamente com o suporte da Microsoft ou em nossa [lista de problemas do github](https://github.com/azure/azure-cli/issues/). Faça perguntas no [StackOverflow usando a marca azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), ou contate a equipe de produto em [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) Forneça comentários na linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e797e-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e797e-1113">Os comandos nesses módulos são estáveis e a sintaxe não deve ser alterada em versões futuras dessa versão da CLI do Azure</span><span class="sxs-lookup"><span data-stu-id="e797e-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e797e-1114">Para verificar a versão da CLI, use `az --version` A saída lista a versão da CLI (2.0.0 nessa versão), os módulos de comando individuais, as versões do Python e GCC que você está usando</span><span class="sxs-lookup"><span data-stu-id="e797e-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e797e-1115">Alguns dos módulos de comando têm um sufixo "b*n*" ou "rc*n*". Esses módulos de comando ainda estão em versão prévia e estarão disponíveis no futuro</span><span class="sxs-lookup"><span data-stu-id="e797e-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e797e-1116">Também temos compilações de versão prévia noturnas da CLI. Para obter informações, consulte essas instruções sobre [como obter as compilações diárias](https://github.com/Azure/azure-cli#nightly-builds) e essas instruções sobre [configuração do desenvolvedor e código de contribuição](https://github.com/Azure/azure-cli#developer-setup)</span><span class="sxs-lookup"><span data-stu-id="e797e-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e797e-1117">Você pode relatar problemas com as compilações de visualização diárias das seguintes maneiras:</span><span class="sxs-lookup"><span data-stu-id="e797e-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e797e-1118">Relatar problemas na [lista de problemas do github](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="e797e-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e797e-1119">Entre em contato com a equipe do produto no endereço [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="e797e-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e797e-1120">Forneça comentários a partir da linha de comando com o comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="e797e-1120">Provide feedback from the command line with the `az feedback` command</span></span>

